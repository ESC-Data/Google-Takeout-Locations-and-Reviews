# 📱 Google Takeout: Applications and Devices
This repository contains:  
- 📜 Script for processing Google Takeout Datasets.
- 📊 PBI Dashboard, a detailed and customized report to uncover deep insights from your Locations and Reviews Data.

## About the project
Google stores extensive information about the devices where our accounts have been logged in. This information is accessible to us through a Google portal. In this project, we will leverage this data to verify the applications installed on all devices associated with our accounts. This will enable us to identify if our account has been cloned or accessed from an unknown device.

## About the Script and Data Sources
The code will read and transform six json files exported fron your Google Account data.
- 📱 **Reviews**: The Reviews JSON file in your Google Takeout data contains detailed information about the reviews you've left on various platforms and locations. This includes details such as: review content, review date, location information, review star rating.

## About the PBI Dashboards

The Power BI dashboard 📊 offers an intuitive view of key correlations within your Google Takeout data. Easily analyze extensive review information to identify standout locations 🌟, those generating the highest customer satisfaction 😊, and locations that need improvements 🏢. Leveraging sentiment analysis 😊 and review data 📈, this dashboard highlights areas for optimization and growth, ensuring your locations receive the attention they deserve for maximum impact 🚀.

As an initial insight, you can the filter the top-performing locations 📈 on the bottom table, you can quickly reveal lcations that have an average rating below 4.5 ⭐, which is the benchmark for maintaining a good reputation and competitiveness. Using the dashboard, you can perform sentiment analysis 😊 and take action to address this crucial issue. By improving ratings, your business becomes more favorable to customers and enhances its positioning 📍🚀.

Understanding and analyzing competitors' reviews is also key 🔑. This dashboard provides insights into their weaknesses and strengths, helping your business to differentiate itself. Measuring, understanding, and maintaining this indicator is crucial for the success of any location 🏢 and, consequently, the company 📈.
![Google Reviews](https://github.com/user-attachments/assets/39850d3b-afb6-4eca-93bb-cb3da22177b2)


## About ESC Data
With over 10 years of experience in e-commerce, 🌟 ESC Data 🌟 stands out in the market by focusing on optimizing results. Through data-driven strategies, we deliver simple, effective, and creative solutions for your company or brand. 🚀 Boost your online presence and sales with our listing optimization, Amazon advertising, and data analytics. Visit us at https://www.esc-data.com/projects for more details! 📈

## Procedure to Follow

**Request Data from Google**: First, we need to request Google to return the information stored about us. To do this, open your preferred browser and navigate to Google Takeout. On this page, select the "Google Play" option.
After that, choose how often you want to download the data. For this case, select "Export once". Also, choose how you want the data to be delivered. The best option is to keep the default setting: "Send download link via email". After a few hours (or days), you will receive a download link in your Gmail inbox, from which you can download the .zip file.

**Extract the Data**: Once the .zip file is downloaded, unzip the data and save it in a folder, for example, D:\project\. For now, keep the files in that location.

**Transform the Data from JSON to CSV Format**: In the GitHub repository for this project, there is a Python script file that we need to execute to transform the data into CSV format. Download it and run it, replacing the FILE PATH variable by the file path of the flder that you cretaed on the previous step. After running the Python file, you will see a new CSV file has been created.
****Note****: To execute the Python file, you need to have Python installed on your computer and the Pandas library. 

**Import the Data to PowerBI**: Next, go to the GitHub repository again and download the .pbix file and the date.csv file into the same directory where the new files were created.
Open the PowerBI file and from the main menu, select "Transform Data". This option will open a new window. This window contains the transformations applied to the files to fit the report's data model. However, you need to modify the file path for these files. To do this efficiently, change the value of the "Folder" parameter to the directory where your CSV files are stored.

**Update the Data**: Finally, in PowerBI, refresh the data, and in the visualizations, you will be able to see the applications installed on your various devices.


