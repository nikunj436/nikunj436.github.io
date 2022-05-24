
# py_aws mini-project overview (flask web framwork with mongodb)
## - Nikunj Rabadiya | [Linkedin](http://www.linkedin.com/in/nikunj-rabadiya)
###  - aws EKS (Kubernetes), Docker, Docker-Compose, Jenkins Pipeline (declarative syntax Jenkinsfile)  

- git repo: - https://github.com/nikunj436/py_aws or [click here](https://github.com/nikunj436/py_aws)
- aws EKS cluster webapp link:- https://bit.ly/3zbGOrx or [click here](https://bit.ly/3zbGOrx)
- Deleting Eks cluster soon cause it incurs charges


# Let's go backwards with project (as it created) .

## Jenkins Pipeline

- amazon Ec2 ubuntu instance created with addition port 8080(Jenkins default port).
- dependencies installed -> openjdk 11, docker, jenkins.
- sudo su - jenkins 
- aws cli, ekctl(v 1.21 used), cluster config file fetched. 
- Jenkinsfile declarative syntax used. Please check my repo.
- see below snapshot how "stage area" actually turns out. 

<p>&nbsp;</p>
 <img width="500" alt="image" src="https://user-images.githubusercontent.com/87404299/170044918-c17bdce4-8f4f-4efa-bd5d-b71325107bfc.png">
 <img width="500" alt="image" src="https://user-images.githubusercontent.com/87404299/170036222-8c8f19e4-9f28-47f5-947b-52f8e508259e.png">
<p>&nbsp;</p>
 <img width="500" alt="image" src="https://user-images.githubusercontent.com/87404299/170039383-b24cd852-db94-4f6b-ab9a-26155cd3c0c3.png">
<p>&nbsp;</p>
 <img width="500" alt="Screenshot 2022-05-24 183029" src="https://user-images.githubusercontent.com/87404299/170041075-ad2a3948-8d20-48df-b9b6-70e5987737a1.png">
<p>&nbsp;</p>
- above snapshot - Rolling update:- one by one new pod is being created and old pod is being deleted 


## Amazon EKS (using console)
- dependencies:- node group(4 worker node t3.micro), respective IAM, vpc, root or administration(user).
- local machine:- installed:- aws cli, ekctl(v1.21 used).
<p>&nbsp;</p>
<img width="500" alt="image" src="https://user-images.githubusercontent.com/87404299/170044395-3995b892-78d1-4f6e-95c2-1b46327e0f38.png">
<img width="500" alt="image" src="https://user-images.githubusercontent.com/87404299/170044312-c2480aad-dba0-477b-ba1f-85f55452fd3a.png">
<p>&nbsp;</p>

## k8s, Dockerfile, Docker-compose yaml files
- please find a k8s folder for kubernetes yaml files in my repo.
- Dockerfile used to containerization and pushed to docker hub so it can act as k8s webapp deployment image.
- Docker-compose only used on my local machine for sack of completion.

## web app overview
- mondodb used for database.
- a simple flask web-form accepting name and it's get stored in mongodb database.
- Please find below snapshots.

<p>&nbsp;</p>
<img width="443" alt="image" src="https://user-images.githubusercontent.com/87404299/170046631-d7ef7344-6e47-4e3e-a000-9bb69981195b.png">
<p>&nbsp;</p>
<img width="442" alt="image" src="https://user-images.githubusercontent.com/87404299/170046692-c563346d-5f6d-435e-80d1-a263e9340c6b.png">
<p>&nbsp;</p>
<img width="443" alt="image" src="https://user-images.githubusercontent.com/87404299/170046762-9b1785fc-ec96-41d4-a351-93aa8360613d.png">
<p>&nbsp;</p>
