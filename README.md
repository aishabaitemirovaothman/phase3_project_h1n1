# Seasonal Flu Vaccination Prediction Model
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
The dataset originally has 35 input features. We dropped two columns that had more than 46% percent of missing data ('employment_occupation' and 'employment_industry'). All the other features that had missing values were imputed using sklearn's SimpleImputer.
