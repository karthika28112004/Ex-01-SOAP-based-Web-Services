# Ex-01-SOAP-based-Web-Services

## Aim:

To create and execute SOAP-based web service program using server, client and client- side remote invocation.

## Procedure:

### Server-side:
#### Step 1:
Open NetBeans IDE.
#### Step 2:
Click File->New Project. Choose Java Web and then Web Application and click Next.
![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/a050f285-8941-4e69-9be2-2846977c8d0f)





#### Step 3:
Give your Project a suitable Name and then click Next.
#### Step 4:
In the next window, make sure you have selected Server as “GlassFish Server” and Java EE Version as “Java EE 7 Web”. Click Finish.
![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/d2ed74f8-058b-4ee6-a295-a4238a594a0c)


 


#### Step 5:
Your new project will appear in the Projects tab in the left-most part of NetBeans.

#### Step 6:
Right click your Project and select New->Web-Service.

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/d9cc9111-579f-4234-8490-6bf5794badff)




#### Step 7:
In the new window, give your web service a name and a package name. Click Finish.
 
![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/f4a78d06-8755-4669-8277-099f47b15528)




#### Step 8:
A new coding tab will open that contains your web service.

#### Step 9:
Expand the folder “Web Services” under your project. You should see your newly created web service. Right-click on it and choose “Add Operation”.

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/76b4a986-cea6-4682-a32f-bbc17c9b7cb4)




#### Step 10:
A new window to add operation will appear. In that give Name, Return Type to your operation. Then click the Add button to add necessary arguments/parameters for that
 
operation. (Since we are demonstrating simple addition, we use two arguments/parameters.) Once you are happy with your parameters/arguments, click OK.

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/b86fdcd7-3c8e-4049-abfd-25f3812ec144)



#### Step 11:
NetBeans will automatically generate the skeleton for the operation which will be like,

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/e989a7db-b1e6-4a51-9dea-f42088daa335)




#### Step 12:
. Replace return 0.0 with return (a+b)

#### Step 13:
Save your project. Right-click on the project, select “Clean and Build”. Once the Building process is successful, again Right-click on the project, select “Deploy”.
Deploying might take time depending on the size of the project. 

### Step 14:
Once your project is successfully deployed, right-click on your web service name and select “Test Web Service”
![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/4c570e88-c194-47af-b020-b292e249cb13)


 


#### Step 15:
A new browser window will appear which will look like this

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/3df5bc59-c447-4440-bec0-78290d7fd051)




#### Step 16: 
You can give inputs to your web service and check whether it is working properly or not. If it is working properly, you will get a page like this

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/c537deef-47e9-4803-b42c-37112bc1568e)

 
### Client-side:


#### Step 1:
Create a new Java Web Project in NetBeans. (Follow Steps 1-5 as in section 1.1)
#### Step 2:
Right-click on the project and select New->Web Service Client.

![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/3d62dde3-46f0-44ca-b819-988b75e30cff)




#### Step 3: 
A new window will appear. Select “Project” under the heading “Specify the WSDL file of the Web Service.” and click Browse

#### Step 4: 
A new window will appear, in that carefully choose appropriate web service and click OK.
![image](https://github.com/karthika28112004/Ex-01-SOAP-based-Web-Services/assets/128035087/420c5a28-e912-4f49-888f-f6e90c0d21a4)


 
#### Step 5:
The Project file will be filled with the location to the WSDL file of the web service. If you prefer, you can give a package name. Or else click Finish
 ![c5](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/8bb6e72e-8085-42c6-b88e-db310a49605a)



#### Step 6:
In the Output Window at the bottom of NetBeans, you can notice that the client gathers the operations available in the web service.

#### Step 7:
Once it is done, you should see “BUILD SUCCESSFUL”.

#### Step 8:
Right-click on “Web Pages” under your Project and select “JSP”.

![c8](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/4053beb0-00c4-4f5a-8a7b-7f961b885084)

#### Step 9: 
A new window will appear, give a name to your jsp page and click Finish.

#### Step 10: 
Expand the folder named “Web Service References”-> “Addition” “Addition” “AdditionPort”. Once expanded you should see all the operations available in your web service.

#### Step 11: 
Carefully drag “add” operation and drop it into the JSP page. NetBeans will automatically create the code for invoking this operation which will be like,
 
 ![c11](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/b37ebd64-c3c4-4e9c-9ba4-bf41c6b246bb)



#### Step 12: 
Give values to your arguments and run the JSP file. 

#### Step 13:
A new browser window with the output will appear. 

### Client-Side Remote Invocation

#### Step 1: 
Follow Step 1 and Step 2 as in Client-side (section 1.2).

#### Step 2:
A new window will appear. Select “WSDL URL” under the heading “Specify the WSDL file of the Web Service.” and type the URL of the web service’s WSDL file. (Typically, the URL of the form http://ip:8080/Proj_name/Webservice_name?wsdl)
 

![cr2](https://github.com/DrMalathiSaravanan/Ex-03-SOAP-based-Web-Services/assets/139700114/7d6eb944-5735-40b1-a5fc-7af19d6b92c8)

#### Step 3: 
The remaining procedure is the same as the Client-side.


## Result:
Thus, the SOAP based addition program using Web service is executed successfully.
