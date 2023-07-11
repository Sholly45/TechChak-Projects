## Documentation For Task 2: Create An Alias Record In Amazon Route53
# This shows how the task was completed

 I uploaded the website assets in an s3 bucket in the north Virginia region and enables static website hosting. I then got the s3 endpoint as shown below

  ![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/11.PNG)
  ![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/2.PNG)

I got my domain name name, then used Cloudfront and created a distribution for my s3 buckets endpoints, i filled in the details of the s3, left the rest as default, however in the security section as shown below I generated a certificate using aws certificate manager which will then be used for the CloudFront distribution below 

![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/3.PNG)

Proceed to route 53 and create a hosted zone, input the domain and leave rest as blank and save 

![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/4.PNG)

Then create a record using the wizard to create a simple record, set the alias and select route traffic to alias to cloudfront distribution as shown below, then input your cloudfront distribution “domain name“ and create records.
![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/5.PNG)
 

After filling in all the parameters as shown above test your configurations by copying your new domain and paste on your browser.
![1](https://github.com/Sholly45/TechChak-Projects/blob/9b32a24c9afe0e444de6c3ac86f264ee6a2f2a8f/Task-2/images/6.PNG)
