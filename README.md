# Survey Results Sheet - Project 3

### Check out the live website: <a href="https://survey-results-sheet.onrender.com/">Survey Website</a>

<hr>

<img src="images/amIresponsive.png">

<hr>

## 1. Project Overview
<hr>

### 1.1 Objective

<hr>

The primary objective of the project is to utilize the power of Python modules to manipulate user data for a respective customer and output this data into clear and usable information.

The end-user can then glean important insights from the results of their survey and positively calculate, plan and react in a more efficient manner.
<hr>

### 1.2 User Stories

<hr>

#### First time users:

* As a first time user I want an excellent visual experience
* As a first time user I want to quickly understand what the site is about.
* As a first time user I want easily manipulate sight data for clarity.
* As a first time user I want the ability to easily navigate the site.
* As a first time user I want to easily distingish this site as a trusted site which is safe to use.

#### Returning Users:

* As a returning user I would like to see regular updates.
* As a returning user I would like to download data information.
* As a returing user I would like to learn more about the subject matter.

### 1.3 Design

This site is using a combination of the Python libraries gspread, pandas, and streamlit to connect to a Google Sheets document, retrieve data from it, and then create a web page for displaying that data using visualizations. 

The web page configuration is set using streamlit and the visualizations are created using plotly.express. This negated the need for an index.html, css file, and other codes normally attributed to interact web design.

The data is also filtered based on user input using streamlit widgets, and then the filtered data is used to create additional visualizations using plotly.express. Finally, the resulting web page is served using streamlit. A massive undertaking!
<hr>

<img src="images/survey.png">
<img src="images/MidSection_Spreadsheet.png">

<hr>
## 2 Features
<hr>

The website consists of a single page with several sections. The first section includes a header and subheader, displayed at the top of the page. The page also includes a 3D scatter plot, which is created using data from a Google Sheets document and displayed using the plotly.express library. 

<img src="images/3dPlotter.png">
This 3D plot element retrieves information from a google cloud spreadsheet, found at the following address: bit.ly/3VItB0A

This document will also be used for future iterations of the project, which will be explained later within this document.

Below the scatter plot, there is a section which includes information about the total number of participants in the data and the most popular rating from the data. 

<img src="images/Data_analysis_results.png">
Within this area is an orange slider, with which the end-user can edit the results of the survey to his/her liking. There is functionality within the code that allows for the dynamic altering of the bar graph data below it.

<img src="images/Votes_to_Ratings.png">
Within this widget, as well as all others within the website, the user is able to download site data in several formats, including image format.

The website text is created using streamlit's st.markdown function. There are also several streamlit widgets on the page, including a slider and a multiselect widget, which allow the user to filter the data displayed on the page. 

<img src="images/PieChart.png" alt="pie chart">
The filtered data is then used to create additional visualizations, including a bar chart and a pie chart, using plotly.express. These visualizations are displayed below the widgets. Overall the website is designed to allow users to explore and analyze data from Google Sheets document through interactive visualizations.