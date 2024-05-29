# Project Background
A food standard agency evaluates various establishments across the UK, and gives them hygiene rating. The editors of food magazine, Eat Save, Love has asked to evaulate some of the ratings data in order to help journalist and food critics decide where to focus future articles. 

### Important file:
Make sure that there is a folder called Resources. In that folder you will find **establishments.json**

## Database
There are 2 ways to create the database:
1. Open MongoDB, name the database **uk_food**, and name the collection **establishments**
2. Open Command Prompt and do the following:
<br>&ensp;- In Command Prompt, your terminal needs to be rooted/opened to "Resources" directory/folder 
<br>&ensp;- Copy and paste this line of code: mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
<br>&ensp;- Press Enter and you will know that you have successfully imported the json file when you see 3 lines simlar to the ones below: 
<br>&ensp; 2023-07-24T23:02:23.472-0400    connected to: mongodb://localhost/ 
<br>&ensp; 2023-07-24T23:02:23.473-0400    dropping: uk_food.establishments 
<br>&ensp; 2023-07-24T23:02:25.698-0400    39779 document(s) imported successfully. 0 document(s) failed to import. 

## Jupyter Notebook
**First run, NoSQL_setup_starter.ipynb**
<br>In this file, a new restaurant is added to the database, find a specific type of BusinessTypeID and only return BusinessTypeID and Business Type fields. Then the new restaurant BusinessTypeID is updated. Any establishment with LocalAuthorityName: Dover is removed from the database and number values that are stored as strings are convereted to the appropriate variable type. 

<br>**Next run NoSQL_analysis_start.ipynb**
<br>Exploratory analysis is conducted where specific information is asked from the magazine such as give establishments with hygene score equal to 20. 




