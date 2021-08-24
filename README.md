## Running the application locally
        
1. Run the application using an embedded Tomcat:

	    $ mvn clean package
	    $ mvn cargo:run
	    
2. You can then access the bank application here: http://localhost:8080/insecure-bank/

## Running with Docker

Run the insecure-bank application with Docker.

Place Hdiv agent and license in the application root folder.

        $ docker build -t insecure-bank .
        $ docker run -p 8080:8080 -d --name insecure-bank-app insecure-bank
        $ docker logs insecure-bank-app

Open the application in > http://localhost:8080/insecure-bank        

## Login credentials
- Username: john
- Password: test
