# ZOMATO RESTAURANT ANALYSIS

## Description & Methods
This project was conducted for Zomato, a multinational restaurant aggregator and food delivery company. Its goal was to understand the business performance of restaurants and customers by having analysts choose an area of focus to build a research plan around, conduct the analysis, and deliver conclusions and suggestions. The research area chosen was Restaurant analysis; learning, from the data, things like what restaurants are popular, which generate the highest revenue, and why.
  * After choosing the type of analysis, the first part of the project was to build a plan- deciding on the metrics and parameters for the investigation, how to structure the dashboard, and making a detailed decomposition.
The decomposition included:
    *   Questions: What restaurants are popular? What cuisines are popular? What restaurants generate the highest revenue? Why? What are the most profitable areas or restaurants?
    *   Hypothesis: The most popular and most profitable restaurants will have the biggest number of orders and highest sales amounts.
    *   Visualizations: a bubble map, a bar chart, and a scatterplot.
    *   Dashboard Assembly: The orders and restaurant tables will be combined using an Outer JOIN, specifically a LEFT JOIN through the ID and r_id fields.
  * Once the plan was completed, the construction of the visualizations and dashboard was next.
    * The first is a bubble map, created based on the sum of the sales quantity of each restaurant.
    * The second is a simple bar chart that compares the sales amount of each restaurant.
    * The last is a scatter plot that factors in the number of orders versus the sales amount($) of the restaurants.
  * Finally, the dashboard assembled contains all three visualizations that adjust to each others' filtered settings. The dashboard shows the bigger picture within the data as well as any specifics within.

## Findings
* Fast food chains are bringing in the most in sales and customer orders. The visualization helps us see that American food chains take up four of the top five highest restaurants in order quantities. This visualization also helps us see that fast-food clients most likely require more of Zomato's resources and services.
* More orders do not mean more in sales. It is important to note that sales amount and order quantity do not always have a positive correlation...let’s look at the restaurant Huber & Holly. With only 13 orders they amassed over $1.6M. Price ranges and restaurant class have a great impact on these correlations. 
Strategically speaking, restaurants with a negative correlation, specifically like this one, would be the best clients to have for Zomato. More profits with less resources utilized. But that would be dependent on the business structure Zomato has with each client.
* Domino's Pizza was the highest in both order quantity and total sales. From the bar chart, we learn that Domino's Pizza brings in the most sales, by far, in comparison to the rest of the restaurants that Zomato aggregates. However, this is only clear when looking at the SUM of the sales amount for all four years. The restaurant with the highest sales amount varies through the years since data is missing from the years of 2017 and 2020. It is interesting that not only the restaurant is popular but the simplistic cuisine seems to be favored by customers. This reiterates that American food chains are Zomato's most in-demand clientele.

  Recommendations
 * Zomato should focus more resources on Italian fast-food restaurants, specifically pizza cuisine.
 * Zomato should take inventory of the lowest-performing restaurants and decide if it is in the company's best interest to keep servicing them.
 * Zomato should invest in higher priced restaurants that make more profit from fewer orders, meaning more revenue while deploying less of the resources.

## Media
![0E38269F-7DB9-4784-A463-1691594E75E9_1_105_c](https://github.com/user-attachments/assets/687e6d9e-168c-4b43-a65d-d91db1637bcc)

![A8496B02-7A3B-409A-8CAD-00A4AA7A6669_1_105_c](https://github.com/user-attachments/assets/2a0b41b8-d621-4789-9b47-195ff39723af)


![F9AAB98E-3CCB-49B7-B996-9CE6C1C1F2C5](https://github.com/user-attachments/assets/1bce44b1-8ea1-45bc-847c-9b98b3299315)

[Dashboard 1.pdf](https://github.com/user-attachments/files/18232439/Dashboard.1.pdf)



## Link to project page
* [https://public.tableau.com/views/SuperstoreReturnsAnalysis_17347924139440/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link](https://public.tableau.com/views/ZomatoRestaurantAnalysis_17347925757390/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)


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
