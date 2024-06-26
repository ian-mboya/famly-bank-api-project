<h1>Interacting with the API</h1>
<p> FastAPI offers a simplified way of interacting with APIs via SwaggerUI. This is a rich web page with features that make testing out APIs built on FastAPI much simpler.<p>

<h2> Getting Started <h2>
<p> Ensure that your server is running on this address "http://127.0.0.1:8000"</p>
<br>
<p> To use SwaggerUI just add /docs to the the url in the address bar. "http://127.0.0.1:8000/docs"</p>
<br>
This is what you should see in your web browser.
  
![image](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/0ca2d4db-0a21-4318-96f0-c39b63b4fc28)


As mentioned, FastAPI's SwaggerUI provides a friendly interface to API developers. As we can see, it is able to identify our API endpoints and Schema. 

<h2>Making POST request</h2>
<p>1. We have our database created in Postgres. We are going to make a POST request that has the following request body that sends the particular fee details to our database.</p>


![image](https://github.com/ian-mboya/family-bank-api-project/blob/main/assets/POST%20request%20empty.png?raw=true)

<p>2. These are our values that we need appended onto our database.</p>

![image](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/d09a0a1c-3f17-4f5c-ae1d-d539d927b701)


<p>3. After pressing execute, we should see the following 200 success code showing that the data has been successfully been sent to the database </p>

![image](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/8b4e9463-f727-4cc0-a763-44c53322bd7a)



<p>4. Here is the updated value in our database.
<p>Before</p>

![Database unapdated](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/60efec03-45cd-4250-9b1c-d5b6fdbc7004)

<p>After</p>

![database updated](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/57b5d880-c986-4bc7-88a1-ac1c7b1c2870)


We have covered making POST requests in our API.


<h2> Making GET requests </h2>
<p>We have two endpoints that allow us to get a single student's payment history via student id and another one that is able to query all students' payment history</p>


<p>1.  We will begin by getting a single student's payment history. Here we will enter the student's ID in the previous demo
</p>

![GET request by id 1](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/45b99d8b-d931-45ee-8c98-026289bd2c79)

<p>2. Here is the response</p>

![GET request 1 by id response](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/2b7d7568-9d08-4fab-873b-de52a6be2117)


<p>3. A student may have conducted a number of transactions. We will use an example of such a student in our database</p>

![GET by ID multiple](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/ca576bce-ae2e-48b4-b7b9-2b4a9af4a3a3)

<p>This is the response with the student's entire transaction history</p>

![image](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/090f5e3d-0bcf-4657-a2e0-0e9a9f01afbb)

<p>To get the entire history for all students we will just enter the URL "http://127.0.0.1:8000/statements/". But here is how we do it in the UI</p>

![GET statements all](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/5b41486e-ba65-4c22-90b1-6763864521e8)

<p>Response</p>

![GET statements all response](https://github.com/ian-mboya/family-bank-api-project/assets/68651784/61229671-beac-4d96-a0a2-651895014104)


We have successfully demonstrated that our API is working







