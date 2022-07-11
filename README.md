# messaging-service-rabbitmq

Demo application for Background Processing with RabbitMQ, Python & Flask

## Description

Checkout _requirements.txt_ for libraries used.

Install RabbitMQ using Docker’s official management image.

Connect to http://locahost:15672 and see the RabbitMQ management console.

Use the username and password guest to login.

Use the following command to run the docker and start all the processes:

#### _docker-compose up -d_
```
Starting demo_app_rabbitmq_1 ... done
Starting demo_app_worker_1   ... done
Starting demo_app_server_1   ... done
```

_localhost:5000/create-job/_ 
just hit above end-point on your localhost and you will see the messages flowing through.

Now you can check message is received by Worker by checking logs:

#### _docker logs demo_app_worker_1_
```
Connecting to server ...
Waiting for messages...
Received hii
Done
```


## Versions

Python: 3.9

## Install dependencies

pip install -r requirements.txt

## Running the app

python run.py


