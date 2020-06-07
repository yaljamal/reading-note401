# OAuth
* OAUTH2.0
> it is the login using any provider like (github , facebook , google account )
When you “Login with Google”, you’ve actually given the application (or website) the keys to some of your personal information and access levels at Google.

# How does OAuth work?

1. Application spawns the “Login Using xxx” window, asking for specific permissions
2. User Agrees to allow this to happen
3. Remote service (i.e. Google) contacts the application with a one-time-use *Code*
4. The application calls back to a special address on the remote service to exchange that *Code* for a *Token*
5. Once the *token* has been granted, the application will then be able to contact the remote service, using that *Token* to access information on behalf of the user
The *token* is the user

# Access Code

First the client needs to grant the application permission. To do this you need to provide an <a> tag that will take them to the service’s authorization page. This <a> tag should pass the following information through a query string to the authorization server. Every service is slightly different in their specific requirements, but in some form or another, variables like these are part of this initial request

* `response_type=code` indicates that your server wants to receive an authorization code
* `client_id=<your client id>` tells the authorization server which app the user is granting access to
* `redirect_uri=<your redirect uri>` tells the auth server which server endpoint to redirect to
* `scope=<list of scopes>` tells the auth server what you want the user to give access to
* `state=<anything you want>` a place where you can store info to pass to your server if you want

# Access Token
If the users grants access to the application, the authorization server will redirect to a provided redirect URI callback with a “code”. Once you have this code, you can exchange it for an access token by making a POST request to the authorization server and providing the following information:

- `grant_type=authorization_code`
- `code=<the code your received`
- `redirect_uri=REDIRECT_URI` must be same as the redirect URI your client provided
- `client_id=<your client id>` tells the authorization server which application is making the requests

- `client_secret=<your client secret>` authenticates that the application making the request is the application registered with the client_id

- Once you get an access token, you can use it to make API calls to the service on behalf of that user
