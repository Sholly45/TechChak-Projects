## React Frontend Deployment(Roadmap1)
# This shows how the task was completed

I installed node js on my computer, then i cloned the GitHub repo with my vscode, then did an **npm install**, was able to confirm that the app is working well, and then created a production by running **npm build**

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/2.PNG)

When that was confirmed, a build folder was created, which I then copied into an s3 bucket, where i also enabled static website hosting

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/4.PNG)


i then went to Cloudfront to create a distribution and used the SSL certificate I had created

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/5.PNG)

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/6.PNG)

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/7.PNG)

Then I went to route 53 and created a hosted zone. and did a mapping of my route53 zone to my Cloudfront origin as shown below

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/8.PNG)

And i tested the domain and it works as shown below

![1](https://github.com/Sholly45/TechChak-Projects/blob/4461acb62451fd1a880fa1740cdb7489a7d69963/Task-4/images/9.PNG)

