# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation

## Procedure:

### Server side:

Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.


![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/6d45ffaa-5b69-4e7c-b6d5-16bc134ea518)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/9d47bd48-7da5-45c7-ab80-de39a8235996)



Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/7cba56d6-942c-46ec-8dcb-6f112ebab4ee)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.


Step 6: Alter getHtml() method as shown below.


Step 7: Save your project, clean and build it. Deploy your project.
 

 ![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/1130e1a7-457c-4ad2-90e1-2d9a9c8caf79)



Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/2aaf2813-b9bb-45f0-ad39-3a7f34a25fc9)



Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 

Step 4: Carefully select your RESTful resource (web service) and click OK.

![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/2beef9c8-f8ff-437a-9000-ed9315862722)


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.


![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/3b185691-374a-471e-b307-41cdeb362883)



Step 6: An editing tab will open. Alter getHtml() method with the following.
 

![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/126a100d-b53b-4173-8854-31145c9e6c83)

 

Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.


![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/c2155322-3575-444e-b9fb-cd6c1f2ca72b)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.



 ![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/0c2df78f-f9de-4b8f-848b-417894a4879a)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.


![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/468c9acd-a75f-4047-b807-c49b37771b87)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 
![image](https://github.com/Vijayalakshmi230/Ex-04_RESTful_Web_Services/assets/127175503/af5426ce-3ae2-4285-8286-a9e96f2e0cb8)



Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2

Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";


Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
