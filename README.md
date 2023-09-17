# Hajar Banyalmarjeh
# This project is to get messages from the console and to get messages where the producer will read from a csv file, in this case, the file is called csv. 

# streaming-04-multiple-consumers

> Use RabbitMQ to distribute tasks to multiple workers

One process will create task messages. Multiple worker processes will share the work. 


## Before You Begin

1. Fork this starter repo into your GitHub.
1. Clone your repo down to your machine.
1. View / Command Palette - then Python: Select Interpreter
1. Select your conda environment. 

## Read

1. Read the [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)
1. Read the code and comments in this repo.

## RabbitMQ Admin 

RabbitMQ comes with an admin panel. When you run the task emitter, reply y to open it. 

(Python makes it easy to open a web page - see the code to learn how.)

## Execute the Producer

1. Run emitter_of_tasks.py (say y to monitor RabbitMQ queues)

Explore the RabbitMQ website.

<img width="1495" alt="Screenshot 2023-09-15 at 8 06 59 PM" src="https://github.com/Hajarbany/streaming-04-multiple-consumers/assets/97689037/66df10d4-7274-40e5-b41f-bfa528dd1cb6">

## Execute a Consumer / Worker

1. Run listening_worker.py

Will it terminate on its own? How do you know? Yes it terminated on it's own once it received all the messages 

## Ready for Work

1. Use your emitter_of_tasks to produce more task messages.

## Start Another Listening Worker 

1. Use your listening_worker.py script to launch a second worker. 

Follow the tutorial. 
Add multiple tasks (e.g. First message, Second message, etc.)
How are tasks distributed? Each task gets received after the other 
Monitor the windows with at least two workers. 
Which worker gets which tasks?


## Reference

- [RabbitMQ Tutorial - Work Queues](https://www.rabbitmq.com/tutorials/tutorial-two-python.html)


## Screenshot

See a running example with at least 3 concurrent process windows here:
<img width="1225" alt="Screenshot 2023-09-15 at 8 07 51 PM" src="https://github.com/Hajarbany/streaming-04-multiple-consumers/assets/97689037/893433fc-e4ca-4eb3-a68f-dead080c090f">

