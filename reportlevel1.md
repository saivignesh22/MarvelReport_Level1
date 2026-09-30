# CL - Tasks :  
  
## Task 1 : Working with Git and GitHub Basics  
In this task , I learnt a lot about version control system, cloning repositories , conflicts arising when two branches are to be merged, forking, making a pull request(PR) etc.I created and managed branches for feature development, which helped me understand how multiple devs work on a project parallely without affecting the main branch.  
I further learnt more git features such as git revert , git cherry pick , git rebase which increased my knowledge of git and how it helps in efficient managing and tracking of changes in the code.  
I referred to a Youtube channel Apna College to learn all about Git and GitHub and practiced by creating a demo repo and performing all of the above mentioned on my own.  
![img](https://raw.githubusercontent.com/saivignesh22/MarvelReport_Level1/refs/heads/main/gitbash%20branching.jpg)

## Task 2 : Exploring Docker Fundamentals  
This task taught me a lot about docker containers , virtual machines , difference between containers and VM's . I learnt a few important docker commands all of which i implemented practically in the Google Cloud Shell Terminal since virtualization was not possible in my PC .  

<br />

Furthermore I learnt more about images which can be fetched from Docker Hub and how to containerize it, how to manage container lifecycles by starting, stopping, restarting, and removing containers with appropriate Docker commands.    
By this task I understood how docker simplifies software development, testing, and deployment across different environments.   
![img](https://raw.githubusercontent.com/saivignesh22/MarvelReport_Level1/refs/heads/main/docker%20image.jpg)    

## Task 3 : Dockerize a Simple Application
Through this task, I learned how to dockerize and deploy a simple application and as mentioned earlier I did it using Google Cloud Console. 
I created a Dockerfile, built the Docker image, and ran the application as a container within the Google Cloud environment. I also learned how to configure port mapping so that the application could be accessed through a browser. Additionally, I understood how Docker images are built in layers, where each Dockerfile instruction contributes to the final image.   
This task gave me practical hands-on experience with Docker containerization.
![img](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/task3%201%20(1).jpg)
![img2](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/task3%201%20(2).jpg)

## Task 4 : Launch and Manage an AWS EC2 Instance
In this task, I learnt how to launch and manage an AWS EC2 virtual machine, select a suitable instance type, and configure its security group to allow secure SSH access.    
I learned how to connect to the instance using a .pem key and execute commands remotely. I also installed and configured an Nginx web server and accessed the hosted webpage using the EC2 public IP address.   

<br />

Finally, I gained a basic understanding of how CPU, memory, and CPU credits are allocated and utilized in cloud VMs, and how EC2 provides scalable computing resources.  

<br />

btw a huge shoutout for the AWS session on EC2 instance and S3 buckets conducted by the AWS student builder group for a good intro to these topics.
![img](https://raw.github.com/saivignesh22/MarvelReport_Level1/ec72f6921f0f7a1f88df4600f517f768b2be3fa5/ec21.jpg)  

![img2](https://raw.github.com/saivignesh22/MarvelReport_Level1/ec72f6921f0f7a1f88df4600f517f768b2be3fa5/ec22.jpg) 

## Task 5: Kubernetes Basics and Writing Pod Specs

I learned the basics of Kubernetes again by using Google Cloud Console. I understood key Kubernetes concepts such as clusters, nodes, pods, and the control plane, and how they work together to manage containerized applications. 

<br />
  
I created a pod specification using a YAML manifest to deploy an Nginx container and applied it to the Kubernetes environment using kubectl. I also learned how to use commands such as kubectl get pods and kubectl logs to check pod status and troubleshoot application logs. 

<br />

This task gave me practical experience with Kubernetes YAML files, Pod deployment, container management, and monitoring applications in a cloud environment.
![img](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/k8%202.jpg)
![img2](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/k8%201.jpg)

## Task 6: Manage AWS S3 and IAM with CLI
In this task, I learned the fundamentals of AWS IAM, S3 buckets, and the AWS CLI.
- I created an IAM user and assigned appropriate S3 permissions using an IAM policy, gaining an understanding of users, policies, roles, and the principle of least privilege.
- I then configured the AWS CLI with the IAM user's credentials and verified the connection to AWS using the `aws sts get-caller-identity` command.  

This helped me understand how authentication and authorization work when accessing AWS services through the command line.

I created an S3 bucket, created a test file locally, and uploaded it to the bucket using `aws s3 cp`. I verified the uploaded object using `aws s3 ls`, downloaded it back to the local system, and confirmed its contents.    

Finally, I deleted the S3 object and the bucket after completing the exercise. Through this task, I gained practical experience in cloud storage management, IAM based access control, AWS CLI operations, and secure management of AWS resources.  

![img](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/task6a.png)  
![img2](https:raw.//github.com/saivignesh22/MarvelReport_Level1/main/task6d.png)

## Task 7: Deploy a Containerized Application on Kubernetes
I learned how to deploy and manage a containerized application on Kubernetes using Google Cloud Console . I created deployment and service YAML manifests to deploy the dockerized application with multiple replicas and manage its availability.

<br />

I also learnt how to use kubectl to scale deployments up and down, monitor replicas, and understand how Kubernetes performs rolling updates. This task gave me practical experience with Kubernetes deployments, services, scaling, networking, and application management in a cloud environment.
![img](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/task7%20k8%201.jpg)
![img2](https://raw.github.com/saivignesh22/MarvelReport_Level1/main/task7%20k8%202.jpg)  

## Task 8: Use Kubernetes Secrets and Environment Variables
In this task, I learned how Kubernetes manages application configuration and sensitive information using ConfigMaps and Secrets.    
- I created a ConfigMap to store non-sensitive configuration such as the application name and environment. 
- Created a Kubernetes Secret to securely store AWS Access Key ID and Secret Access Key instead of hardcoding them in the application or Deployment configuration. 
- I then created a Kubernetes Deployment and used `configMapKeyRef` and `secretKeyRef` to inject these values into the Pod as environment variables.

- After deploying the application, verified that the ConfigMap and Secret were successfully consumed by the running Pod using `kubectl` commands.
- The IAM user was successfully identified.  
Through this task, I understood the difference between ConfigMaps and Secrets and learned how Kubernetes can provide configuration and sensitive credentials to applications without directly hardcoding them.

![img](https://github.com/saivignesh22/MarvelReport_Level1/blob/main/task8a.png)

## Task 9 : Deploy an App to Push Files from Kubernetes to S3  
- I learned how to integrate Docker, Kubernetes, AWS IAM, Kubernetes Secrets, and Amazon S3 into a complete file-upload application. 
- Developed a simple Flask-based web application that allows users to select and upload files through a web interface. It uses boto3 library to communitcate with S3. 
- I created a Dockerfile and containerized the Flask application along with its required dependencies. I then built the Docker image and deployed it on a minikube Kubernetes cluster using a Deployment.
- Used a Kubernetes Secret to provide the AWS Access Key ID and Secret Access Key to the application as environment variables instead of hardcoding them in the source code.
- A Kubernetes Service was used to expose the Flask application, and port forwarding allowed me to access the application through the browser(sice i was using google cloud console).
-File was selected and uploaded in the application which used boto3 to store the file in configured S3 bucket.
-Verified the same

![img](https://github.com/saivignesh22/MarvelReport_Level1/blob/main/task9a.png)

![img](https://github.com/saivignesh22/MarvelReport_Level1/blob/main/task9b.png)  

# CY - Tasks :  

## A. Fundamentals of Computer Networking (Task 1-5)  : 
In this task, I learnt as the topic says "fundamentals of computer networking".

<br />

- Basically it was about how devices communicate with each other and how a network is just a collection of connected devices that share info and resources.   

<br />  

- Through this task, I learned the difference between private and public networks and how devices are identified using IP and MAC addresses.

<br />

- I also learned the role of ports in networking and studied commonly used ports such as HTTP (80), HTTPS (443) and SSH (22) .  
Data Transmission through packets and frames and the process of encapsulation in the OSI model  was also interesting.  

<br />  

- Additionally, I studied various networking devices including switches, routers, firewalls,  VPNs etc.   
I understood their functions, operating layers, and how they contribute the network communication.  

<br />

This task indeed provided me with a strong foundation in networking concepts, protocols, data transmission, and network security.  

![img](https://media.geeksforgeeks.org/wp-content/uploads/20250726184452563578/frame_25-660.webp)  

## B. Protocols (Task 6-11)  :  

In this task, I learned about several important networking protocols and concepts that are used for communication across computer networks.

<br />

- I learnt about **DNS (Domain Name System)**, which acts like the phonebook of the Internet by converting domain names into IP addresses.

<br />

- I also learned about **DHCP (Dynamic Host Configuration Protocol)** and how it automatically provides devices with network settings. The DORA process (**Discover, Offer, Request, Acknowledge**) showed how devices obtain an IP address without manual configuration.

<br />

- **ICMP (Internet Control Message Protocol)**: ICMP messages are used by tools such as `ping` and `traceroute` to test connectivity, measure network delays, and discover the route packets take across networks.

<br />

- Also how HTTPS uses SSL/TLS encryption to protect data exchanged between clients and servers.   
By inspecting website certificates, I gained insight into how browsers verify the authenticity of websites and establish secure connections.

<br />
This was a very interesting topic :   

- **OSI Model**: The OSI model divides network communication into seven layers. I understood the roles of the Physical, Data Link, Network, Transport, and Application layers, along with concepts such as packets, frames, routing, and encapsulation.

<br />

Overall, this task provided a strong foundation in networking fundamentals and helped me understand how modern computer networks operate.

![OSI Model](https://raw.githubusercontent.com/saivignesh22/MarvelReport_Level1/refs/heads/main/OSI-7-layers.jpg)  

## C. Windows (Task 12-17) : 
This was one of the topic of tasks which was like a realisation for me about how i little i knew about the Operating System present in my device.  

<br />

- Anyways, in these tasks i learnt how powershell is a object oriented command line tool and cmd is text based and how each one of them have their own purposes.  

<br />

- System32 folder which stores critical system files that are essential for the operating system’s functionality and how any modification can break the system and render it unusable.  

 <br />

- It's quite funny but recently i did modify the system32 folder of my PC due to some error .(I used AI to guide me through the process tho ! )  

<br />

- Moreover I learnt about the type of user accounts in windows : administrator and standard. I also learnt how the controls and access is different among both these accounts.  

<br />

Also learnt that Windows includes built-in tools to keep the system safe.

## D. Linux  (Task 18-19) :  

In this task, I learned the basics of the Linux operating system and its importance in modern computing environments. I understood how linux is a  flexible, and open-source OS that is the foundation of many technologies we use daily.

<br />

Linux is widely used in:
- Web servers that host websites and online applications
- Automotive systems and infotainment units
- Traffic management systems and industrial infrastructure

<br />

I also learned that Linux is available in different distributions (distros),  such as **Ubuntu** and **Debian** which are widely used due to their flexibility, and ease of use. 

<br />

The practical part of this task focused on file and directory management in Linux. I learned how to navigate the filesystem and perform common operations using command-line tools.

<br />

In this task I understood the significance of Linux in real world systems.  

## E.  Cryptography :  
This also was a very interesting topic related to the key terms used in the day to day process of cryptography. Also how it is ensures secure communication without any hinders.   

<br />

Some of the keyterms being:  

<br />

- cipher
- ciphertext
- encryption
- decryption
- key etc.

<br />

It also protects the one of the important measure of the CIA triad which is integrity of the data.  
Encryption and it's types were also one of the main focus of this task. Symmetric and Asymmetric encryption whic basically depends on the number and the type of keys.  
![img](https://media.geeksforgeeks.org/wp-content/uploads/20240409125853/Asymmetric-.webp)

## F. Principles of Cybersecurity :   
This topic mainly included about the CIA triad, which is the basic framework on which the security posture of an organization is built upon.   
May it be the NIST CSF or NIST RMF all of these frameworks are based on the CIA triad.
The CIA Triad meaning - 

<br />  

- Confidentiality
- Integrity
- Availability

<br />

These are the three pillars of cybersecurity which any organisation aims to protect and preserve.
![img](https://cdn.prod.website-files.com/6a020fca21245d64af2c19d8/6a020fca21245d64af2c3767_66a372b4a3d814c4fc284041_63fdd44daa2d3e1f527b40e7_CIA%252520Triad.jpeg)
## G. Red Teaming : 
This task gave me a brief idea about what more to explore in this field of security and how Red Teaming which is a part of Offensive Security is one of the path which can be explored more and can be pursued.    

<br />

It gave more details about a few offensive sec terms and also how a person pursuing this field needs to develop a mindset to think like a hacker does and exploit the vulns present in the organisation's security posture.
