# face-landmark-detection-system
An ML model inference system. 

The project involves training a facial landmark detection model, deploying it in a production environment with Docker containers, creating a web application for facial point detection via POST requests, storing images in an S3 bucket and their corresponding facial point coordinates in a NoSQL database. 



## Stage 1
- Train a prototype of the model. Training is performed via pytorch lightning. Add logging via MLFlow
- Create a backend server 
- The model is inferred from a .pt file on in each container
- Containerize each application 


## Stage 2
- Add a noSQL database for landmark storage
- Add an S3 bucket for image storage 


## Stage 3
- Add ngingx for proxing and backend load balancing


## Stage 4
- Use triton inference server instead of regular containers with the .pt model
- Convert the model to ONNX format
- Add gRPC protocol for communication between the backend and inferenece containers

## Stage 5
- Add orchestration (Docker Swarm would be enough)



