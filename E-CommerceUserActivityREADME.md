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
* https://docs.google.com/spreadsheets/d/1zCk-BiFZGvS8r3g2QGe8Qj6i8srMiEok37ZqbSnf2uY/edit?usp=sharing

## Deployment Instructions & System Requirements
#### Deployment Instructions for Google Sheets
* Access Google Sheets
  * Via Web Browser: Google Sheets is a cloud-based application, so there’s no need to install software. You can access it directly through your web browser by visiting the following link:
   * Google Sheets
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
