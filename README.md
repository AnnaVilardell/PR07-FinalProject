![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Ironhack Sales Funnel Prediction


*Anna Vilardell*

*Data Analytics-Part Time Course | Barcelona June 2020*

*PRO7-FinalProject*

_____________________________________________________________________________________________________________________________________________________________


Deriving meaningful insights from data, and converting knowledge into action, is easier said than done.

There are challenges that organizations face in adopting analytics. As for instance, during this project 2 of the challenges I’ve found were:
- Poor quality data, referring to both qualitative and quantitative pieces of information
- Data privacy, also called information privacy which is the aspect of information technology (IT) that deals with the ability an organization or individual has to determine what data in a computer system can be shared with third parties.

Regardless of above the mentioned challenges, the importance of data and capturing the impact from analytics will be my overall goal through this project.


![Data Impact](https://s27389.pcdn.co/wp-content/uploads/2020/05/coronavirus-diary-when-data-science-becomes-an-art-1-1024x440.jpeg)



## Content
- [Content](#Content)
- [Project Description](#Project_Description)
- [Project Workflow](#Project_Workflow)
- [Organization](#Organization)
- [Links](#Links)



## Project Description


As the definiton says, Machine learning is an application of artificial intelligence (AI) that provides systems the ability to automatically learn and improve from experience without being explicitly programmed. It focuses on the development of computer programs that can access data and use it to learn for themselves.

In my case, I've used machine learning to create a model that not only predicts Ironhack Sales but also shows the journey of that sale with a decision tree.

Besides my deep love for data, being the Admissions Manager at Ironhack Barcelona, have drove me to see the importance of data and its potential. Unfortunately, most of the times we collect a lot of data but without paying much attention to its quality and not having time to take a look at the one we have and use it smartly. So, this project have gave me the opportunitty to work on it.


**Dataset**

The dataset chosen is data of +40k potential students that have applied to 1 of our Ironhack campus between the year 2016 to 2021. Note that Ironhack has 10 campuses inclusing Remote campus.

The specific date we have from our students is besides demographic data, dates/timings of the bootcamp, the type of the bootcamp they applied to, the cost od the bootcamps...

    Metadata
 
    - bootcamp_course: course associated to the opportunity, either WD, UX or DA.
    - bootcamp_format: format associated to the opportunity, either FT or PT.
    - bootcamp_start_date: Start Date of the course associated to thez opportunity.
    - stage: The stage name the application lives at that moment.
    - lost_deal_reason: Reason why the applicant has dropped the admission process
    - stage_before_lost: The stage where the opportunity is before getting lost
    - created_date: Date and time when this record was created.
    - close_date: Date when the opportunity is expected to close (before closing) or closed.
    - drop_reason: Reason why the applicant has dropped after paying his deposit
    - net_amount: Amount minus Discount or Scholarship Amount
    - discount_type: Type of the discount, either Scholarship or Discount
    - discount_name: Name of the discount initiative associated to the opportunity
    - discount_amount: Amount of the discount that the applicant received
    - scholarship_name: Name of the scholarship initiative associated to the opportunity
    - scholarship_amount: Amount of the scholarship discount given to the opportunity
    - financing_options: name of the financing option
    - financing_option_amount: amount in local currency of the financing option
    - deposit_payment: The amount of the tuition neither the student or Ironhack paid
    - Stage Duration: The number of days the opportunity was in the stage listed in the Stage column
    - ...


**Main objectives**

I've create a model to classify if a potential student is going to enrol or not to the Ironhack School and, moreover, to undersand the journey he/she is more likely to follow. See below an example of a tree where we could see the journey of the Paris Campus prospects:

![TreeExample](Images/PAR01_M_tree.png)
 
 The 3 objectives that will impact Ironhack are:
   1. Know better funnel trends per campus, to dedicate +/- resources to ≠ prospects and stages depending on the campus they are applying.
   2. Recognize better our target, to give insights to marketing. This will also enable us to receive later more qualify prospects.
   3. Predict better sales, and so revenue. This will also enable us to better treat the cashflow.



##  Project Workflow

1. Environment

2. Data Preparation

    2.1 EDA
    
    2.2 Data Wrangling
    
        - Explore Data
        - Clean Data
        - Remove usless columns
        - Creat new columns
    
    2.3 Feature Selection  
    
        - Feature selection was done togeter with the Model
        

3. Select From Model (Classification Models)
        
        - Data Preprocessing
        - Classification Models
            - LogisticRegression
            - SVM
            - KNeighborsClassifier
            - LinearDiscriminantAnalysis
            - GaussianNB
            - RandomForestClassifier
            - MLPClassifier

4. Train Models (Machine Learning Classification Models)

        - RandomForestClassifier
          - Data Preprocessing
          - Gridsearch
          - Classifier (with best params)
          - Feature Importance
          - Tree Visualization
   
5. Ensemble Methods

        - XGBoost
          - Data Preprocessing
          - Gridsearch
          - Classifier (with best params)
          - Feature Importance



## Organization

### Main Organization of the project thought GitHub Project board

1. Organize a Project GitHub project board with main tasks and timings
2. Create a repository including a .gitignore file and a Readme.md
3. Data Preparation
4. Modeling
5. Tuning
6. Write conclusions
7. Prepare presentation
7. Complete Readme.md



### Inside this repository you can find 3 folders with all data:

**CSVs folder**

   - CSVs raw data (will only be available to Irohack Staff):

       - apps_ih.csv
       - apps_ih_extended.csv (final version & used for our project)

   - CSVs clean data:

       - apps_allYears_semiClean.csv
       - apps_allYears_clean_selCols.csv
       - apps_allYears_clean_selCols_addCols.csv

       - apps_BCN20201_clean_selCols.csv
       - apps_BCN20201_clean_Sel_addCols.csv

       - apps_PAR20201_clean_selCols.csv
       - apps_PAR20201_clean_Sel_addCols.csv

  
**Notebooks folder**

1. Environment
   
   - Scraping API Salesforce.ipynb

2. Data Preparation

   - EDA.ipynb 
   - AllCampusesYears_DataWrangling.ipynb
   - BCN20201_DataWrangling.ipynb
   - PAR20201_DataWrangling.ipynb

3. Select From Model (Classification Models)
     
   - AllCampusesYears_SelectFromModel .ipynb

4. Train Models (Machine Learning Classification Models)
    
   - AllCampusesYears_Model.ipynb
   - AllCampusesYears_Model_ImpFeatures.ipynb
   - BCN20201_Model.ipynb
   - PAR20201_Model.ipynb
   - PAR20201_Model_ImpFeatures.ipynb

5. Ensemble Methods
   
   - AllCampusesYears_Ensemble_ImpFeatures.ipynb
   - BCN20201_Ensemble_ImpFeatures.ipynb
   - PAR20201_Ensemble_ImpFeatures.ipynb


**Images folder**

   - ACY_M_tree.png
   - BCN01_M_tree.png
   - PAR01_M_tree.png
   - PAR01_M_FI_tree.png

**Other documents**

   - README.md
   - tree.dot
   - AllCampuses&Years_tree.dot


## Links 

[Repository](https://github.com/AnnaVilardell/PR07-FinalProject/tree/dev)

[Presentation](https://docs.google.com/presentation/d/196ZB-p4pVIgY2WUVr9x7SytEhjKWepOd5rbtqUL-bPs/edit#slide=id.g35f391192_00)

[GitHub Project](https://github.com/AnnaVilardell/PR07-FinalProject/projects/1?add_cards_query=is%3Aopen)
