Make sure that there is a folder called Resources. In that folder you will find:
<br>&ensp; 1. establishments.json

## Command Prompt
<br>Before running opening Jupyter Notebook, you need to open Command Prompt.
<br>&ensp;- In Command Prompt, your terminal needs to be rooted/opened to "Resources" directory/folder 
<br>&ensp;- Copy and paste this line of code: mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
<br>&ensp;- Press Enter and you will know that you have successfully imported the json file when you see 3 lines simlar to the ones below: 
<br>&ensp; 2023-07-24T23:02:23.472-0400    connected to: mongodb://localhost/ 
<br>&ensp; 2023-07-24T23:02:23.473-0400    dropping: uk_food.establishments 
<br>&ensp; 2023-07-24T23:02:25.698-0400    39779 document(s) imported successfully. 0 document(s) failed to import. 

## Jupyter Notebook
<br>First run, NoSQL_setup_starter.ipynb
<br>Then run, NoSQL_analysis_start.ipynb




