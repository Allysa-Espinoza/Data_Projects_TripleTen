# SHOPIFY APP ANALYSIS

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
![DD497202-A125-405A-916E-AF7A011FC4AE_1_105_c](https://github.com/user-attachments/assets/38ac5d84-86b6-457f-9e65-0bb2c6893edd)

![4F424CF6-8CF8-4331-BA97-3CC809F02CBE_1_105_c](https://github.com/user-attachments/assets/e194b76b-2c4e-44b5-83fd-898ecd4fc07a)

![A09A9F4C-ADC6-43ED-9FA9-9070C14FDFF1_1_105_c](https://github.com/user-attachments/assets/cbe77482-7bbd-46e5-bf87-fabf526b40bf)


## Link to project page
N/A

## Deployment Instructions & System Requirements
#### Deployment Instructions for Power BI
* Download Power BI Desktop
  * Power BI Desktop is available for free and can be installed on Windows-based systems.
  * Go to the official Microsoft Power BI website: Power BI Desktop Download.
  * Click "Download free" to get the installer.
* Install Power BI Desktop
  * Once the installer (.exe file) has been downloaded, double-click it to start the installation process.
  * Follow the on-screen instructions:
  * Choose your preferred installation options.
  * Click Install when prompted to begin the installation.
* Launch Power BI Desktop
  * After installation, open Power BI Desktop by searching for it in the Start Menu or by clicking the Power BI Desktop icon on your desktop.
  * The first time you launch the application, you may be prompted to sign in to your Microsoft account. If you don't have one, you can create one at Microsoft Account Signup.

#### System Requirements for Power BI
Here are the system requirements for running Power BI Desktop on your local machine:

For Windows:
Operating System:

Windows 10 (64-bit) or later
Windows Server 2016 or later (for server environments)
Power BI Desktop does not run on older versions of Windows (Windows 8.1 or lower, Windows 7).
Processor:

A 64-bit processor (x64 architecture)
At least 1 GHz or faster, with at least 2 cores (4 cores or more recommended for large datasets)
Memory (RAM):

Minimum 2 GB of RAM (4 GB or more recommended for better performance)
8 GB or more of RAM is recommended for larger data models or complex reports.
Disk Space:

At least 1 GB of free disk space (more may be required depending on data model size)
Display:

A screen resolution of at least 1440 x 900 or higher is recommended for optimal display of data and visuals.
Graphics:

A DirectX 10 compatible graphics card for accelerated rendering. While not strictly required, it improves performance with large visualizations.
Internet Connection:

Required for downloading and installing Power BI Desktop.
An internet connection is also required for publishing reports to Power BI Service and for receiving data refresh updates (if applicable).
Power BI Service (for Online Use and Collaboration)
To fully utilize Power BI and collaborate with colleagues or stakeholders:

Browser Compatibility:

Latest versions of Google Chrome, Microsoft Edge, Safari, or Mozilla Firefox are supported.
Internet Explorer is not recommended for an optimal experience.
Power BI Service Subscription (Optional):

While Power BI Desktop is free, to share and collaborate with others or access more advanced features, you may need a Power BI Pro or Power BI Premium license.
The Power BI Pro license offers collaboration, sharing, and additional features, while Power BI Premium offers dedicated cloud resources and increased data model size for enterprise needs.

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
