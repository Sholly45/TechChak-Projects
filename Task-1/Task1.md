## Documentation For Task 1: Host Your Static Website Using S3 And Cloudfront
# This shows how the task was completed

I first hosted a static website using s3 and confirmed if it was working as shown below

![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/1.PNG)


Open Cloudfront from the AWS console and create the distribution. Fill out the form as shown below and then create the distribution

![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/2.PNG)
![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/3.PNG)

Copy the policy generated after distribution has been created
![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/4.PNG)


Then go to S3 and go to the bucket where the webapp is hosted and then select edit bucket policy and then paste the policy in there as shown below then save changes
![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/5.PNG)

Go back to Cloudfront and copy the Distribution domain name as shown below and paste in an incognito browser to confirm if it works as shown below

![1](https://github.com/Sholly45/TechChak-Projects/blob/9261cbfd9aca44fd19dc21781b8ef29ee3cb15e1/Task-1/images/7.PNG)
![1](https://github.com/Sholly45/TechChak-Projects/blob/613d891cbd84ece1120af835e6ac05eab84df61c/Task-1/images/6.PNG)











