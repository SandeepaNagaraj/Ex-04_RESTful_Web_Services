# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/d5fa9f5c-85fa-4532-982a-623b6c8fc6ea)



Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 
 
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/8eca6031-2a0f-4839-8339-500fa6041b09)


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/3e6563a9-cafe-4cf6-b4df-570a6aef5721)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/6f869e00-387b-4e99-bd06-61b08a8447d0)
 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/1589c890-d1ad-4205-b4fb-cba7a34ec79b)




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.
Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/4baf5bc0-f699-4880-91ae-46e91bdf838d)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/80510a07-a84e-4a72-ae19-fbe71023bd5f)

Step 6: An editing tab will open. Alter getHtml() method with the following.
 ![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/c14ee72e-6067-4c40-9a68-55f84c1dd2fd)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/d3619df1-5efc-4baa-b5ad-1b3d0bc8c1ef)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/8089342b-1ab3-4f6d-a5ab-605383a3da5e)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/e18bc2b8-b158-43c9-8eea-09d35acdc6a1)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/SandeepaNagaraj/Ex-04_RESTful_Web_Services/assets/113017853/f9232797-9e80-4f8c-9983-c05523bd8ba5)



Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
