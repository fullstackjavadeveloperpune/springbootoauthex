# springbootoauthex
Spring Boot OAuth 2.0 Implementation

OAuth 2.0, which stands for “Open Authorization”, is a standard designed to allow a website or application to access resources hosted by other web apps on behalf of a user.


Steps for OAuth 2.0-
1. Google Console
2. API & Services
3. Credentials
4. Create OAuth client ID
5. Select as Web Application
6. Give Application Name
7. URI's- http://localhost:8080
8. Redirect URI's- http://localhost:8080/login/oauth2/code/google
9. Click on Create
10. Copy the Client ID and Secrete then add those in Spring Boot Application YAML File
11. Run & Test your Spring  Boot Application

---------------------------------------------------------------------------------------------------

Please use below content in appliaction.yaml file-

spring:
  security:
    oauth2:
      client:
        registration:
          google :
            clientId: your_client_id
            clientSecret: your_client_secret
