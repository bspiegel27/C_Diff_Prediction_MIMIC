# Prediction of Clostridium Difficile Infection In ICU Patients Utilizing MIMIC-III Database
This project is my capstone project completed as part of the data science immersive program with General Assembly. For this project, I utilized the MIMIC-III ICU database (part of the physionet collaboration project between MIT and Beth Israel Medical Center). Project notebooks, presentations and a summary of findings/results below are in the process of being uploaded - check back soon for more content!

# MIMIC-III data background

    Dictionary and additional info can be found here: https://mimic.physionet.org/about/mimic/

    Schema: https://mit-lcp.github.io/mimic-schema-spy/

    GitHub Code Respository: https://github.com/MIT-LCP/mimic-code

# Project Notebooks
The following 3 notebooks have been uploaded so far:

### 1 - Create Patient Admits Dataframe
 
    Creates an initial dataframe of unique patient admissions and ICU stays alongside key demographics.
    Makes use of 3 MIMIC-III tables: Patients, Admissions, and ICUStays.
  
### 2 - C. Diff Infection Labeling and Inclusion Criteria Finalization
      
    C. Diff Case Definition:
      Timestamped lab diagnosis of CDI prior to cutoff of 2 days post-ICU intime

      Utilizing a standard cutoff of 2 days post-ICU admission aligns with timing of other risk assessments typically made such as
      mortality/morbidity predictions with scales like APACHE (made around 1 days after ICU admit). As such, a tool based on this model
      could be implemented into existing clinical workflows.

    Resulting Patient Population:
      
      Overall CDI rate of ~1.42%
      Total 670 cases / 47,000 ICU Stays

### 3 - Basic Demographics

    Demographic features explored:
        age
        gender
        insurance
        language
        ethnicity
        marital status

Note that underlying data files are not and will not be included given data use agreement signed to gain access to the data
