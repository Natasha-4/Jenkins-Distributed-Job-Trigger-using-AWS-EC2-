# Jenkins-Distributed-Job-Trigger-using-AWS-EC2
Overview: This project demonstrates how to set up two Jenkins servers on AWS EC2 where one Jenkins server (Controller) triggers a build on another Jenkins server (Remote Server). The controller triggers the remote job using the Jenkins REST API and curl command.

Architecture:
EC2 Instance 1 → Jenkins Controller -EC2 Instance 2 → Remote Jenkins Server

Steps:
1. Launch two EC2 instances on AWS. 
2. Install Java and Jenkins on both servers.
3. Create a Jenkins job on the Remote Server. 
4. Enable "Trigger builds remotely" and add a token.
5. Test the trigger using the Jenkins API URL.
6. Create a job on the Controller Jenkins.
7. Add a curl command to trigger the remote job.

Result: The controller Jenkins server successfully triggers builds on the remote Jenkins server, demonstrating basic distributed CI/CD automation using Jenkins and AWS.
