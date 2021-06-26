
# MsFit-sa Anaylsis

### Observations 
1. Hosting Methodology seen on AWS only one website which is not related to msFit-sa , No instances running currently on Ohio , but it is totally insurced and no priviliges that protecting the project Assests ..

2. The whole videos are rendered from youtube which is publicly accessable 

3. The web is not secured by SSL connection inspected on IOS and expecting the same on Android .. 

4. the s3 bucket is directly accessable through internet "different site !!!!!!! "

5. payment is not secured with SSL , it depends on Apple Pay APIs 

6. a lot of UI glitches ..

7. it seems that the app hosted somewhere else than AWS in the moment of inspection 25-06-2021 

8. Recommended to host on Vemo or Secure the youtube public links 

### Purposed Arhcitecture 

![alt MSFit-SA Architecture](https://github.com/AliAhmedNada/msfitReview/blob/main/AWSServices.png)

#### This is Phase 1 for the Arhcitecture required based on the small chunch of info we have currently 

###### 1st we have cognito as Authorizeration and Authentication fedration to register and to have user Rigid Authentication methodolgy 
###### 2nd we have CloudFront as this is a static website to render the views on Mobile IOS and Android Much more faster 
###### 3rd route53 to configure domain to use it within cloud front to be an alias 
###### 4th RDS read replica to make sure that we will never have loads within reads while writing data 
###### 5th finally lambda to manage the read write data Operations with RDS 

This Architecture is Subjected to change according to the Information we are going to digesit 



Created by : 
Ali Nada

