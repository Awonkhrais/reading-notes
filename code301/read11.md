# Readings: Authentication

## What is OAuth


1.What is OAuth?
* OAUTH allows websites and services to share assets among users.
* Open-standard authorization protocol or framework.

2.Give an example of what using OAuth would look like.

* An example of OAuth being utilized is when you visit a website, and it gives you the option to sign into their system using your other accoundts they can link the services logon with.

* Like using your Google or GitHub account to login to a site

3.How does OAuth work? What are the steps that it takes to authenticate the user?

* firstly, the first website will connect to the second website on the users behalf using OAuth.

* the second web site will generate some kind of one-time-token and a one-time-secret token to the involved parties of this entire transaction.

* the first page will take the secret and regular token to the client.

* the client will present the two tokens to the provider.

* If there is authentication required, the client will ask the provider for authentication to approve the transaction to the second site.

* then the user approves.
* The user is given approved access tokens.
* then the user will give those tokens to the first web site.
* then the access tokens will be taken to the second web site.
* the second website will allow the first website access.
* the user can see the transaction occuring.

![OAuth](https://dzf8vqv24eqhg.cloudfront.net/userfiles/866/14262/ckfinder/images/2020_03_10_09_00_551.png)

4.What is OpenID?
* OpenID is a way for humans to log into machines. OpenID is an authenticator and not a authorizor.

(is similar except it is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.)

## Authorization and Authentication flows

![Authentication](https://s3.ap-south-1.amazonaws.com/afteracademy-server-uploads/authentication-vs-authorization-diff-a7acc34e88679381.png)

1.What is the difference between authorization and authentication?

**The difference between authorization and authentication, can be simplified by determiing who are what is logging into another service or device. For instance, when humans log into the computer, the computer will ask for a password or something letting the computer know that it is you that is logging in. So the computer needs authentication in order for the user to access the computer. From there, if the user wants to access a service, lets say a web page of some sort. From there the user will be able to log in with OAuth which the comoputer will try to log into other services on the users behalf. So it is like the computer logging in to another service. For the computers to achieve this, they will require authorization.**

2.What is Authorization Code Flow?
* Authorization code flow is the exchange of code for tokens.

![](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)

3.What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

* used when mobile and native applications require additional security

![](https://images.ctfassets.net/cdy7uua7fh8z/3pstjSYx3YNSiJQnwKZvm5/33c941faf2e0c434a9ab1f0f3a06e13a/auth-sequence-auth-code-pkce.png)

4.What is Implicit Flow with Form Post?

* Implicit Flow is an alternative method for fetching the required tokens for access. This method will prevent the need to worry about "securely storing client secrets."

5.What is Client Credentials Flow?

* services running in the backend and authenticatng and authorizing the app rather than the user can sometimes pose a problem. To allieviate this, you can use the Client Credentials Flow.

6.What is Device Authorization Flow?

* Alternative for authenticate, where the device asks the user to go to a link on their computer or smartphone and authorize the device, in which they pass along their Client ID to initiate the authorization process and get a token.

7.What is Resource Owner Password Flow?

* Used by highly-trusted applications, which requests that users provide credentials (username and password), typically using an interactive form.