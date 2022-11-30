docker build . --tag=task_1

docker run -d -p 8000:80 task_1

http://localhost:8000
