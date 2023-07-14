![1](https://github.com/Sholly45/TechChak-Projects/blob/1bcdd5a3ec184789437871354e204a18c9111e91/Task-4/images/1.png)

# React Frontend Deployment(Roadmap1)
**Project Task**: Welcome on board and I am thrilled to have you on our team. As you already know, we are a Car dealership company. We currently have a team of developers working on our web application. (Both the front and back ends). Our backend is built in nodejs, and our frontend is built in REACTJS. The preferred deployment mode is to deploy the front end (REACT) as a static website hosted in S3 and served to our users via CloudFront. Once this is achieved, the management wants you to get a registered domain name from AWS Route 53 or any other provider like GoDaddy, once this has been accomplished. Next, configure route53 or the domain name provider of your choice to direct traffic to the CloudFront distribution where our static website is hosted. In the end, users should be able to access our static website when they visit the domain.

Also as an additional measure to provide lower-latency data access in another region, I recommend configuring a cross-region bucket replication for the s3 bucket.

Keep in mind we still have the backend architecture to set up (We will address this in the next milestone). 

Below is the Architecture provided by the lead engineer for the front-end static app

Understand that this is just the front-end and when the app is spun up, we might not see lists of cars for sale because we have not set up the backend app yet. This backend app will be set up in the next project and will be responsible for helping us fetch data from a database into the front end of our app. We can't even log in yet because there is no backend to validate our credentials 

The react Static website code is stored in this repository 

**https://github.com/techchak/techchak-dealership-frontend-app**

Feel free to clone this repo to your local machine so you can upload the code into the s3 bucket.

Here is a wiki on how to clone a repo into your local machine
