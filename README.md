# Kickstarting with Excel

## Overview of Project
Louise is using the Kickstarter fundraising platform to fund her play *Fever*. Her goal is to raise over $10,000 for her project. Analysis of the Kickstarter data will provide insights into what factors make a project's campaign sucessful. Data analysis will be used to understand campaigns from start to finish and help Louise mirror other successful campaigns. Excel will be used to organize, sort, and analyze the crowdfunding data.

### Purpose
Louise's campaign came close to its goal in a short amount of time. Now she wants to know how it compares to other campaigns. Campaign outcomes will be analyzed and visualized based on launch dates and funding goals. 

## Analysis and Challenges

The Kickstarter data was first downloaded and saved in organized and easy to access folders. The data was then resized, organized, and formatted for the purpose of familiarization. Filters, conditional formatting, and the freeze panes features were also used in getting aquainted with the data. It is important to be familiar with the data before attempting to manipulate or summarize it. 

Next filters were applied and subcategories were parsed out from parent categories in order to create more detailed data for analysis. Louise's project falls under the theater category and plays subcategory. From here summary tables, pivot charts, and graphs were created to summarize the data in a more digestible and readable way. Factors that make a successful campaign can then be more easily interpreted from the summary tables and graphs.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106785377/179426165-50d31f4d-03d4-4966-8ec5-e54d8b4c9fce.png)

Louise is intersted in campaign oucomes based on launch dates and funraising goals. Campaign outcomes are categorized based on if they were successful, failed, or canceled.

### Analysis of Outcomes Based on Launch Date
First, a new column labeled “Years” was created. The YEAR() fuction was used to extract the year from the “Date Created Conversion” column in the data. 

Next, a pivot table was created in a new tab labeled "Theater Outcomes by Launch Date." The table was set up to allow filters based on parent category and years, and to show successful, failed, and canceled projects based on launch date. The table was filtered to show data for the theater category.

<img width="458" alt="Pivot Table" src="https://user-images.githubusercontent.com/106785377/179426143-4f2a6e0f-ff79-41e5-8d9b-1f7851df6c42.png">

A line chart was then created based on the summary table to show theater outcomes based on launch date. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106785377/179426174-bd401e21-5bad-4301-9a7b-c8bee9fc2b28.png)

The month of May had the most successful campaigns, while June, July, and October all had a similar number of failed campaigns. This can be seen by studying the points on the line chart.

### Analysis of Outcomes Based on Goals
Next, the data was analyzed to visualize the percentage of successful, failed, and canceled plays based on the funding goal amount.

A new sheet labeled “Outcomes Based on Goals” was created. Then headers were created and dollar amount ranges were inserted in order to group projects based on goal amounts. 

<img width="82" alt="Dollar Amount Ranges" src="https://user-images.githubusercontent.com/106785377/179426944-1e577a30-ab93-4fff-8b78-be2e2cec025c.png">

The COUNTIFS() function was used to populate the number of successful, failed, and canceled columns by filtering on the outcome column in the data, the goal amount ranges created in the previous step, and the plays subcategory as the criteria. 

<img width="730" alt="Formula Example" src="https://user-images.githubusercontent.com/106785377/179426993-c65490e4-a66f-4655-b86f-78fb43521f49.png">

The sum function was used to calculate the total number of projects and the percentage was calculated for each row. 

<img width="699" alt="Table Example" src="https://user-images.githubusercontent.com/106785377/179427044-f7ca8078-f762-400d-8b4e-396ee59582d3.png">

Next a line chart was created based on the data to visualize the relationship between the goal-amount ranges and the percentage of successful, failed, or canceled projects.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106785377/179427014-8ade879b-ecec-4edc-8b6c-98673714d5fd.png)

The most successful outcomes based on goal amount, or highest percentage successful, is for goals below 4,999 and between 35,000 and 44,999 dollars.

### Challenges and Difficulties Encountered

No major challenges arose during the analysis of this data. 

One possible challenge that could have occured is getting an error when extracting the year from the “Date Created Conversion” column. The “Date Created Conversion” column was created by converting the launched at date to a readable date. The launched at dates were in unix timestamp format and needed epoch conversion. If this wasn't done correctly, the year would not have been available for extraction. 

Another possible challenge that could have occured is getting incorrect values for the Oucomes Based on Goals chart using the COUNTIFS() formula. This formula can get long and therefore it has many opportunities for errors. The formula that was used required manual input for each of the goal amount ranges. This manual input could've been avoided by using greater than or less than formulas in the table rather than strings. Ie <1000 instead of "less than 1000." This way a cell could've been selected rather than manually entering in the range for each cell. This also would've cut down on time entering the formulas for each cell.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  The month of May is the best month to launch a theater campaign, as it has the highest number of successful campaigns. The month of October is the worst month to launch a theater campaign as it has the highest number of failed campaigns compared to sucessful campaigns.

- What can you conclude about the Outcomes based on Goals?

  The most successful outcomes based on goals for plays are for goals below 4,999 and between 35,000 and 44,999 dollars. Clearly having a low goal is easy to achieve. Above the low goal range though, goals between the ranges including 35,000 to 44,999 dollars seems to be a successful range.

- What are some limitations of this dataset?

  The datasets give direction towards what months and what goals might give succussful or failed campaigns, but they do not explain why or take other factors into account. For example, do theater campaigns tend to fail in October because of the time of year or because those plays happen to also have goals that are too high, etc.

- What are some other possible tables and/or graphs that we could create?

  It would be useful to plot mean goals based on launch date and compare the results to that of outcomes based on launch date. This would give more insight to why campaigns fail in certain months.
