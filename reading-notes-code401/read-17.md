# Read-17, Code 401, 19 April 2021

## AWS: S3 and Lambda

## Vocabulary

- Server Instances
  A server instance is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

- Containers
  A web container (also known as a servlet container; and compare "webcontainer") is the component of a web server that interacts with Jakarta Servlets. ... The Web container creates servlet instances, loads and unloads servlets, creates and manages request and response objects, and performs other servlet-management tasks.

- Cloud Services
  Cloud services are services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

- Cloud Architecuture
  Cloud Architecture refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. Cloud architecture defines the components as well as the relationships between them.

- AWS
  is a secure cloud services platform, offering compute power, database storage, content delivery and other functionality to help businesses scale and grow. In simple words AWS allows you to do the following things- Running web and application servers in the cloud to host dynamic websites.

- EC2/Beanstalk vs Heroku
  Heroku is best suitable for Startups, Medium Businesses whereas AWS is mainly focused on Medium Businesses and Large Enterprises. Heroku can meet low computational demands whereas AWS can meet high/very high computational demands. Heroku doesn't needs infrastructure maintenance whereas AWS needs a dedicated DevOps guy.

### Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   AWS and how to use it, BeanStalk, EC2

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   I'm hoping to implement what I learn for AWS by my Own.

3. What are you most excited about trying to implement or see how it works?
   Using the AWS/EC2 Beanstalk to deploy my Database and a full website

### Preperation Material

- AWS S3
  Amazon Simple Storage Service (Amazon S3) is storage for the internet. You can use Amazon S3 to store and retrieve any amount of data at any time, from anywhere on the web. You can accomplish these tasks using the AWS Management Console, which is a simple and intuitive web interface.
  ![AWSS3](https://lh5.googleusercontent.com/KGIHx2ypgtGDRx0QDl4htQy33B4i-fVs8y75So28yDYk4dJ65iPTM67aU9Jh-m05Yr1tCXdzdrrq8g8pvvgjpgPwoNvCjorm55h9BL2AdW5B9YqiefIa410HGjAPoNPsAvdftW6X)
  Database backup is an important operation to consider for any database system. Taking backups not only allows restoring upon database failures but also recovering from data corruption. However, storing a backup in durable and reliable storage can be expensive. Cloud services like AWS S3 provide highly durable and reliable storage for database backups while reducing costs with archival facilities using AWS Glacier.

- AWS Lambda
  AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

  The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

  The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. And so “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

- CDN
  ![cdn](https://stokewebdesign.co.uk/wp-content/uploads/2020/02/cdn-edge-server-768x480.png)

  Content Distribution Network (CDN) is now available to new and existing customers with all our hosting packages.
  CDN provides your websites with a performance boost wherever your users are in the world. With increased loading times that benefits your website with dynamic caching; providing full control over the duration of caching of images, Javascript and CSS.

  As well as edge-caching it includes a comprehensive website speed optimisation suite. Through tools like image compression and code minification, it can drastically speed-up a website. We will determine which settings are suited best for your website based upon the platform used and whether fresh content is added frequently.

[GitHub-link](https://omar-tarawneh.github.io/reading-notes/reading-notes-code401/read-17)
