# .Net-EfCore-WebApi-IdentitiyServer-TokenBasedAuthentication
I created a project that has a "Token Based Authentication", and also the project includes a SQL Server for saving datas.  You can easily see "How to create a token,refresh token and some identity rules".

# Basic Topics About The Project Structures 

`JWT`

![image](https://user-images.githubusercontent.com/71414017/171815545-c0bfbee0-2086-44f3-b4a1-5c3e6177ab84.png)

--> `Description: `
  JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

`Why we have to use JWT Based Authentication for more security`

![image](https://user-images.githubusercontent.com/71414017/171815642-11ed6971-b640-4220-9515-3b23635f5393.png)

--> `Authorization:` This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

`Information Exchange:` JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.

`Role Based Authorization`
![image](https://user-images.githubusercontent.com/71414017/171926600-73380cc8-2cbd-4948-994f-1c1920b87beb.png)

--> `Description` Role-based authorization enables customer management of users and their roles independently from Payment Feature Services. Role-based authorization has a user registry that is not part of Payment Feature Services. This authorization is optional and does not replace the current model. Customers must select the implementation that best fits their business needs.
