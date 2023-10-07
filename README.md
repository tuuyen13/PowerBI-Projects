# PowerBI-Projects

This repository contains a collection of Power BI projects that sole real-world problems
## 📌 Case Studies
- [Case Study #1 - Data Professional Survey](#1-case-study-1---data-professional-survey)
- [Case Study #2 - Analyzing Customer Churn](#2-case-study-2---analyzing-customer-churn)
- [Case Study #3 - Competitor Sales Analysis](#3-case-study-3---competitor-sales-analysis))
- [Case Study #4 - HR Analytics](#4-case-study-4---hr-analytics)

## 1. Case Study #1 - Data Professional Survey


## 2. Case Study #2 - Analyzing Customer Churn
The problem: Solving customer churn
- A fictitious dataset about churn from a Telecom provider (Databel)
- Your task: discover why customers are churning
### Customer status
| Variable           | Description                                       |
|------------------|---------------------------------------------------|
| `Customer ID`    | The unique ID that identifies a customer         |
| `Churn Label`    | Contains "Yes" or "No" to indicate if a customer churned |
| `Churn Reason`   | The particular reason why the customer ended the contract |
| `Churn Category` | Groups multiple churn reasons together for analysis purposes |
### Demographics
| Variable          | Description                                              |
|------------------|----------------------------------------------------------|
| `Gender`     | The gender of the customer, indicated by "Male", "Female" or "Prefer not to say" |
| `Under 30`         | Indicates if the customer is under 30 with "Yes" or "No" |
| `Senior`     | Indicates if the customer is 65 or above with "Yes" or "No" |
| `Age`        | The age of the customer                                   |

### Contract information:
| Variable            | Description                                              |
|-----------------|----------------------------------------------------------|
| `Contract Type` | Contains "Month-to-Month", "One Year" or "Two Year"     |
| `Payment Method`| Preferred payment method of the customer indicated with "Credit Card", "Direct Debit" or "Paper Check" |
| `State`         | The code of the state where the customer lives          |
| `Phone Number`  | Phone number of the customer                             |
| `Group`         | Indicates if the customer is part of a group contract. A group contract offers advantages and is generally cheaper. Contains "Yes" or "No" |
| `Number of Customers in Group` | Number of customers part of the group               |

### Subscription types & Charges
| Variable                           | Description                                                                                             |
|----------------------------------|---------------------------------------------------------------------------------------------------------|
| `Account Length (in months)`     | The number of months the customer has been with Databel                                                |
| `Local Calls`                    | Amount of local (within the US) calls from the customer                                                  |
| `Intl Calls`                     | Amount of international (outside the US) calls from the customer                                         |
| `Intl Mins`                      | The number of minutes spent calling internationally                                                      |
| `Intl Plan`                      | Indicates if the customer has a premium plan to call internationally for free with "Yes" or "No". This premium is reflected in the amount of the monthly charge |
| `Extra International Charges`    | Contains the extra charges for international calls for customers who are not on an international plan  |
| `Customer Service Calls`         | The number of calls made to customer service                                                             |
| `Avg Monthly GB Download`        | Contains the average monthly download volume in gigabytes                                                |
| `Unlimited Data Plan`            | Indicates if the customer has free unlimited download capacity with "Yes" or "No". This premium is reflected in the amount of the monthly charge |
| `Extra Data Charges`             | Contains the extra charges for data downloads for customers who are not on an unlimited plan           |
| `Monthly Charges`                | Average of all Monthly Charges to the customer                                                           |
| `Total Charges`                  | Sum of all monthly charges                                                                              |

## 3. Case Study #3 - Competitor Sales Analysis
Case study scenario: 
- Analyze manufacturers' sales internally
- Comparing sales against other competitors
- Comparing product performance against other competitors
### Products
| Field          | Description                                                 |
|----------------|-------------------------------------------------------------|
| `PerformancelD`| A unique ID that identifies a product.                       |
| `Product`      | Name of the product.                                        |
| `Segment`      | Contains the segment of the product.                         |
| `Category`     | Contains the type of product category.                       |
| `ManufacturerID`| A unique ID that identifies a manufacturer. Connects to Manufacturer. |
| `Price`        | Contains the price and currency of the product.             |
| `Description`  | Description of the product.                                 |
### Manufacturer
| Field           | Description                                      |
|-----------------|--------------------------------------------------|
| `ManufacturerID`| A unique ID that identifies the manufacturer.    |
| `Manufacturer`  | Name of the manufacturer.                        |
| `Logo`          | Hyperlinks that store the logo images of the manufacturers. |

### Geography
| Field     | Description                                  |
|-----------|----------------------------------------------|
| `Zip`     | Contains the zipcode of a specific region.  |
| `City`    | Contains the name of the city.              |
| `State`   | Contains the name of the state.             |
| `Region`  | Contains the region details.                |
| `District`| Contains the district name.                 |
| `Country` | Contains the name of the country.           |

### Sales
| Field       | Description                                                  |
|-------------|--------------------------------------------------------------|
| `ProductID` | A unique ID that identifies the product. Connects to Products table. |
| `Date`      | Contains the date of the transaction.                        |
| `Zip`       | Contains the zipcode where the transaction happened.         |
| `Units`     | Number of units sold of the product.                         |
| `Revenue`   | Revenue generated by the product.                            |

### International Sales Folder
| Field       | Description                                                |
|-------------|------------------------------------------------------------|
| `ProductID` | A unique ID that identifies the product.                   |
| `Date`      | Contains the date of the transaction.                      |
| `Zip`       | Contains the zipcode where the transaction happened.       |
| `Units`     | Number of units sold of the product.                       |
| `Revenue`   | Revenue generated by the product.                          |
| `Country`   | Contains the name of the country where the transaction happened. |

## 4. Case Study #4 - HR Analytics
Case study goals
- Monitor key HR metrics on employees
- Understand what factors impact attrition
### Performance
| Variable                             | Description                                                             |
|-----------------------------------|-------------------------------------------------------------------------|
| `PerformanceID`                   | A unique ID that identifies an individual performance review.            |
| `EmployeeID`                      | A unique ID that identifies an employee. Connects to DimEmployee.       |
| `ReviewDate`                      | Date an employee's review took place.                                    |
| `EnvironmentSatisfaction`         | Rating for employees' satisfaction with their environment. Connects to DimSatisfiedLevel. |
| `JobSatisfaction`                 | Rating for employees' satisfaction with their job role. Connects to DimSatisfiedLevel.  |
| `RelationshipSatisfaction`        | Rating for employees' satisfaction with their relationships at work. Connects to DimSatisfiedLevel. |
| `WorkLifeBalance`                 | Rating for employees' satisfaction with their work-life balance. Connects to DimSatisfiedLevel. |
| `SelfRating`                      | Rating for employees' performance based on their own view. Connects to DimRatingLevel. |
| `ManagerRating`                   | Rating for employees' performance based on their manager's view. Connects to DimRatingLevel. |
| `TrainingOpportunitiesWithinYear` | Number of training opportunities offered in the last 12 months.           |
| `TrainingOpportunitiesTaken`      | Number of training opportunities taken.                                  |
### Employee
| Field                  | Description                                                                                                      |
|------------------------|------------------------------------------------------------------------------------------------------------------|
| `EmployeeID`           | A unique ID that identifies an employee.                                                                        |
| `FirstName`            | First name of an employee.                                                                                      |
| `LastName`             | Last name of an employee.                                                                                       |
| `Gender`               | Self-defined employee gender identity.                                                                          |
| `Age`                  | Current age of an employee.                                                                                     |
| `Business Travel`      | Frequency of business travel - three categories: Frequent Traveller, Some Travel, and No Travel.               |
| `Department`           | Department an employee works in three categories: Technology, HR, and Sales.                                   |
| `DistanceFromHome`     | Kilometer distance between an employee's home and their office.                                                 |
| `State`                | State where the employee lives.                                                                                 |
| `Ethnicity`            | Self-defined employee ethnicity.                                                                                |
| `Education`            | Education level for employees'. Connects to DimEducationLevel.                                                  |
| `EducationField`       | Employee field of study.                                                                                        |
| `Job Role`             | Current/latest employee job role.                                                                               |
| `MaritalStatus`        | Current/latest employee marital status.                                                                        |
| `Salary`               | Current/latest employee salary.                                                                                 |
| `StockOptionLevel`     | The banding level for stock options that the employee has.                                                       |
| `Overtime`             | Contains "Yes" and "No" to indicate whether an employee is expected to work overtime in their role.            |
| `HireDate`             | Date the employee joined the company.                                                                          |
| `Attrition`            | Contains "Yes" and "No" to indicate whether an employee has left the organization.                              |
| `YearsAtCompany`       | Number of years since the employee joined the organization.                                                       |
| `YearsInMostRecentRole`| Number of years the employee has been in their most recent role.                                                 |
| `YearsSinceLastPromotion` | Number of years since the employee last got promoted.                                                        |
| `YearsWithCurrManager` | Number of years the employee has been with their current manager.                                                |

### Satisfied Level
| Field              | Description                                                                                             |
|--------------------|---------------------------------------------------------------------------------------------------------|
| `SatisfactionID`   | A unique ID that connects to EnvironmentSatisfaction, JobSatisfaction, RelationshipSatisfaction, and Work-Life Balance in FactPerformanceRating. |
| `SatisfactionLevel`| Provides meaning to the satisfaction level: Very Satisfied, Satisfied, Neutral, Dissatisfied, and Very Dissatisfied. |


### Rating level
| Field           | Description                                                                                      |
|-----------------|--------------------------------------------------------------------------------------------------|
| `RatingID`      | A unique ID that connects to SelfRating and ManagerRating in FactPerformanceRating.            |
| `RatingLevel`   | Provides meaning to the rating level: Above and Beyond, Exceeds Expectation, Meets Expectation, Needs Improvement, and Unacceptable. |

### Education Level
| Field                | Description                                                                                     |
|----------------------|-------------------------------------------------------------------------------------------------|
| `EducationLevellD`   | A unique ID that connects to Education in DimEmployee.                                           |
| `EducationLevel`     | Provides meaning to the education level: Doctorate, Masters, Bachelors, High School, and No Formal Qualifications. |
