# Readings: OAuth

## [OAuth 2 Simplified](https://aaronparecki.com/oauth-2-simplified/)

<!-- ### Author -->

Roles

The Third-Party Application: "Client"
The client is the application that is attempting to get access to the user's account. It needs to get permission from the user before it can do so.

The API: "Resource Server"
The resource server is the API server used to access the user's information.

The Authorization Server
This is the server that presents the interface where the user approves or denies the request. In smaller implementations, this may be the same server as the API server, but larger scale deployments will often build this as a separate component.

The User: "Resource Owner"
The resource owner is the person who is giving access to some portion of their account.

Creating an App

- Redirect URIs

- Client ID and Secret

Authorization
The first step of OAuth 2 is to get authorization from the user. For browser-based or mobile apps, this is usually accomplished by displaying an interface provided by the service to the user.

OAuth 2 provides several "grant types" for different use cases. The grant types defined are:

- Authorization Code for apps running on a web server, browser-based and mobile apps

- Password for logging in with a username and password (only for first-party apps)

- Client credentials for application access without a user present
Implicit was previously recommended for clients without a secret, but has been superseded by using the Authorization Code grant with PKCE.

Web Server Apps

Web server apps are the most common type of application you encounter when dealing with OAuth servers. Web apps are written in a server-side language and run on a server where the source code of the application is not available to the public. This means the application is able to use its client secret when communicating with the authorization server, which can help avoid many attack vectors.

- response_type=code - Indicates that your server expects to receive an authorization code

- client_id - The client ID you received when you first created the application

- redirect_uri - Indicates the URI to return the user to after authorization is complete

- scope - One or more scope values indicating which parts of the user's account you wish to access

- state - A random string generated by your application, which you'll verify later

---


## [Build a Simple REST API with Node and OAuth 2.0](https://developer.okta.com/blog/2018/08/21/build-secure-rest-api-with-node)

JavaScript is used everywhere on the web - nearly every web page will include at least some JavaScript, and even if it doesn’t, your browser probably has some sort of extension that injects bits of JavaScript code on to the page anyway. It’s hard to avoid in 2018.

JavaScript can also be used outside the context of a browser, for anything from hosting a web server to controlling an RC car or running a full-fledged operating system. Sometimes you want a couple of servers to talk to each other, whether on a local network or over the internet.

Today, I’ll show you how to create a REST API using Node.js, and secure it with OAuth 2.0 to prevent unwarranted requests. REST APIs are all over the web, but without the proper tools require a ton of boilerplate code. I’ll show you how to use a couple of amazing tools that make it all a breeze, including Okta to implement the Client Credentials Flow, which securely connects two machines together without the context of a user.

Click the title link to see "Build a RESTful Node API Server
".

---

[Back to Home](https://pdariuslee.github.io/reading-notes/)