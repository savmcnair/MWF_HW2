# MWF_HW2
Repo 2 for Modern Workflows in Data Science
*1. Get EVS data. The data you want is ZA7500. You can find it here: https://search.gesis.org/research_data/ZA7500 (10%)*

I made a research account under my UMD email, smcnair1@umd.edu to download the data. I downloaded the SPSS version of the data, and stored it in the folder I will be working out of for this assignment.

*2. Write an overall report as a pdf.*

*• clean data for analysis (20%)*
Done in master_script. I created separate versions of this for the stats and public policy outputs, report_with_code and report_no_code.

*• descriptive tables, graphs and regression tables (20%)*
Done in master_script. I created separate versions of this for the stats and public policy outputs, report_with_code and report_no_code.

*• two version of the report, one showing no R code (for policy makers) and one that also shows your code (for statisticians) (10%)*
I created separate scripts so I could alter the output of the code in the pdfs using include=FALSE. The reports are stored in outputs > overall. The policy output is report_no_code and the stats output is report_with_code.

*3. Country level automated report in html.*

*• the 33 reports and the syntax that produces them (20%)*
I used two scripts to produce these outputs, flexible_by_country and template_report. These can be found in the scripts folder. 

*• dynamic (i.e., changes depending on the data) interpretation of results (10%)*

I added two dynamic reporting sections, sex and age, to each of the outputs. These give interpretations of the mean population and if more men or women are in the population. 

*4. Presentation of reports (e.g., labels and captions), Github repo structure and commits (10%)*

All graphs and tables have captions for the overall descriptives, graphs, and regression models. All graphs have titles and legends in all country reports. The dynamic report has 2 dynamic interpretations of the sex and age data for each country.

The GitHub repo is organized as such: 

- data folder, where I keep the unzipped 7500 data. 

- outputs - where all reports live

	- overall: 

		- report_with_code: stats report

		- report_no_code: policy report, with no r code

	- country_specific: has a dynamic report made for each country

- scripts: 
	- master_script: where I developed the code to get descriptives, graphs, and regression models. This was the basis for other scripts

	- report_with_code: creates the stats specific report with code for interpretation

	- report_no_code: creates policy specific report with no code for simplicity

	- flexible_by_country: where the loop for making the dynamic reports is, this is the script to run to create the country specific outputs

	- template_report: the template rmd file to make dynamic reports.
