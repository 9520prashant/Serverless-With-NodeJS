## Serverless Framework With NodeJS

### Serverless.yml configuration breakdown

* Name of the Service.

    ```bash
      service: serverless-api-http
    ```

* Framework Version.

    ```bash
      frameworkVersion: '3'
    ```

* Provider and Runtime Name.

    ```bash
        provider:
            name: aws
            runtime: nodejs18.x
    ```
* Functions that will run on Cloud.

    ```bash
        function:
            serverless-api-http:
            handler: Hello.handler
            event: 
            - httpAPI
              path: /
              method: get
    ```
    
In the above code, handler is a function named `Hello.handler` to execute when a request is made to the root `path /` on `get` method, and API gateway is HTTP.
     
