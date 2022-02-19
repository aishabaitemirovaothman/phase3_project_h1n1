# Seasonal Flu Vaccination Prediction Model (In Progress)
<p>
<b>Author:</b> Aisha Baitemirova-Othman
<br>
<b>Instructor:</b> David Elliott
</p>

![GettyImages-1166057429-copy-scaled](https://user-images.githubusercontent.com/92397144/145737018-1b3ded68-616c-4073-b139-2793121504b5.jpg)

## Objectives



## Business Problem
PetSmart Arizona is looking for ways to reduce the amount of sick days that its employees take by encouraging those who do not get flu vaccines to do so. Arizona law prohibits companies from requiring employees to provide a proof of vaccinations. Also company does not want to explicitly ask its employees about their vaccine status because that would make some employees uncomfortable and possibly not willing to disclose that information or give a misleading information for fear of being discriminated against. Instead, PetSmart wants to use a model that could accurately predict someone's vaccination status based on some basic input information about that person. Our team was tasked with building that prediction model. 

## Data
The dataset that we are using for training and testing our model is a dataset from https://www.drivendata.org/competitions/66/flu-shot-learning/. It consists of some features that each have some demographic information about a particular respondent as well as his/her opinion about flu vaccinations and whether he has a certain routine that prevents him/her from getting sick with flu. 
The dataset originally has 35 input features. We dropped two columns that had more than 46% percent of missing data ('employment_occupation' and 'employment_industry'). All the other features that had missing values were imputed using sklearn's SimpleImputer() transformer. 

## Models and Metrics
We used four different prediction models and compared their results using ROC AUC curve before tuning any hyperparameters. 
<img width="738" alt="Screen Shot 2021-12-10 at 08 54 37" src="https://user-images.githubusercontent.com/92397144/146062877-fa2ec38b-8b2b-42f8-aff1-c1f1c4818523.png">

The results after tuning the hyperparameters:

## Feature Analysis
We found out that two of the features are particularly important when predicting our target variable (whether someone is vaccinated against flu or not). The first one is the person's opinion about the risks associated with having flu. Those who think that the risks are very low tend to get vaccinated in far lower rates than those who take flu more seriously. 

<img width="399" alt="Screen Shot 2021-12-14 at 13 09 12" src="https://user-images.githubusercontent.com/92397144/146063750-c48cba31-70a7-46b3-8f8f-d398c0a864e1.png">

The second important feature is whether the person's doctor recommended to get vaccinated or not. The percentage of those who got vaccinated in the group whose doctors recommended them the vaccine is a lot higher than in the other group whose doctors did not recommend the flu vaccine. 

<img width="398" alt="Screen Shot 2021-12-14 at 13 18 07" src="https://user-images.githubusercontent.com/92397144/146064921-4242c90b-4d0f-41c6-8693-776da7bfc37e.png">

## Policy Recommendations
* Based on our findings we think that it is very important that PetSmart work on increasing the awareness of its employees of the potential dangers and complications of flu virus. 
* It is also very important to make sure that all of the company's employees have access to adequate and affrodable medical care. The reason for that is because the doctor's recommendation about a flu vaccine plays a major factor in whether the person is going to get vaccinated or not. We are not sure why not all people get a flu vaccine recommendation from their doctors, but we believe that one of the reasons is a possible lack of regular and affordable access to medical care. 
