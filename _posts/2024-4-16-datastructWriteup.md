---
layouts: base
title: Data Struct Writeup
comments: true
description: Data Struct Writeup
type: tangibles
courses: { compsci: {week: 14} }
---

<style>

</style>
## From the [MiraCosta CS113 course catalog](https://catalog.miracosta.edu/disciplines/computerscience/#courseinventory)

Students explore the software development process by developing effective solutions using industry-standard tools. Topics include searching, sorting, hashing, algorithm analysis, object-oriented design, collections, lists, stacks, queues, trees, sets, dictionaries, and graphs.

- Map the below elements from MiraCosta course description using your CPT project.
  
  - This must be unique to your portion of the integrated project.
  - This is a pre-requisite prior to answering the college board questions that have been posted to AP Classroom.

### Collections
Blog Python Model code and SQLite Database.

- From VSCode using SQLite3 Editor, show your unique collection/table in database, display rows and columns in the table of the SQLite database.
- From VSCode model, show your unique code that was created to initialize table and create test data.

- <img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/4ade91d3-0a8e-413d-b67c-11b9eb97b208'>
- User function that constructs the columns and attributes for each of the users. Notice at the top of the screenshot all of the columns are being created.

- <img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/28060884-3391-4b3c-801d-1a83b2d3ec7e'>

- Initialization for the user database, inputting values for each of their attributes to generate the data.

- **Initialized Data**

<img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/e005d500-acd9-491a-b99e-69ed049b75d5'>
> Initialized SQLite User database. Unique columns that stores user's points and items. Integrated from our LMC CPT Project, so that whenever a user watches videos they can obtain points and buy items from the shop page from our LMC CPT. 

### Lists and Dictionaries
Blog Python API code and use of List and Dictionaries.

- In VSCode using Debugger, show a list as extracted from database as Python objects.

<img src="https://github.com/trevorhuang1/csp_blog/assets/118785933/419fdd13-e644-40bd-ba83-05c1e274641b">
- At the stage where the JSON data is being prepared for the GET request output. In the debugger, each user object can be viewed in the debugger with their associated values.

- In VSCode use Debugger and list,  show two distinct example examples of  dictionaries, show Keys/Values using debugger.

    <img src="https://github.com/trevorhuang1/csp_blog/assets/118785933/b1230c3c-88f4-41c7-85d2-fe062595a8ce">
- At this portion of the code, each user has a dictionary to store each of their attributes or values, including uid and password. When checking if the user exists via their uid dictionary value, they are assigned a JWT token for authentication purposes.
### APIs and JSON
Blog Python API code and use of Postman to request and respond with JSON.

- In VSCode, show Python API code definition for request and response using GET, POST, UPDATE methods.  Discuss algorithmic condition used to direct request to appropriate Python method based on request method.
- In Postman, show the JSON response data for 200 success conditions on GET, POST, and UPDATE methods.

- **GET**

<img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/31155b64-18e3-4d76-9e2e-33552228734a'>
- GET request to retrieve user data from the database

- **PUT Request(Update)**

<img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/7f1187ee-3437-47b3-9d48-eab876d5d8a5'>
- PUT request to update user values. Specifically, in our project which is a game we use it to update the user's points and current items.

- In VSCode, show algorithmic conditions used to validate data on a POST condition.

- **POST**

<img src='https://github.com/M8tth3/m8th3_2.0/assets/64436503/b40ea976-2181-4b4a-8424-ba2773a5ddee'>
- Security POST request which creates a JWT Token for the user 
- In Postman, show URL request and Body requirements for GET, POST, and UPDATE methods.


- **POST**

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/a5fd7961-e0bc-4d63-bc92-d10dc185e44d">
- This POST request is for authentication and after providing the body shown above, it will run it through the SECURITY POST request and if the UID is found in the database, the user will be given a JWT token which is stored in the form of a cookie.

- **GET**

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/26a2e034-e647-46ee-969e-6d3e0a49911c">
- GET request to retrieve user data after authentication

- **UPDATE(PUT)**

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/9efa7aa7-06fb-4925-8921-755e89655145">
- After providing the values that you want the user to have. The PUT request searches for the UID provided in the database and replaces the user's values with the ones provided in the PUT request.

- In Postman, show the JSON response for error for 400 when missing body on a POST request.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/ae0cc745-7a69-4ad0-950b-183b4ea629f4">

- Here is the POST request when no body is provided for the POST request.
- In Postman, show the JSON response for error for 404 when providing an unknown user ID to a UPDATE request.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/8e79f5fd-5867-4d86-a9ac-cefd8da2ef5f">
- UID is not provided and error 404 pops up during PUT request.

### Frontend
Blog JavaScript API fetch code and formatting code to display JSON.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/9fc67cac-93e4-442d-ba31-78a50acb53bc">
- Body that is provided to the fetch request to send a PUT request to the backend

- In Chrome inspect, show response of JSON objects from fetch of GET, POST, and UPDATE methods.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/3db958e0-bea4-490a-bf7c-7b35e502e3d2">
- In the context of our baking game, when the user bakes a pastry the user's points and baked goods have to be updated in the backend. In the image above the list that is provided to send the PUT request is shown.

> Returns a JSON list to the backend to update what items the user has as well as updating the points column
- In the Chrome browser, show a demo (GET) of obtaining an Array of JSON objects that are  formatted into the browsers screen.

 <img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/34fdddc7-6bb0-41d8-b75c-2852348ae00a">
- This is the leader board for our game, when a GET request is sent to the backend the array of user objects is printed in the console above to display all their attributes.
 
  - In JavaScript code, describe fetch and method that obtained the Array of JSON objects.
  > In the code that fetches the current items and points that the user has so they can be updated, it uses a GET request and finds the matching uid to receive a stringified array of the user's items in the backend.  
  - In JavaScript code, show code that performs iteration and formatting of data into HTML. 

  <img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/71653139-537b-4572-ad03-3bf23c220dee">
  > Iterates through data and formats into a leader board. 
- In the Chrome browser, show a demo (POST or UPDATE) gathering and sending input and receiving a response that show update.  Repeat this demo showing both success and failure.
  
  - In JavaScript code, show and describe code that handles success.  Describe how code shows success to the user in the Chrome Browser screen.

  <img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/1d2a2be4-6661-4e02-b45e-e3e5886dd2e3">

  <img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/e1de9969-c16c-4f82-b320-a0e46186ad72">
  > Success screen when correct ingredients are put into the baking pan 
  - In JavaScript code, show and describe code that handles failure.  Describe how the code shows failure to the user in the Chrome Browser screen.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/4fce9e26-e67c-4254-bfb9-ec893b18f6c8">
> When the user inputs the ingredients they want to try baking, it sends a GET request to a baking api which contains all possible recipe combinations. Then it, after sorting the ingredients the user inputted into a list, it compares the two lists and if the ingredient doesn't exist it returns as 'failed.'

## Optional/Extra, Algorithm Analysis
In the ML projects, there is a great deal of algorithm analysis. Think about preparing data and predictions.

- Show algorithms and preparation of data for analysis.  This includes cleaning, encoding, and one-hot encoding.
- Show algorithms and preparation for predictions.

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/8a4103f6-0b3e-44e6-a039-a67a8674312e">

> Converts data values to values that can be processed and trained. For example, the date is converted into a readable formate using the .to_datetime function. 

<img src="https://github.com/M8tth3/m8th3_2.0/assets/64436503/0acf8993-ea03-40cd-a042-81e201f28748">
> Reshapes to a 2d array, trains the data via Linear Regression. In the predictInflation function after training the data, it formats the input dates, then reshapes the timestamp to a 2D array so that it can run the predict function.  

- Discuss concepts and understanding of Linear Regression algorithms.
> Linear regression assumes a linear relationship between the two variables provided. In this case, it would be time and inflation. After taking the data it calculates the LSRL(Least squares regression line) to estimate values in the future, based off of the data provided by the user. In this case, the data that we provided was an inflation model with a generally upwards trend, so as time goes on the model predicts a certain increase in inflation each year. However, we only examine the impact of one independent variable which is time.
- Discuss concepts and understanding of Decision Tree analysis algorithms.
> Decision tree analysis in machine learning is to lay out all possible outcomes and making decisions based on those results. Decision trees can be used for both regression and classification tasks. In general in order to use decision trees data needs to first be preprocessed and cleaned. Then, to ensure the most accurate outcome, variables that are likely to have relevance to the target variable are chosen. Then the model is trained with either classification or regression. After evaluating the model's accuracy it can be used to make predictions on new and unseen data. 