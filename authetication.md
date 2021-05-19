
- Difference between API and Application security 
    - In the case of API, authentication is on User's behalf
    - and in application environment, it is the application who take the credentials from the user and it acting on its on behalf. Basically user's authentication is delegated to application. 

### OAuth 2
- It is called Delegated Authorization Protocal, since User delegates it's access to the application to act on user's behalf.
- Actors
    - Users aka Resource Owner
    - Application aka Client
    - API aka Resource Server
    - Authorization Server

- Bearer Token
    - Carries the security information and user's access information.
    - It flows as Authorization Header in the HTTPS request just as Basic Authorization Headers - Username and Password 

    - JWT - JSON Web Token
        - Essentially a token in JSON format and contains information about user and it's access. It is encoded.
        - it has Header, Payload and Verify Signature
            - Header - contains meta information such as algorithm used
            - Payload - has the user related data
            - Verify Signature - this is used to verify the validity of the token and to make sure it came from the trusted party