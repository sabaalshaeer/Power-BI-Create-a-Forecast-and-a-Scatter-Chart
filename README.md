# Power-BI-Create-a-Forecast-and-a-Scatter-Chart
Exercise 1: Create the Report
In this exercise you will create the Sales Exploration report.

Task 1: Get started – Sign in
In this task you will setup the environment for the lab by signing in to Power BI.

Important: If you have already signed in to Power BI in a previous lab, continue from the next task.

To open Microsoft Edge, on the taskbar, click the Microsoft Edge program shortcut.

Picture 7

In the Microsoft Edge browser window, navigate to https://powerbi.microsoft.com.

Tip: You can also use the Power BI Service favorite on the Microsoft Edge favorites bar.

Click Sign In (located at the top-right corner).

Picture 5

Enter the account details provided to you.

If prompted to update the password, reenter the provided password, and then enter and confirm a new password.

Important: Be sure to record your new password.

Complete the sign in process.

If prompted by Microsoft Edge to stay signed in, click Yes.

In the Microsoft Edge browser window, in the Power BI service, in the Navigation pane, expand My Workspace.

Picture 4

Leave the Microsoft Edge browser window open.

Task 2: Get started – Create a dataset
In this task you will setup the environment for the lab by creating a dataset.

Important: If you have already published the dataset in the Create a Power BI Dashboard lab, continue from the next task.

In the Microsoft Edge browser window, in the Power BI service, in the Navigation pane, at the bottom, click Get Data.

Picture 8

In the Files tile, click Get.

Picture 10

Click the Local File tile.

Picture 11

In the Open window, navigate to the D:\PL300\Labs\08-create-power-bi-dashboard\Solution folder.

Select the Sales Analysis.pbix file, and then click Open.

If prompted to replace the dataset, click Replace it.

Task 3: Create the report
In this task you will create the Sales Exploration report.

To open the Power BI Desktop, on the taskbar, click the Microsoft Power BI Desktop shortcut.

Important: If you already have Power BI Desktop open (from a previous lab), close that instance.

Picture 14

To close the getting started window, at the top-left of the window, click X.

Picture 13

If Power BI Desktop is not signed in to the Power BI service, at the top-right, click Sign In.

Picture 16

Complete the sign in process using the same account used to sign in to the Power BI service.

To save the file, click the File ribbon tab to open the backstage view.

Select Save.

Picture 12

In the Save As window, navigate to the D:\PL300\MySolution folder.

In the File Name box, enter Sales Exploration and click Save.

Picture 1

To create a live connection to the Sales Analysis dataset, on the Home ribbon tab, from inside the Data group, click Power BI Datasets.

Picture 15

In the Select a Dataset to Create a Report window, select the Sales Analysis dataset.

Click Create.

Picture 17

Save the Power BI Desktop file.

You’ll now create two report pages, and on each page you’ll work with a different visual to analyze and explore data.

Exercise 2: Create a Scatter Chart
In this exercise you will create a scatter chart that can be animated.

Task 1: Create an animated scatter chart
In this task you will create a scatter chart that can be animated.

Rename Page 1 as Scatter Chart.

Picture 67

Add a Scatter Chart visual to the report page, and then position and resize it so it fills the entire page.

Picture 18

Picture 75

Add the following fields to the visual wells/areas:

The labs use a shorthand notation to reference a field. It will look like this: Reseller | Business Type. In this example, Reseller is the table name and Business Type is the field name.

X Axis: Sales | Sales

Y Axis: Sales | Profit Margin

Legend: Reseller | Business Type

Size: Sales | Quantity

Play Axis: Date | Quarter

Picture 39

The chart can be animated when a field is added to the Play Axis well/area.

In the Filters pane, add the Product | Category field to the Filters On This Page well/area.

In the filter card, filter by Bikes.

Picture 40

To animate the chart, at the bottom left corner, click Play.

Picture 41

Watch the entire animation cycle from FY2018 Q1 to FY2020 Q4.

The scatter chart allows understanding the measure values simultaneously: in this case, order quantity, sales revenue, and profit margin.

Each bubble represents a reseller business type. Changes in the bubble size reflect increased or decreased order quantities. While horizontal movements represent increases/decreases in sales revenue, and vertical movements represent increases/decreases in profitability.

When the animation stops, click one of the bubbles to reveal its tracking over time.

Hover the cursor over any bubble to reveal a tooltip describing the measure values for the reseller type at that point in time.

In the Filters pane, filter by Clothing only, and notice that it produces a very different result.

Save the Power BI Desktop file.

Exercise 3: Create a Forecast
In this exercise you will create a forecast to determine possible future sales revenue.

Task 1: Create a forecast
In this task you will create a forecast to determine possible future sales revenue.

Add a new page, and then rename the page to Forecast.

Picture 66

Add a Line Chart visual to the report page, and then position and resize it so it fills the entire page.

Picture 19

Picture 74

Add the following fields to the visual wells/areas:

X-axis: Date | Date

Y-axis: Sales | Sales

Picture 46

In the Filters pane, add the Date | Year field to the Filters On This Page well/area.

In the filter card, filter by two years: FY2019 and FY2020.

Picture 47

When forecasting over a time line, you will need at least two cycles (years) of data to produce an accurate and stable forecast.

Add also the Product | Category field to the Filters On This Page well/area, and filter by Bikes.

Picture 48

To add a forecast, beneath the Visualizations pane, select the Analytics pane.

Picture 20

Expand the Forecast section.

If the Forecast section is not available, it’s probably because the visual hasn’t been correctly configured. Forecasting is only available when two conditions are met: the axis has a single field of type date, and there’s only one value field.

Turn the Forecast option to On.

Picture 51

Configure the following forecast properties:

Units: Months

Forecast length: 1 month

Seasonality: 365

Confidence interval: 80%

Click Apply.

Picture 52

In the line visual, notice that the forecast has extended one month beyond the history data.

The gray area represents the confidence. The wider the confidence, the less stable—and therefore the less accurate—the forecast is likely to be.

When you know the length of the cycle, in this case annual, you should enter the seasonality points. Sometimes it could be weekly (7), or monthly (30).

In the Filters pane, filter by Clothing only, and notice that it produces a different result.

Save the Power BI Desktop file.

Task 2: Finish up
In this task you will complete the lab.

Select the Scatter Chart page.

Save the Power BI Desktop file.

To publish the file to your My workspace, on the Home ribbon tab, from inside the Share group, click Publish and then click Select to publish.

Picture 23
