# ZOMATO RESTAURANT ANALYSIS

## Description & Methods
This project was conducted for Zomato, a multinational restaurant aggregator and food delivery company. Its goal was to understand the business performance of restaurants and customers by having analysts choose an area of focus to build a research plan around, conduct the analysis, and deliver conclusions and suggestions. The research area chosen was Restaurant analysis; learning, from the data, things like what restaurants are popular, which generate the highest revenue, and why.
  * After choosing the type of analysis, the first part of the project was to build a plan- deciding on the metrics and parameters for the investigation, how to structure the dashboard, and making a detailed decomposition.
The decomposition included:
    *   Questions: What restaurants are popular? What cuisines are popular? What restaurants generate the highest revenue? Why? What are the most profitable areas or restaurants?
    *   Hypothesis: The most popular and most profitable restaurants will have the biggest number of orders and highest sales amounts.
    *   Visualizations: a heatmap, a bar chart, and a scatterplot.
    *   Dashboard Assembly: The orders and restaurant tables will be combined using an Outer JOIN, specifically a LEFT JOIN through the ID and r_id fields.
  * A heatmap visualization was created with the measures being; the Month of Order Date, State, and Average Profit. After the three best combinations of month and state were determined, a return on ad spend formula was used to tally what Superstore's advertising budget should be. They wanted to spend no more than 1/5th of their profits on advertising.

## Findings
* The two biggest centers for profit and loss, each, and their respective categories were identified as the following: office supplies in California and Technology in New York, Technology in Ohio, and Office Supplies in Texas, respectively.
* An advertising budget was justified by identifying the 3 best combinations of states and months of the year to advertise in: Indiana during October, Vermont during November, and Washington during March. After running a return on ad spend ratio, and Superstore willing to pay 1/5 of advertising profits, respectively, the Superstore should be willing to pay the following: $128.62, $119.20, and $104.26.
* Through data visualization and calculated fields, both the products and customers with the highest return rates were determined. Based on the average profit against the average return rate on a dimension of State, Superstore was recommended for the continuation of business in Vermont as it had the highest ranking within the visualization measures.

## Media
![04C8B086-99C1-4CDA-A5BD-22900EEC8C08](https://github.com/user-attachments/assets/d941308b-5a7e-4a71-bab1-09c23af2a1d4)
[Advertising Chart.pdf](https://github.com/user-attachments/files/18221774/Advertising.Chart.pdf)

[Profits & Losses A.pdf](https://github.com/user-attachments/files/18221781/Profits.Losses.A.pdf)

![9FEA711A-834E-44EE-86A9-70212D56B84C_1_102_o](https://github.com/user-attachments/assets/2dfc81fb-b4d2-4ff9-bc1b-719868d66db4)


## Link to project page
* https://public.tableau.com/views/SuperstoreReturnsAnalysis_17347924139440/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link


## Deployment Instructions & System Requirements
#### Deployment Instructions for Tableau Public

1. Download Tableau Public
* Visit the official Tableau Public download page: Tableau Public Download
* Click the "Download Tableau Public" button to begin the download.

2. Install Tableau Public
* Once the installer has downloaded, locate and double-click the .exe (Windows) or .dmg (Mac) file to start the installation process.
* Follow the on-screen prompts to complete the installation:
  * Windows: Click "Next" to proceed through the setup wizard, and select "Install".
  - Mac: Drag the Tableau Public icon to your "Applications" folder to complete the installation.

3. Launch Tableau Public
* After installation, open Tableau Public by clicking on the desktop icon (or from your Applications folder on Mac).
* The first time you launch Tableau Public, you will be asked to sign in to your Tableau Public account (you can create a free account if you don’t have one).

4. Create and Publish Visualizations
* Once logged in, you can start creating your visualizations by importing your data (Excel, Google Sheets, etc.).
* Design your visualizations using Tableau's drag-and-drop interface.
* After creating your work, click the "File" menu and select "Save to Tableau Public" to upload your visualization to the Tableau Public server for sharing online.


#### System Requirements for Tableau Public
Tableau Public is available for both Windows and Mac, and here are the minimum system requirements for each platform:

#### For Windows:
* Operating System:
  * Windows 10 (64-bit) or Windows 11
  * Windows 8.1 (64-bit) or Windows 7 (64-bit) (Service Pack 1 or higher)
* Processor:
  * At least 1.5 GHz or higher (dual-core or better recommended)
* RAM:
  * Minimum 2 GB (4 GB or more recommended for better performance)
* Disk Space:
  * At least 1.5 GB of free disk space
* Display:
  * Resolution of 1366 x 768 or higher
* Graphics:
  * A compatible graphics card with support for OpenGL 3.2 or later
* Internet Connection:
  * Required for downloading Tableau Public and for saving visualizations to Tableau Public's online platform.

#### For Mac:
* Operating System:
  *macOS 10.15 (Catalina) or later
* Processor:
  * Intel Core i3 (or better) processor
* RAM:
  * Minimum 4 GB (8 GB or more recommended for optimal performance)
* Disk Space:
  * At least 1.5 GB of free disk space
* Display:
  * Resolution of 1280 x 800 or higher
* Graphics:
  * A compatible graphics card with support for OpenGL 3.2 or later
* Internet Connection:
  * Required for downloading Tableau Public and saving work to the cloud.
