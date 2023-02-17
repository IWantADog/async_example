# start
- grpc server: 
  ```
  python server.py
  ```
- flask server: 
  ```
  gunicorn -c flask_app/gunicorn.conf.py 'flask_app.app:app'
  ```
- test client:
  ```
  ab -r -n 2000 -c 200 http://127.0.0.1:8000/greet/\?ident\=1
  ```