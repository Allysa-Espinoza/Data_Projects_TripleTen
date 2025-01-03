# E-COMMERCE USER ACTIVITY ANALYSIS

## Description & Methods
The executive team of the E-commerce company is interested in understanding how well the website  converts product page views into purchases and better understanding how users interact with the website. Exploring the raw transaction logs in their data shows each row represents an activity, or event, by a user on the company’s website. Each time a user views a product page, opens their shopping cart, or completes a purchase, the event is captured in the activity logs. With this, the project was divided into four main parts:
### 1. Building a conversion funnel
   - Data from the “raw_user_activity” sheet was used to create the funnel in a pivot table as a new sheet called “conversion_funnel”
   - The COUNTUNIQUE function delivered only three stages in the funnel
   - using the counts in each stage, the 'total_conversion' and ' conversion_rates' columns were added to the pivot table with their respective calculations for each conversion stage.
### 2. Preparing data for cohort analysis
   - The acquisition cohorts were based on the month of a user's first purchase. The cohort metrics were also tracked by month.
   - created the 'purchase_activity' page by selecting only the purchase event types from the 'raw_user_activity' sheet using a data filter.
   - Using the new “purchase_activity” sheet data, inserted a pivot table as a new sheet called “first_purchase”. The pivot table settings were configured to calculate the minimum on the event_date field for each user.
   - the data was transferred to a new column: first_purchase_date in cell G1 of the “purchase_activity” sheet. VLOOKUP function was used to find the date from the “first_purchase” sheet that corresponds to the user ID in cell A2.
   - Three new columns were created to group the users and transactions by month for the cohort analysis: eveny_month, first_purchase_month, and cohort_age.
   - Used TEXT() function to create event_month in column H and first_purchase_month in column I. The months were formatted as YYYY-MM
   - DATEDIF() function was used to create cohort_age in column J as the number of months between the first purchase and the event
### 3. Calculating retention rates
  - Using the data from the “purchase_activity” sheet,  another pivot table was added as a new sheet called “cohort_analysis”. Used first_purchase_month for Rows, cohort_age for Columns, and user_id for Values.
  - created a new blank sheet called “retention_rates”, labeled cells A3 to A7 for each cohort age in chronological order, added column labels in cells B2 to E2 that represent the cohort ages from 1 to 4 months, and in cell B3, write a formula that calculates the retention rate for each cohort at each cohort age in the table you created, based on the starting cohort sizes.
### 4. Organizing and documenting the spreadsheet
  - wrote a results synopsis briefly summarizing the results and conclusions from the 'conversion_funnel' and 'retention_rates" sheets.
  - briefly explained the properties of each analysis; raw data, conversion funnel and retention rates.

## Findings
* The business analysis found that 10.34% of product page views convert to purchases, which is considered a good conversion rate, generally speaking.
* It was also found that retention rates are the highest in the cohort from '2020-09', and remain so for the longest time between all six cohort groups. While looking at the cohort analysis values can make it seem that the '2020-09' cohort has the least amount of conversions, only when you calculate the retention rates can you see what the numbers are really saying.

## Media
![184D3992-DFBC-461A-BA94-BE29C0F71B01](https://github.com/user-attachments/assets/446ce2d8-31ef-415d-a131-634750299c58)

![05F31C22-6792-403D-BADD-562E95A6F5D4](https://github.com/user-attachments/assets/5a79664c-b3af-4d2f-8f03-7b6e6e0d6e1f)

![A5FEBB4E-888F-4DF3-AA1E-3552424CDFEB](https://github.com/user-attachments/assets/0ee6899c-67dc-46a6-b517-30eb014dac45)

[E-Commerce User Activity - Executive Summary.pdf](https://github.com/user-attachments/files/18238958/E-Commerce.User.Activity.-.Executive.Summary.pdf)


## Link to project page
* https://docs.google.com/spreadsheets/d/1zCk-BiFZGvS8r3g2QGe8Qj6i8srMiEok37ZqbSnf2uY/edit?usp=sharing

## Deployment Instructions & System Requirements
#### Deployment Instructions for Google Sheets
* Access Google Sheets
  * Via Web Browser: Google Sheets is a cloud-based application, so there’s no need to install software. You can access it directly through your web browser by visiting the following link: https://workspace.google.com/products/sheets/
  * Via Google Drive: If you’re logged into Google Drive, you can create and manage Google Sheets by clicking the "New" button and selecting Google Sheets from the dropdown menu.
* Sign In
  *To use Google Sheets, you'll need a Google account. If you don’t have one, create a free Google account at Google Account Creation.
  *Sign in to your Google account to begin using Google Sheets.
* Create a New Google Sheet
  *Once logged into your Google account, go to Google Sheets or open Google Drive.
  *In Google Sheets, click on the + Blank option to create a new spreadsheet.
  *Alternatively, if you’re in Google Drive, click New > Google Sheets to create a new document.
* Work on Your Spreadsheet
  * Google Sheets offers all the basic functionality of traditional spreadsheet applications like Excel, including formulas, charts, data analysis tools, and collaboration features.
  * You can enter data, format cells, create formulas, insert charts, and much more.
* Collaborate and Share
  * Google Sheets allows multiple users to collaborate in real-time. To share a sheet:
  * Click on the Share button in the top right corner.
  * Enter the email addresses of people you want to share the sheet with or generate a shareable link.
  * You can set permissions (Viewer, Commenter, or Editor) for each person.
* Save and Access Sheets
  *Google Sheets automatically saves your work in real-time as you make changes. Your spreadsheet will be stored in your Google Drive, and you can access it from any device with an internet connection.
* Download and Export
  *You can download your Google Sheet in several formats, including:
   * Excel (.xlsx)
   * PDF
   * CSV
   * Web page (HTML)
   * For download: Go to File > Download, and select your preferred format.

#### System Requirements for Google Sheets
Google Sheets is a cloud-based application, meaning it works on any device with an internet connection and a supported web browser. Here are the basic requirements:

#### For Desktop (Web Browser)
* Operating System:
  * Windows 7 or later (for Windows users)
  * macOS 10.10 or later (for macOS users)
  * Linux (latest versions with a supported browser)
* Web Browser:
  * Google Chrome (Recommended)
  * Mozilla Firefox (Latest version)
  * Safari (Latest version)
  * Microsoft Edge (Latest version)
Note: Google Sheets works best on the latest versions of Chrome and Firefox. Older browser versions might have limited functionality.

* Internet Connection:
  * Required for accessing Google Sheets. Google Sheets is a cloud-based app, so a stable internet connection is essential for full functionality. However, you can also use Google Sheets offline by enabling offline mode in Google Drive.
* Screen Resolution:
  * Minimum: 1024 x 768 pixels for a better user experience. Higher resolutions (1920 x 1080 or more) are recommended for a clearer and more efficient workspace.
