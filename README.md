# COVID-19 (SARS-CoV-2) Pandemic Dataset for Greece # 

The aim of this repository is to create a dataset for the SARS-CoV-2 epidemic in Greece.

**:mega: LAST CASES UPDATE: 24/04/2020** 

## Updates ##

### 19/04/2020 ###
**Tests** variable on 14/04/2020 deleted due to misleading information in the press releases and reports.

### 15/04/2020 ###
Missing values due to missing report from 12/04/2020 were replaced as follows: Confirmed (Men), Confirmed (Women), Confirmed (>= 65 Years Old), Confirmed (40-64 Years Old), Confirmed (18-39 Years Old), Confirmed (0-17 Years Old) were replaced with the rounded (up) median value of the 11/04/2020 and 13/04/2020. Death Age (>=65 Years Old), Death Age (40-64 Years Old), Death Age (18-39 Years Old), Death Age (0-17 Years Old) were cross references from the news and are the actual values. All the other vales can be obtained from the press release.

r1 -> 12/04/2020 - [3 Death Age (>=65 Years Old) + 2 Death Age (Unidentified)](https://www.lifo.gr/now/greece/278098/koronoios-megalonei-o-arithmon-thymaton-stin-ellada-alloi-dyo-nekroi)  
r2 -> 12/04/2020 - [1 Death Age (>=65 Years Old)](https://www.news247.gr/koinonia/koronoios-stoys-99-oi-nekroi-stin-ellada.7622521.html) 

From the above we find out that the 2 Deaths with unidentified age are within the 40-64 Age group.

### 05/04/2020 ###
- Missing values are now reported as blank (Nan) rather than 0.
- Folder with the images added

### 04/04/2020 ###
- Raw folder now contains also the press releases from [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/) - Will be updated further
- Variables are now splitted into two csv files (2 sheets in xlsx). Standard & Secondary. Secondary variables are variables with multiple missing values
- New variables added in Standard and Secondary Variables. Standard Variables now include **Death (Women)** and **Death (Men)**. Secondary Variables now include **Death Age (>=65 Years Old)**, **Death Age (40-64 Years Old)**, **Death Age (18-39 Years Old)**, **Death Age (0-17 Years Old)**, **Travelers**, **Confirmed Transimission**. See the table below for more info.
- Data from now on will also be based in press releases from [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/)

### 03/04/2020 ###
- There are multiple missing values due to missing reports from [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/). The missing values are reported at the table below. 

### 29/03/2020 ###
- There are missing values from the 26/03/2020 to 29/03/2020 due to missing reports from National Organization of Public Health - [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/). The data from 26/03/2020 to 28/03/2020 are obtained from the press releases published in the website of the [Ministry of Health](https://www.moh.gov.gr/articles/ministry/grafeio-typoy/press-releases) and also saved as pdfs under [raw folder](daataset/raw). 
- The information included in the reports seems to have chanced since 29/03/2020. The reports do not include the following fields **Recovered (from hospital)**, **In Hospital**, **Hospitalized**, **In Hospital (men)**, **In Hospital (>65)**.
- **In Critical** variable since the 1st critical case in Greece 4/03/2020. The values are obtained trough the graphs in the 29/03/2020 report. 
- *eody_data* folder renamed to *dataset*.
- Several changes in the current README file.

## Data Sources ##
Data included are since the 26/02/2020, 1st confirmed case of SARS-CoV-2 in Greece. 

Until **19/03/2020** data are retrieved from [Novel Coronavirus (COVID-19) Cases, provided by JHU CSSE](https://github.com/CSSEGISandData/COVID-19)

From **20/03/2020** data are obtained by parsing the reports and press releases from the National Organization of Public Health - [Εθνικός Οργανισμός Δημόσιας Υγείας](https://eody.gov.gr/)

## Data explained ##
Under [dataset](dataset/) folder you can find the raw files (.pdf) from the National Organization of Public Health along with .csv(s) and .xlsx files which contain the following variables as a timeline. The following table shows the availability of each field per date. 

### STANRDARD VARIABLES ###

| Variable                     | From       | To         | Missing Values           |
|------------------------------|------------|------------|--------------------------|
| Confirmed                    | 2020-02-26 | 2020-04-24 | 2020-04-19               |
| Critical Condition           | 2020-02-26 | 2020-04-24 | 2020-04-19               |
| Deaths                       | 2020-02-26 | 2020-04-24 | 2020-04-19               |
| Tests                        | 2020-03-20 | 2020-04-24 | 2020-03-26, 2020-04-14, 2020-04-19   |
| Recovered (from hospital)    | 2020-02-26 | 2020-03-27 | 2020-04-19               |
| In Hospital                  | 2020-03-20 | 2020-03-25 | 2020-04-19               |
| Confirmed (Men)              | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-03, 2020-04-19 |
| Confirmed (Women)            | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-03, 2020-04-19 |
| Confirmed (\>= 65 Years Old) | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-02, 2020-04-19  |
| Confirmed (40-64 Years Old)  | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-02, 2020-04-19  |
| Confirmed (18-39 Years Old)  | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-02, 2020-04-19  |
| Confirmed (0-17 Years Old)   | 2020-03-20 | 2020-04-24 | 2020-03-26 - 2020-03-28, 2020-03-30 - 2020-04-02, 2020-04-19  |
| Death (Women)                | 2020-02-26 | 2020-04-24 | 2020-04-19               |
| Death (Men)                  | 2020-02-26 | 2020-04-24 | 2020-04-19               |


### SECONDARY VARIABLES ###

| Variable                    | From       | To         | Missing Values           |
|---------------------------  |------------|------------|--------------------------|
| Citizenship Identified      | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28, 2020-04-19  |
| Greek Citizenship           | 2020-03-20 | 2020-03-29 | 2020-03-26 - 2020-03-28, 2020-04-19  |
| Hospitalized                | 2020-03-20 | 2020-03-25 | 2020-04-19               |
| In Hospital (men)           | 2020-03-20 | 2020-03-25 | 2020-04-19               |
| In Hospital (\>=65)         | 2020-03-20 | 2020-03-25 | 2020-04-19               |
| Death Age (>=65 Years Old)  | 2020-04-03 | 2020-04-24 | 2020-04-19               |
| Death Age (40-64 Years Old) | 2020-04-03 | 2020-04-24 | 2020-04-19               |
| Death Age (18-39 Years Old) | 2020-04-03 | 2020-04-24 | 2020-04-19               |
| Death Age (0-17 Years Old)  | 2020-04-03 | 2020-04-24 | 2020-04-19               |
| Travelers                   | 2020-04-03 | 2020-04-24 | 2020-04-19               |
| Confirmed Transimission     | 2020-04-03 | 2020-04-24 | 2020-04-19               |


Only **Confirmed**, **Deaths**, **Recovered**, **Critical Condition**, **Death (Women)** and **Death (Men)**   are available before 20/03/20.

## Future Updates ##
- Explanation of the variables
- Automation on extracting the data from the .pdf files
- Map with the cases
- Contribution guide
- Visualizations

## Attributions ## 
For the thumbnail image:
<div>Icons made by <a href="https://www.flaticon.com/authors/freepik" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>
Icons made by <a href="https://www.flaticon.com/authors/smashicons" title="Smashicons">Smashicons</a> from <a href="https://www.flaticon.com/" title="Flaticon"> www.flaticon.com</a>