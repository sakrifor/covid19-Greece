# COVID19 (Coronavirus Disease) Dataset for Greece #

**LAST UPDATE: 26/03/2020 13:00**
**WILL BE UPDATED DAILY** 

## Aim ##
The aim of this repository is to create a dataset for the SARS-CoV-2 epidemic in Greece.

## Data Sources ##
Data included are since the 26/02/2020, 1st confirmed case of SARS-CoV-2 in Greece. 

Until **19/03/2020** data are retrieved from [Novel Coronavirus (COVID-19) Cases, provided by JHU CSSE](https://github.com/CSSEGISandData/COVID-19)

From **20/03/2020** data are obtained by parsing the reports from the National Organization of Public Health - [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/)

## Data explained ##
Under [eody_data](eody_data/) folder you can find the raw files (.pdf) from the National Organization of Public Health along with .csv and .xlsx files which contain the following variables as a timeline. 

- Confirmed
- Deaths
- Recovered (from Hospital)
- Tests
- Citizenship Identified
- Greek Citizenship
- Gender Identified
- Men
- Women
- Age Identified
- \>= 65 Years Old
- 40-64 Years Old
- 18-39 Years Old
- 0-17 Years Old
- Hospitalized
- In Hospital
- Critical
- In Hospital (men)
- In Hospital (>65)

Only **Confirmed**,**Deaths** and **Recovered** are available before 20/03/20.

## Future Updates ##
- Explanation of the variables
- Automation on extracting the data from the .pdf files
- Map with the cases
- Contribution guide
- Visualizations
