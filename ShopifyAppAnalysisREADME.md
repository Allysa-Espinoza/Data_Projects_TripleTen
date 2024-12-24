# SHOPIFY APP ANALYSIS

## Description & Methods
The project was to be conducted in the role of a newly hired analyst to review the landscape of apps on the Shopify platform, using data scraped from publicly available Shopify websites to figure out what key factors play into the success of a Shopify app.  With this, the project was divided into three main tasks:
### 1. App Landscape
   - To find key statistics on the types of apps there are, a new sheet 'App Landscape' was created and it used data from the Apps table
    - added a KPI Card counting the unique number of apps
    -  
### 2. Reviews
   - The acquisition cohorts were based on the month of a user's first purchase. The cohort metrics were also tracked by month.
   - created the 'purchase_activity' page by selecting only the purchase event types from the 'raw_user_activity' sheet using a data filter.
   - Using the new “purchase_activity” sheet data, inserted a pivot table as a new sheet called “first_purchase”. The pivot table settings were configured to calculate the minimum on the event_date field for each user.
   - the data was transferred to a new column: first_purchase_date in cell G1 of the “purchase_activity” sheet. VLOOKUP function was used to find the date from the “first_purchase” sheet that corresponds to the user ID in cell A2.
   - Three new columns were created to group the users and transactions by month for the cohort analysis: eveny_month, first_purchase_month, and cohort_age.
   - Used TEXT() function to create event_month in column H and first_purchase_month in column I. The months were formatted as YYYY-MM
   - DATEDIF() function was used to create cohort_age in column J as the number of months between the first purchase and the event
### 3. App Reviews
  - Using the data from the “purchase_activity” sheet,  another pivot table was added as a new sheet called “cohort_analysis”. Used first_purchase_month for Rows, cohort_age for Columns, and user_id for Values.
  - created a new blank sheet called “retention_rates”, labeled cells A3 to A7 for each cohort age in chronological order, added column labels in cells B2 to E2 that represent the cohort ages from 1 to 4 months, and in cell B3, write a formula that calculates the retention rate for each cohort at each cohort age in the table you created, based on the starting cohort sizes.


## Findings
* The business analysis found that 10.34% of product page views convert to purchases, which is considered a good conversion rate, generally speaking.
* It was also found that retention rates are the highest in the cohort from '2020-09', and remain so for the longest time between all six cohort groups. While looking at the cohort analysis values can make it seem that the '2020-09' cohort has the least amount of conversions, only when you calculate the retention rates can you see what the numbers are really saying.

## Media
![36F989D3-C457-4A15-B026-7D02C9111A04](https://github.com/user-attachments/assets/28cda591-9390-4984-b61b-9a5ecd1dab47)

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

#### For Windows:
* Operating System:
  * Windows 10 (64-bit) or later
  * Windows Server 2016 or later (for server environments)
  * Power BI Desktop does not run on older versions of Windows (Windows 8.1 or lower, Windows 7).
* Processor:
  * A 64-bit processor (x64 architecture)
  * At least 1 GHz or faster, with at least 2 cores (4 cores or more recommended for large datasets)
* Memory (RAM):
  * Minimum 2 GB of RAM (4 GB or more recommended for better performance)
  * 8 GB or more of RAM is recommended for larger data models or complex reports.
* Disk Space:
  * At least 1 GB of free disk space (more may be required depending on data model size)
* Display:
  * A screen resolution of at least 1440 x 900 or higher is recommended for optimal display of data and visuals.
* Graphics:
  * A DirectX 10 compatible graphics card for accelerated rendering. While not strictly required, it improves performance with large visualizations.
* Internet Connection:
  * Required for downloading and installing Power BI Desktop.
  * An internet connection is also required for publishing reports to Power BI Service and for receiving data refresh updates (if applicable).
#### Power BI Service (for Online Use and Collaboration)
To fully utilize Power BI and collaborate with colleagues or stakeholders:
* Browser Compatibility:
  * Latest versions of Google Chrome, Microsoft Edge, Safari, or Mozilla Firefox are supported.
  * Internet Explorer is not recommended for an optimal experience.
* Power BI Service Subscription (Optional):
  * While Power BI Desktop is free, to share and collaborate with others or access more advanced features, you may need a Power BI Pro or Power BI Premium license.
  * The Power BI Pro license offers collaboration, sharing, and additional features, while Power BI Premium offers dedicated cloud resources and increased data model size for enterprise needs.

#### Options for Running Power BI on a Mac
* Using Power BI Service (Web Version):
  * You can use Power BI Service through any modern web browser, including those on macOS (Google Chrome, Safari, or Mozilla Firefox). This allows you to create, view, and interact with reports, dashboards, and data models without needing to install Power BI Desktop.
  * Access Power BI Service: Power BI Service
* Running Power BI Desktop via a Virtual Machine or Windows Environment:
  *Virtualization: You can use virtualization software (such as Parallels Desktop or VMware Fusion) to run a Windows environment on your Mac. With this, you can install and run Power BI Desktop as you would on a Windows machine.
  * Boot Camp: Alternatively, you can set up Boot Camp to dual-boot Windows on your Mac, allowing you to install Power BI Desktop in the Windows partition.
* Using Wine or Crossover (Non-native Solution):
  * Some users have successfully run Power BI Desktop on macOS using Wine or Crossover to simulate a Windows environment. However, this is not officially supported by Microsoft, and there could be performance or stability issues.
#### System Requirements for Power BI Service on macOS (Web Version)
If you're planning to use Power BI Service via a web browser, here are the browser requirements:
#### For Web Browsers on macOS:
* Operating System:
  * macOS 10.13 (High Sierra) or later is recommended to ensure compatibility with the latest versions of web browsers.
* Web Browsers:
  * Google Chrome (recommended)
  * Safari (latest version)
  * Mozilla Firefox (latest version)
  * Microsoft Edge (latest version)
* Internet Connection:
  * A stable internet connection is required to access Power BI Service.
* Display:
  * Minimum resolution of 1280 x 800 pixels for optimal user experience.
* Graphics:
  * A graphics card capable of rendering modern web apps, which is typically built into most recent Mac devices.
#### System Requirements for Running Power BI Desktop on Mac via Virtual Machine or Boot Camp
If you choose to run Power BI Desktop in a Windows environment on your Mac (using Parallels, VMware Fusion, or Boot Camp), here are the basic system requirements for Power BI Desktop running in Windows:

#### For Windows on Mac (via Virtual Machine or Boot Camp):
* Operating System:
  * Windows 10 (64-bit) or later.
  * Windows 7 or 8.1 (64-bit) are supported, but Power BI recommends using Windows 10 for the best performance and compatibility.
* Processor:
  * 1.8 GHz or faster x64-based processor (Intel or AMD).
* Memory:
  * Minimum 4 GB of RAM (8 GB recommended for larger datasets or complex reports).
* Disk Space:
  * At least 1 GB of available disk space for installation (more may be required depending on data models).
* Graphics:
  * A DirectX 10-compatible graphics card or better.
* Display:
  * A screen resolution of 1366 x 768 or higher is recommended.
* Internet Connection:
  * Required for downloading and installing Power BI Desktop and for publishing reports to Power BI Service.
#### Summary:
* Power BI Desktop is not directly supported on macOS, but you can still access Power BI Service (the web version) using any modern browser on macOS.
* If you need Power BI Desktop specifically, you can run it on macOS using a virtual machine, Boot Camp, or emulation software like Wine or Crossover.
* Power BI Service via the browser requires a stable internet connection and a supported browser.

