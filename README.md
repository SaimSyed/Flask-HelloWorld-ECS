# Flask-HelloWorld-ECS

Agenda: Dockerize a simple "Hello World" Flask App (first on a virtual machine and then on AWS ECS Serice). This app will be completly cloud native.

Create a virtual machine/ec2 instance (as this is simple hello world flask app any free tier like t2.mico will be enough)

Create the Flask application app.py and requirements.txt.

Create a simple Dockerfile to containerize our Flask App (app.py).

Build the container from the image and assign ports to the container.

Curl 0.0.0.0/5000 (You must get the response with a message that is set up as an environment variable )

Commit this container image to AWS ECR with AWS CLI. (You can also commit this first on docker hub and can fetch this image while creating tasks in ECS.)

Make a cluster on AWS ECS (I'm going to choose fargate networking only for zero downtime)

Create basics task defination, create service to run tasks (configue LB and AS as per requirement) and create container from the image and assign ports.

Search in web browser the Public IP of container *publicip:5000*
you should get your environment message
![OpsLyft](https://user-images.githubusercontent.com/98846014/159041755-d21cba54-8d1f-4bff-9acb-629f8385a14f.png)
