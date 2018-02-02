
![alt text](extra/med.png)

## USA MEDICARE DATA ANALYSIS

In this submission, I am going to explore Medicare data of United States. The file being used is:

* hospital_gen_info.csv

The data is provided by **Data.Medicare.gov**.It provides direct access to the official data from the Centers for Medicare & Medicaid Services (CMS) that are used on the Medicare.gov Compare Websites and Directories.

**hospital_gen_info.csv** consits a list of all Hospitals that have been registered with Medicare. The list includes addresses, phone numbers, hospital type and many quality measures.

The hospital overall ratings are designed to assist patients, consumers, and others in comparing hospitals side-
by-side. The hospital overall ratings show the quality of care a hospital may provide compared to other
hospitals based on the quality measures reported on Hospital Compare. The hospital overall rating summarizes
more than 60 measures reported on Hospital Compare into a single rating. The measures come from the IQR,
OQR, and other programs and encompass measures in seven measure groups: mortality, safety of care,
readmission, patient experience, effectiveness of care, timeliness of care, and efficient use of medical imaging.
The hospitals can receive between one and five stars, with five stars being the highest rating, and the more
stars, the better the hopsital performs on the quality measures. Most hospitals will display a three star rating.


The data exploration includes:
* **Step 1** Quick Data Exploration; to view the basic data structure in CSV
* **Step 2** Audit / Validate Data; to check our data for various attributes like, uniqueness, completeness, accuracy, consistancy
* **Step 3** Clean Data; to remove bad entries like blank values or Null values in our dataset
* **Step 4** Reformat Data; to adjust our dataset such that it fits into our database
* **Step 5** Insert Data; to insert data from dataset into our database
* **Step 6** Data Analysis; we go through various use cases to analyse the data 

The use cases tested for are:
* distribution of Medicare registered hospitals in each State
    
    We observe that Texas has most number of Medicare registered hospitals followed by California, Florida, Illinois and New York. Northern Mariana Islands, American Samoa and Dover have the least number of Medicare registered hospitals
    
    
    
    
* distribution of different Hospital Owners with Hospital rating more than 3 (good)
    
    We observe that non-Profit Private hospitals have most number of Good ratings, while Federal Government dont have many GOOD ratings for their hospitals.
    
    
    
* which of the High rated hospitals (ratings more than 3) have Readmission rate above National Average. Which means, how frequent are readmissions for high rated hospitals.
    
    We observe that a lot of Hospitals in California and Arizona, although have high overall ratings, but the rate at which patients get hospitalied within 30-Days is Above National Average. Which means, these hospitals perform well on other quality measures, however, patients tend to get hospitalized back more often.
    
    
    
* which of the low rated hospitals (ratings less than 3) have Mortality rate higher than National Average. We also observe which ownership do these hospitals belong to.
    
    We observe that a lot of Voluntary non-Profit Private hospitals have a very low rating and high mortality rate
    
    
    
* State-wise distribution of hospitals with high (above national average) mortality rate
    
    We observe that many Medicare registered hospitals in states like California, Florida, Massachusetts have Mortality Rate higher than National Average. This can be a very important indicator for Hospitals, either Private or Federal. It could mean that more patients in CA, FL and MA visit hospitals in critical conditions.
