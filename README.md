# COVID19 (Coronavirus Disease) Dataset for Greece #

## **Please read the updates below for information on missing values** ##

**LAST UPDATE: 29/03/2020 11:45**

## Updates ##

### 29/03/2020 ###
- There are missing values from the 26/03/2020 to 29/03/2020 due to missing reports from National Organization of Public Health - [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/). The data from 26/03/2020 to 28/03/2020 are obtained from the press releases published in the website of the [Ministry of Health](https://www.moh.gov.gr/articles/ministry/grafeio-typoy/press-releases) and also saved as pdfs under [raw folder](daataset/raw). 
- The information included in the reports seems to have chanced since 29/03/2020. The reports do not include the following fields **Recovered (from hospital)**, **In Hospital**, **Hospitalized**, **In Hospital (men)**, **In Hospital (>65)**.
- **In Critical** variable since the 1st critical case in Greece 4/03/2020. The values are obtained trough the graphs in the 29/03/2020 report. 
- *eody_data* folder renamed to *dataset*.
- Several changes in the current README file.

## Aim ##
The aim of this repository is to create a dataset for the SARS-CoV-2 epidemic in Greece.

## Data Sources ##
Data included are since the 26/02/2020, 1st confirmed case of SARS-CoV-2 in Greece. 

Until **19/03/2020** data are retrieved from [Novel Coronavirus (COVID-19) Cases, provided by JHU CSSE](https://github.com/CSSEGISandData/COVID-19)

From **20/03/2020** data are obtained by parsing the reports from the National Organization of Public Health - [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/) -- **SEE UPDATES**

## Data explained ##
Under [dataset](dataset/) folder you can find the raw files (.pdf) from the National Organization of Public Health along with .csv and .xlsx files which contain the following variables as a timeline. The following table shows the availability of each field per date. 

| Variable                  | From       | To         | Missing Values           |
|---------------------------|------------|------------|--------------------------|
| Confirmed                 | 2020-02-26 | 2020-03-29 |                          |
| Deaths                    | 2020-02-26 | 2020-03-29 |                          |
| Tests                     | 2020-03-20 | 2020-03-29 | 2020-03-26               |
| Recovered (from hospital) | 2020-02-26 | 2020-03-25 |                          |
| In Hospital               | 2020-03-20 | 2020-03-25 |                          |
| In Critical               | 2020-02-26 | 2020-03-29 |                          |
| Hospitalized              | 2020-03-20 | 2020-03-25 |                          |
| Citizenship Identified    | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| Greek Citizenship         | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| Gender Identified         | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| Men                       | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| Women                     | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| Age Identified            | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| \>= 65 Years Old          | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| 40-64 Years Old           | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| 18-39 Years Old           | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| 0-17 Years Old            | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28  |
| In Hospital (men)         | 2020-03-20 | 2020-03-25 |                          |
| In Hospital (\>=65)       | 2020-03-20 | 2020-03-25 |                          |

Only **Confirmed**, **Deaths**, **Recovered** and **In Critical** are available before 20/03/20.

## Future Updates ##
- Explanation of the variables
- Automation on extracting the data from the .pdf files
- Map with the cases
- Contribution guide
- Visualizations
