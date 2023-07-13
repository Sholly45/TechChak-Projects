## Run A React App On AWS Cloud9 From Scratch
# This shows how the task was completed

Log on to the AWS Console and Search Cloud9  from services and then create an environment

![1](https://github.com/Sholly45/TechChak-Projects/blob/e10f0be30ee88dabdb067df8ce55a978a0fe7a4e/Task-3/images/1.png)
![1](https://github.com/Sholly45/TechChak-Projects/blob/e10f0be30ee88dabdb067df8ce55a978a0fe7a4e/Task-3/images/2.png)

Give the environment a name,
Select “New Ec2 Instance” for Environment type,
Instance Type leave as default,
Platform: Select Ubuntu,
Connection Select Leave as default
Then Create


![1](https://github.com/Sholly45/TechChak-Projects/blob/e10f0be30ee88dabdb067df8ce55a978a0fe7a4e/Task-3/images/3.png)

![1](https://github.com/Sholly45/TechChak-Projects/blob/e10f0be30ee88dabdb067df8ce55a978a0fe7a4e/Task-3/images/4.png)

After creation, i selected open and then cloned the repo and switched directory to the cloned repo and the installed the dependencies

**`sudo apt-get install nodejs`**

**`npm install --force`**

**`sudo apt update`**

**`npm start`**

copy the ‘on your network url’ shown on to your browser

![1](https://github.com/Sholly45/TechChak-Projects/blob/e10f0be30ee88dabdb067df8ce55a978a0fe7a4e/Task-3/images/7.png)

Go to your ec2 instance and then select security groups, then go to the inbound rules, and open all ports, then reload the browser

![1](https://github.com/Sholly45/TechChak-Projects/blob/58ef9437c752ae8fa9c6f53eb3d1fefa8948f04c/Task-3/images/8.png)

Then refresh the page, then you would see the App has been successfully deployed

![1](https://github.com/Sholly45/TechChak-Projects/blob/58ef9437c752ae8fa9c6f53eb3d1fefa8948f04c/Task-3/images/10.png)















