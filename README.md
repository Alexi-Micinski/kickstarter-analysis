# Kickstarting with Excel

## Overview of Project
Louise is using the Kickstarter fundraising platform to fund her play *Fever*. Her goal is to raise over $10,000 for her project. Analysis of the Kickstarter data will provide insights into what factors make a project's campaign sucessful. Data analysis will be used to understand campaigns from start to finish and help Louise mirror other successful campaigns. Excel will be used to organize, sort, and analyze the crowdfunding data.

### Purpose
Louise's campaign came close to its goal in a short amount of time. Now she wants to know how it compares to other campaigns. Campaign outcomes will be analyzed and visualized based on launch dates and funding goals. 

## Analysis and Challenges

The Kickstarter data was first downloaded and saved in organized and easy to access folders. The data was then resized, organized, and formatted for the purpose of familiarization. Filters, conditional formatting, and the freeze panes features were also used in getting aquainted with the data. It is important to be familiar with the data before attempting to manipulate or summarize it. 

Next filters were applied and subcategories were parsed out from parent categories in order to create more detailed data for analysis. Louise's project falls under the theater category and plays subcategory. From here summary tables, pivot charts, and graphs were created to summarize the data in a more digestible and readable way. Factors that make a successful campaign can then be more easily interpreted from the summary tables and graphs.![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106785377/179426165-50d31f4d-03d4-4966-8ec5-e54d8b4c9fce.png)


Louise is intersted in campaign oucomes based on launch dates and funraising goals. Campaign outcomes are categorized based on if they were successful, failed, or canceled.

### Analysis of Outcomes Based on Launch Date
First, a new column labeled “Years” was created. The YEAR() fuction was used to extract the year from the “Date Created Conversion” column in the data. 

Next, a pivot table was created in a new tab labeled "Theater Outcomes by Launch Date." The table was set up to allow filters based on parent category and years, and to show successful, failed, and canceled projects based on launch date. The table was filtered to show data for the theater category.

<img width="458" alt="Pivot Table" src="https://user-images.githubusercontent.com/106785377/179426143-4f2a6e0f-ff79-41e5-8d9b-1f7851df6c42.png">

A line chart was then created based on the summary table to show theater outcomes based on launch date. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106785377/179426174-bd401e21-5bad-4301-9a7b-c8bee9fc2b28.png)

The month of May had the most successful campaigns, while June, July, and October all had a similar number of failed campaigns. This can be seen by studying the points on the line chart.

### Analysis of Outcomes Based on Goals


### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
