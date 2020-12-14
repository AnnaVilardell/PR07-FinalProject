![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# PRO7-FinalProject


*Anna Vilardell*

*Data Analytics-Part Time Course | Barcelona June 2020*



## Content
- [Project Description and Workflow](#Project_Description_and_Workflow)
- [Organization](#Organization)
- [Links](#Links)



## Project Description and Workflow


### Description

This project is to apply Machine Learning in a real project.

**Dataset**

The dataset chosen is data of +40k student from IH.

**Metadata**
 
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


**Goal**

Classify if a potential student is going to enrol or not to a school. *What if it would be possible to predict if a potential student will enrol to IH?*  *What if we could understand his/her journey to enrol?*
 
 The main objectives will be:
   1. Know better funnel trends, to dedicate +/- resources to ≠ prospects and stages
   2. Recognize better our target, to give insights to marketing
   3. Predict better BSt, and so our revenue




### Workflow

1. Environment

2. Data Preparation

    2.1 EDA
    
    2.2 Data Wrangling
    
        - Explore Data
        - Clean Data
        - Remove usless columns
        - Creat new columns
    
    2.3 Feature Selection  
    
        - Feature selection was done togeter and after with the Model      
    
    2.4 Feature Engineering
    
        - Was not needed in this project for the type od data we had
        

3. Select From Model (Classification Models)
        
        - LogisticRegression
        - SVM
        - KNeighborsClassifier
        - LinearDiscriminantAnalysis
        - GaussianNB
        - RandomForestClassifier
        - MLPClassifier

4. Train Models (Machine Learning Classification Models)

        - RandomForestClassifier
          - Gridsearch
          - Classifier (with best params)
          - Feature Importance
          - Tree Visualization
   
5. Ensemble Methods

        - XGBoost
          - Gridsearch
          - Classifier (with best params)
          - Feature Importance



## Organization

**Main Organization of the project thought GitHub Project board:**

1. Organize a Project GitHub project board with main tasks and timings
2. Create a repository including a .gitignore file and a Readme.md
3. Data Preparation
4. Modeling
5. Tuning
6. Write conclusions
7. Prepare presentation
7. Complete Readme.md


**Inside this repository you can find:**

CSVs raw data:

    - apps_ih.csv
    - apps_ih_extended.csv (final version & used for our project)

CSVs clean data:
    
    - apps_allYears_semiClean.csv
    - apps_allYears_clean_selCols.csv
    - apps_allYears_clean_selCols_addCols.csv

    - apps_BCN20201_clean_selCols.csv
    - apps_BCN20201_clean_Sel_addCols.csv
    
    - apps_PAR20201_clean_selCols.csv
    - apps_PAR20201_clean_Sel_addCols.csv

   
Jupyter notebook:
    
    - Scraping API Salesforce.ipynb
    
    - EDA.ipynb
    
    - AllCampusesYears_DataWrangling.ipynb
    - AllCampusesYears_SelectFromModel .ipynb
    - AllCampusesYears_Model.ipynb
    - AllCampusesYears_Model_ImpFeatures.ipynb
    - AllCampusesYears_Ensemble_ImpFeatures.ipynb
       
    - BCN20201_DataWrangling.ipynb
    - BCN20201_Model.ipynb
    - BCN20201_Ensemble_ImpFeatures.ipynb

    - PAR20201_DataWrangling.ipynb
    - PAR20201_Model.ipynb
    - PAR20201_Model_ImpFeatures.ipynb
    - PAR20201_Ensemble_ImpFeatures.ipynb
    
Image:

    - ACY_M_tree.png
    - BCN01_M_tree.png
    - PAR01_M_tree.png
    - PAR01_M_FI_tree.png
    

Other:

    - README.md
    - tree.dot
    - AllCampuses&Years_tree.dot



## Links 

[Repository](https://github.com/AnnaVilardell/PR07-FinalProject/tree/dev)

[Presentation](TBDet)

[GitHub Project](https://github.com/AnnaVilardell/PR07-FinalProject/projects/1?add_cards_query=is%3Aopen)
