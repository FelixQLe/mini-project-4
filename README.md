# Mini-project IV

### [Assignment](assignment.md)

## Project/Goals

    Deploying a Model to automate the loan eligibility process based on customer details that are provided as online application forms are being filled. These details concern the customer's Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History.

## Hypothesis
#### Possible hypotheses

    1. Applicants having a credit history more likely get approval, vice-versa. Credit history showing reliable informations of applicants income, spending and saving.
    - Plotting hist graph to compare between group

    2. Applicants with higher applicantincome and co-applicantincome has more more likely get approval. Income is evidently showing their ability to pay back their loan
    - Calculate the total_income(Applicantincome + co-ApplicantIncome) and ploting hist graph

    3. Applicants graduated is likely to be considered to Loan status decision. applicants  graduated is likely to get higher income and secure job which is showing their ability to pay back their loan soon.
    - Plotting hist graph to compare groups

    4. Semiurbun applicants has higher change to get approval, they are in high growth perspectives. Also, rural applicants might spend less than Urban applicants.
    - Plotting hist graph to compare groups

    5. Applicants with self_employed are likely to get approval. If they own a business. For those self_employed they will have high income.
    - Plotting hist graph to compare groups

    6. Applicants have more dependants likely get refused to loan decision. They have to spend more than other groups.
    - Plotting hist graph to compare groups

## EDA 
    1. Applicants having a credit history more likely get approval
![Screen Shot 2022-09-10 at 12 55 43 AM 2](https://user-images.githubusercontent.com/93171100/189472640-9e718536-4d19-4e48-a8fd-25d47fe8d91e.png) ![Screen Shot 2022-09-10 at 12 55 33 AM](https://user-images.githubusercontent.com/93171100/189472651-ceb2c558-63e2-4f89-ad7e-1ebadef527a9.png)

    2. Applicants with higher applicantincome and co-applicantincome has more more likely get approval
 ![Screen Shot 2022-09-10 at 2 42 55 AM](https://user-images.githubusercontent.com/93171100/189472681-069179f1-7f1b-4017-ba52-c065518807cf.png)![Screen Shot 2022-09-10 at 2 42 16 AM](https://user-images.githubusercontent.com/93171100/189472687-81a1c1a2-3de9-4436-8f1d-20ceccabde51.png)



    3. Applicants graduated is likely not to be considered to Loan status decision

    4. Semiurbun applicants has higher change to get approval, they are in high growth perspectives. Also,rural applicants might spend less than Urban applicants.
![Screen Shot 2022-09-10 at 2 41 20 AM](https://user-images.githubusercontent.com/93171100/189472714-c05ac865-4589-4355-89be-ae48f68b9629.png)
![Screen Shot 2022-09-10 at 2 41 40 AM](https://user-images.githubusercontent.com/93171100/189472715-b4d70de1-6e2f-4bb2-a20e-bd32e7a65f60.png)

    
    5. Self_employed status are likely not to be consider in loan decision
    
    6. Applicants have more dependants likely get refused to loan decision

## Process
    1. EDA & cleaning
    - Initial cleaning includes fill nan values with mean, median, mode
    - EDA includes grouping and visualization to test and determine the hypothesises
    2. Feature Engineering
    - numeric tranforming
    - variable tranforming
    - categories transforming
    3. Modeling
    - deploying Pipeline inlcudes numeric, variable, categories tranforming
    - deploying PCA, KBest, prediction model
    4. Deploying
    - Flask on Local
    - Flask on AWS
    4. Testing
    - Using Postpone send request

## Results/Demo
    - Model able to predict 76% accuracy
![Screen Shot 2022-09-09 at 4 14 38 PM](https://user-images.githubusercontent.com/93171100/189472775-52254d56-ce7e-4f58-8383-0c95505238b2.png)

    - API: Using Flask to create rest api which able to take POST requests with param json data from clients, then send back the pre-approval credit decison.
    
![Screen Shot 2022-09-09 at 5 27 02 PM](https://user-images.githubusercontent.com/93171100/189472782-a864e085-2fc9-42cf-a7fe-e82863cf4400.png)

## Challanges 
    - A 2-days project definitely is not enough time to work extra on EDA
    - Modeling is difficult if we want to use the raw data from customer input

## Future Goals
    - Definitely spending more time to do EDA and Modeling, that will imporve predictive power
