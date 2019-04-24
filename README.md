# Insight DevOps Engineering Systems Puzzle

Tested and deployed on an Ubuntu server with AWS EC2 service.

Feel free to check it at http://13.58.143.238:8080.

Run the service using following commands:
```
docker-compose up -d db
docker-compose run --rm flaskapp /bin/bash -c "cd /opt/services/flaskapp/src && python -c  'import database; database.init_db()'"
docker-compose up -d
```
