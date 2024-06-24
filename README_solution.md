**Problem statement 1:**

Step 1: Fork the Repository
Step 2: Clone the Forked Repository
Step 3: Set Up Jenkins
        Start Jenkins and open the Jenkins dashboard at http://localhost:3000.
        Install necessary plugins: "NodeJS Plugin" and "Pipeline".
Step 4: Modify the Application to Serve on Port 3004        
Step 5: Create Jenkins Pipeline -  **Jenkinsfile** in this repo
Step 6: Configure pipeline 
        Go to Jenkins Dashboard.
        Click on "New Item", enter an item name, select "Pipeline", and click "OK".
        In the "Pipeline" section, select "Pipeline script from SCM".
        Choose "Git" and enter your repository URL.
        Set the "Branch Specifier" to */main (or the branch you are using).
        Click "Save" and then "Build Now" to execute the build process.

Note : Inbound rule at 3004 should be allowed , Install Node.js and npm
and Configure NodeJS Plugin in tool configuration in Manage Jenkins



**Problem Statement 2 :**
This problem statement outlines a task to create a Jenkins pipeline that automates the process of
pulling the latest versions of PostgreSQL, Redis, and Mongo Express, as well as MongoDB images
from a public Docker registry. These images are then built into containers locally. Additionally, 
the pipeline should connect the Mongo Express frontend to the MongoDB backend using specific 
access credentials.

Step1 : Pull Images from Public Registry:
The pipeline should use Docker commands to pull the latest versions of the PostgreSQL,
Redis, Mongo Express, and MongoDB images from a public Docker registry (e.g., Docker Hub).

Step2 : Build Images as Containers:
Once the images are pulled, the pipeline should build them into containers locally using 
Docker build commands.

Step3 : Host Images in a Secured Local Registry:
The pipeline should host the built images in a local Docker registry. 
This registry should be secured and accessible using the specified credentials (ati as username and ati1234 as password).

Step4 : Connect Mongo Express Frontend to MongoDB Backend:
The pipeline should set up the Mongo Express frontend to connect to the MongoDB backend
using the specified access credentials (ati as username and ati1234 as password).


Overall, the goal is to automate the process of setting up these services using Docker containers
and Jenkins, ensuring that they are connected and configured correctly.
Jenkinsfile is put under name of **Jenkins_docker**






