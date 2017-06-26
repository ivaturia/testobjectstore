Steps to download "ObjectStore":
- Go to Help --> Install New Software --> Select "--All Available Sites--" and search for "ObjectStore".
- Install the connector.

Download the project and run the project in the Anypoint Studio.

This project runs on port 8081 and here are the APIs supported:
- http://localhost:8081/users/ loads the object store with the key value pairs and displays in json format
- http://localhost:8081/users/{userId} retrieves the value for key userId from object store
- http://localhost:8081/users/delete/{userId} deletes the key from the object store if the key exists based on the userId parameter.

Example requests to test the application:
http://localhost:8081/users/
http://localhost:8081/users/111
http://localhost:8081/users/444
http://localhost:8081/users/555
http://localhost:8081/users/delete/111
http://localhost:8081/users/delete/444

Instructions to deploy it in the cloudhub:
- Right click on the project and select "Anypoint Platform" --> Deploy to cloud.
- A pop up will be displayed for entering Anypoint Platform credentials and deploy the application.