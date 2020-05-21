# Data Analyst Job Landscape in Singapore for 2020

### Methodology
* [1. Background](#point_1)
* [2. Files in this Repository](#point_2)
* [3. Data Scraping Approach](#point_3)
* [4. Findings](#point_4)
* [5. Conclusions](#point_5)
* [6. Acknowledgement](#point_6)

<a id="point_1"></a>
### 1. Background
As graduation approaches for me, I decided that it would be beneficial to get an overview of the Data centered jobs in Singapore. Therefore, I decided to web scrap the popular job site, Glassdoor, to gather data on the jobs on the market and have the bigger picture of the job market.


<a id="point_2"></a>
### 2. Files in this Repository
The files in this bullet points are ordered in a chronological order of usage for this project.
* "chromedriver": Needed for the webscraping algorithm in the 2nd bullet point
* "glassdoor_scraper.py" : The Glassdoor webscraping algorithm
* "Data Collection.ipynb" : The notebook where we call the webscraping algorithm for the different job titles
* "Various Job Titles CSV Files" : Folder containing the CSV files that we save after the Data Collection step in bullet 3
* "Data Cleaning.ipynb" : The notebook with various cleaning algorithm after the data is collected
* "LICENSE" : MIT license for open source projects
* "README.md" : Documentation of the project

<a id="point_3"></a>
### 3. Data Scraping Approach
I chose Glassdoor as the website to attain my data due to the depth and breadth of companies posted. The anonymity nature of Glassdoor further compelled me to use this website to attain job information as it would mean that the information is less skewed towards any party.
<br> Unfortuantely, Glassdoor do not have any public API avaiable, therefore we needed to scrap the data to collect the information on the postings on the site. I utilised selenium package within Python to scrap the website as Glassdoor renders it webpage with Javascript instead of HTML, therefore, we needed the user input function selenium has to offer.


<a id="point_4"></a>
### 4. Findings


<a id="point_5"></a>
### 4. Conclusions


<a id="point_6"></a>
### 6. Acknowledgement
This project would not have been possible without the resources shared by other Github members. There are 2 notable Github members I would like to thank, they are [Mr Ken Jee](https://github.com/PlayingNumbers) and [Mr Ömer Sakarya](https://github.com/arapfaik).
