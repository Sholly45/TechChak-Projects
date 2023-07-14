## Backend End-End Infrastructure
# This shows how the task was completed

I created a custom vpc which I called backend vpc (where I created two security groups called ‘ec2 security group’ which had port 22 and my local ip open and ‘load balancer security group’ which has my http and https ports open) The vpc has 2 private and 2 public subnets attached to it as well. 

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/1.png)
![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/2.png)

I then launched an ec2 instance in the newly formed vpc attached to the ec2 security group
![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/3.png)

I ssh into my instance and installed all node dependencies and confirmed by running the commands as shown on the screenshot below: 
![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/4.png)

I the cloned the application and entered the directory, then installed PM2 by running the command **‘sudo npm install pm2@latest -g’** Ran the command pm2 start server.js to start the application.

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/5.png)


It then generated the start-up script which I ran 

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/6.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/7.png)

After the command ran successfully, I then started the server using the: **`pm2 start server.js’**

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/8.png)

 I then ran the command **‘npm run dev’’** to start the application

 ![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/9.png)

 I then went to my ec2 instance and copied the ip address to the if the application is working fine which can be seen as shown in the screenshot below.

 ![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/10.png)

 I went to the load balancer section of my aws to create a target group in which I point the instance to the load balancers; and selected the HTTP protocol and allowed port 5000. I selected the backend vpc and configured the http to port 5000, and then created the target group

 ![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/12.png)

 I then went to my aws console to configure my load balancer, by selecting the application load balancer, and configuring the load balancer by filling in the parameters as shown in the screenshot below, please note the vpc section must include the custom vpc(backend vpc) created and the load balancer sg in the security group section. Then attach the target group created in the above step and then create.

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/13.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/14.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/16.png)


I then went to test my load balancers and the api and as shown below can be confirmed everything is working fine

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/17.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/18.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/b68d203cdb85873915e0a6e0c85ac41cda9a547b/Task-5/images/19.png)

 

 




