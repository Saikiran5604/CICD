# CICD
I wanted to learn about CICD setup the better to start is by hands on .
 
### Flow 
1. create a simple web application 
2. Write the Docker file for it 
3. Build the Docker image and push to registry 
4. Expose the port and run the container and verify if the website is accesable from localhost:8080

This is the manual steps so when ever i create a change/update in the web application code i need to manually build the image and then run the container and verify if the application is accessiable 

to prevent this manual effort we design a CICD in github actions 
When ever to push the code the CICD pipeline will be trigger and it will build the image and push ECR and run the container and will do the checks as well 
We can add test-cases as well and delete the old image if not required .

