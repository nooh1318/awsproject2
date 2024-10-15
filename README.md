# awsproject2
Architechture of Image recognition using aws

![awsproject ](https://github.com/user-attachments/assets/d18a5487-2ee7-4250-a2bc-6314e102b5ab)

Project Overview:
leveraging Amazon Rekognition to perform image recognition on images stored in Amazon S3. The project involves several AWS services working together to automate the process of analyzing and identifying objects, scenes, and activities within the images.

Key Components in the Architecture:

Res User Light:

Represents the end-user who interacts with the system, potentially uploading images for recognition.

Amazon EC2 (Elastic Compute Cloud):

This is the virtual machine where your application is hosted, possibly interacting with other AWS services like Rekognition. It is accessed through AWS Cloud9, which is a cloud-based IDE used for developing and running code.
Amazon S3 (Simple Storage Service):

The images to be analyzed by Rekognition are stored in an S3 bucket. This scalable storage service is used to store, retrieve, and manage image files securely.

Amazon Rekognition:

This is the main service used for the image recognition task. It processes the images stored in S3, detects objects, scenes, faces, and provides labels for these images based on machine learning algorithms.
IAM (Identity and Access Management):

IAM manages roles and permissions. In this project, IAM ensures that the EC2 instance, Rekognition, and S3 interact securely. It controls access to AWS resources like S3 and Rekognition.

Cloud9:

AWS Cloud9 is used to manage and execute code in a cloud-based development environment. It provides access to the EC2 instance where you develop and run the code for this project.

Workflow:
The end-user uploads an image, which is stored in an S3 bucket.
Your EC2 instance, hosted through Cloud9, processes requests and uses the Rekognition service to detect and label the contents of the image.
IAM ensures that your EC2 instance has the necessary permissions to access Rekognition and S3 for reading and writing image data.
The Rekognition service performs image analysis and returns the results (such as detected objects or scenes) to the application running on EC2.
The processed data or labels can then be displayed to the user or stored for further use.

Summary:
This architecture efficiently handles image recognition tasks by using a combination of AWS services. It allows users to upload images, processes them in the cloud, and provides results using machine learning through Amazon Rekognition. The use of IAM ensures secure interactions between the different services.

Input image given is :

![myimage](https://github.com/user-attachments/assets/b617b739-3790-4c0b-8c10-f7985298af9b)




