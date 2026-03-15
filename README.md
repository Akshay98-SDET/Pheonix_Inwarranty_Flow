# Postman API Automation Integration with Github Actions #
This repository is a demonstration for POC for integrating for postman tests with Postman actions. The tests are written in postman and they are executed on the VM with help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on evry push to the main branch. You can also execute the projects manually using workflow_dispatch. The projects runs on a scheduled time with the help of cron job.

The HTML report is archived and kept in the Artifact section for the team to download, along with that they can view the report directly from Github Pages: https://akshay98-sdet.github.io/Pheonix_Inwarranty_Flow/
The latest reports is mailed to the team members using GMAIL SMTP.

## About Me ##
Hi, My name is Akshay. I have over 4 years of experience working as QA Engineer with knowledge on UI and API Automation using Selenium and RestAssured.
You can connect with me over : https://www.linkedin.com/in/akshayjagadal

## Test Coverege ##
1. Happy flow testing
2. Negative testing and Edge case testing
3. Token testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets Management with Github Secrets

## Tech Stacks ##
1. Postman
2. Node.js 22v
3. Newman
4. Newman-reporter-htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 instance for self hosted Github Runner



## Github Pages ##
You can directly view the latest test report of the postman tests at github page link: https://akshay98-sdet.github.io/Pheonix_Inwarranty_Flow/

## How to run the Project ##
You can run the project on your local system for that:
1. Clone the project on local system: https://github.com/Akshay98-SDET/Pheonix_Inwarranty_Flow
2. Install Nodejs and NPM from https://nodejs.org/en
3. Install Newman using npm install -g newman
4. Install newman-reporter-htmlextra npm install -g newman-reporter-htmlextra
5. Run the newman command:
             newman run 'Inwarranty-flow Collection.postman_collection.json' \
            -e QA.postman_environment.json \
            -d testData.csv \
            -r cli,htmlextra \
            --reporter-htmlextra-export ./newman/index.html

## HTML Report ##
The report will be created in newman folder
![Newman Report](https://github.com/Akshay98-SDET/Pheonix_Inwarranty_Flow/blob/static-content/newman-report.png)
