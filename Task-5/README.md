# Backend End-End Infrastructure
**Project Task**: Congratulations on the successful deployment of the static front-end app via CloudFront. The management is extremely impressed by your hard work and dedication to our infrastructure. As you already know, the react static web app you deployed is just a front-end application and it does not have any backend interaction yet so that the list of available cars can be fetched into the front. Our users can’t use it yet because we don’t have a backend infrastructure in place to interact with via API. The good news is that our backend engineers have completed the backend effort which is written in node js and they have tested it locally. Everything seems to be working fine and the app is ready for deployment into our AWS infrastructure. Before I suggest the approach to setting up the backend architecture, I want you to take a look at the architecture below which represents what you will be helping the team to build as a POC.

Note that we are using Mongo DB, a NoSQL DB outside of our AWS infrastructure, so we do not have to worry about provisioning a database. The credentials to connect to it will be available in the env file of our NodeJs APP (In the ideal world, we will not have credentials in the app, we would rather have it in AWS secret and call it when running our APP)

The backend application has been pushed into this Gitlab repo

https://github.com/techchak/techchak-dealership-backend-app.git
