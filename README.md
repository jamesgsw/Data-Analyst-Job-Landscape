modellingavailable# Data Analyst Job Landscape in Singapore for 2020

## Methodology
* [1. Background](#point_1)
* [2. Usage](#point_2)
* [3. Data Collection Approach](#point_3)
* [4. Findings](#point_4)
  * [4.1 Number of Job Listings per Job Title](#point_4_1)
  * [4.2 Minimum Education Level Required](#point_4_2)
  * [4.3 Technical Skills Requested for Jobs](#point_4_3)
  * [4.4 Academic Skills Requested for Jobs](#point_4_4)
  * [4.5 Hires by ownership type](#point_4_5)
  * [4.6 Job Demand by Industry](#point_4_6)
  * [4.7 Job Description Word Cloud](#point_4_7)
* [5. Conclusions](#point_5)
* [6. Acknowledgement](#point_6)
* [7. Files in this Repository](#point_7)


<a id="point_1"></a>
## 1. Background
As graduation approaches, I decided that it would help to get an overview of the Data centric jobs in Singapore. Therefore, I decided to web scrap the popular job site, Glassdoor, to gather data on the jobs on the market and have the bigger picture of the job market.


<a id="point_2"></a>
## 2. Usage
The project is written in a Jupyter Notebook file in the Python Language, for easy viewing of the project sections, I have included a viewer website that contains these Jupyter Notebook. I have split the notebooks into the various overarching task I perform for this project.
* [Part 1. Data Collection](https://nbviewer.jupyter.org/github/jamesgsw/Data-Analyst-Job-Landscape-in-2020/blob/master/Part%201.%20Data%20Collection.ipynb)
* [Part 2. Data Cleaning](https://nbviewer.jupyter.org/github/jamesgsw/Data-Analyst-Job-Landscape-in-2020/blob/master/Part%202.%20Data%20Cleaning.ipynb)
* [Part 3. Data Analysis](https://nbviewer.jupyter.org/github/jamesgsw/Exploring-the-Big-Data-and-Analytics-Job-Market-in-Singapore-2020/blob/master/Part%203.%20Data%20Analysis.ipynb)


<a id="point_3"></a>
## 3. Data Collection Approach
I chose Glassdoor as the website to attain my data due to the depth and breadth of companies posted. The anonymity nature of Glassdoor further compelled me to use this website to attain job information as it would mean that the information is less skewed towards any party.
<br> Unfortunately, Glassdoor do not have any public API available, therefore we needed to scrap the data to collect the information on the postings on the site. I utilised selenium package within Python to scrap the website as Glassdoor renders it webpage with Javascript instead of HTML, therefore, we needed the user input function selenium has to offer.
<br> The data was pulled on the 22nd May 2020.


<a id="point_4"></a>
## 4. Findings
<br>

<a id="point_4_1"></a>
<h3> 4.1 Number of Job Listings per Job Title </h3>
I wanted to find out the number of job listings for the different Job title that were related to the keywords used in the data collection process. We found that there's the job listings for Data Scientist, followed by Data Analyst, Data Engineer, Manager, Machine Learning Engineer, and finally, Director.

| Job Title	| Number of Jobs |	Relative Frequency, % |
| :---: | :---: | :---: |
| Data Scientist	| 925	| 45.00 |
| Data Analyst	| 477	| 23.00 |
| Data Engineer	| 440	| 21.000 |
| Manager	| 129	| 6.00 |
| Machine Learning Engineer	| 61	| 3.00 |
| Director	| 17 |	1.00 |

![Number of Jobs listed on Glassdoor](https://user-images.githubusercontent.com/36501392/84592079-6f4dd580-ae75-11ea-8235-83ef6543ef2e.png)

<a id="point_4_2"></a>
<h3> 4.2 Minimum Education Level Required </h3>
I found that most jobs posting for data-driven jobs look for hires with Bachelors Degree. However, it can be noted that there's a sizeable numbers of employers looking for masters and PhD level of qualification. There's a sizeable portion of employers who do not specify university level of qualification either as they do not require a university qualification or they omitted the education level in the Job Description.

|Education Level |	Frequency	| Relative Frequency, % |
| :---: | :---: | :---:|
|Bachelors Degree	| 1035 |	51.00 |
|Masters	| 232	| 11.00 |
|PhD	| 299	| 15.00 |
|No Education Specified	| 299	| 15.00 |

![Minimum Education Level required](https://user-images.githubusercontent.com/36501392/82721446-bf5ecf80-9cef-11ea-9f57-d48ad5d65426.png)

<a id="point_4_3"></a>
<h3> 4.3 Technical Skills Requested for Jobs </h3>
As I expected Python was the most requested skillset that employer wanted prospective hires to have, it's closely followed by SQL. Big data platforms such as Apache Spark and Hadoop alongside Scala are relatively high in demand as well.
I was very surprise to see that R was not highly requested in the technology industry but I postulate that R is used greater in academic circles.

| Technical Skills |	Frequency	| Relative Frequency, % |
| :---: | :---: | :---:|
| AWS	| 328	| 16.00 |
| Excel	| 763	| 37.00 |
| Python | 1351	| 66.00 |
| R	| 159	| 8.00 |
| Spark	| 629	| 31.00 |
| Hadoop | 531	| 26.00 |
| Scala	| 509	| 25.00 |
| SQL	| 1193	| 58.00 |

![Technical Skills requested for Job](https://user-images.githubusercontent.com/36501392/82721458-cd145500-9cef-11ea-80fe-48f0f39d6865.png)

<a id="point_4_4"></a>
<h3> 4.4 Academic Skills Requested for Jobs </h3>
Unsurprisingly, the top academic skill set looked for by employers is Machine Learning with predictive analysis. However other academic skills sets such as DevOps, Statistics and Database Management is actually rarely mention, and Calculus was not mention at all.
I postulate that many employers believe that these skills should be instilled into them during their academic training. Therefore, in the next sub-section, I'll investigate the education level that employers expect.

![Academic Skills requested for Job](https://user-images.githubusercontent.com/36501392/82721464-d3a2cc80-9cef-11ea-8ca8-1f0f14cb75db.png)

<a id="point_4_5"></a>
<h3> 4.5 Hires by ownership type </h3>
We found that by ownership, the biggest hire of data driven jobs is the private sector. Followed by public companies and government firms. This is not surprising that private and public company are the biggest players, as they are profit driven and would want to capitalise on new technology and skill set that can help to streamline their operations.

| Ownership	| Number of Jobs	| Relative Frequency, % |
| :---: | :---: | :---: |
| Company - Private |	815	| 40.00 |
| Company - Public	| 503	| 25.00 |
| Government	| 258	| 13.00 |
|Subsidiary or Business Segment	| 33	| 2.00 |
| College / University	| 16	| 1.00 |
| Contract	| 9	| 0.00 |
| Unknown	| 9	| 0.00 |

![Screenshot 2020-05-23 at 12 32 40](https://user-images.githubusercontent.com/36501392/82721645-8de70380-9cf1-11ea-9747-a1f81a8023db.png)

<a id="point_4_6"></a>
<h3> 4.6 Job Demand by Industry </h3>
We found that the largest listings per industry is the government agencies, followed by internet companies and banking industry. However, it's important to note that we grouped the entire government agencies and its subsidiary as a single industry. Therefore, this might partially explain this large percentage of the job listings.
![Job demand by Industry](https://user-images.githubusercontent.com/36501392/84592963-e1291d80-ae7b-11ea-8ad6-70a09ba0af2e.png)

<a id="point_4_7"></a>
<h3> 4.7 Job Description Word Cloud </h3>
In the job description, we find that the knowledge in machine learning is the most popular skill that is requested by employers. Other notable skills are data mining, predictive modeling, data pipeline, natural language processing and big data.

![Job Description Word Cloud](https://user-images.githubusercontent.com/36501392/82721433-a9e9a580-9cef-11ea-86df-defbd17b1b34.png)


<a id="point_5"></a>
## 5. Conclusions
Overall, I'm satisfied with the outcome of this project where I was able to fulfil my 2 goals of the project and have a better understanding of the Data centric Job Market. However, I would like to note that there are assumptions and limitations to the dataset that I would like to improve for future improvements, where I would like to gather data from Linkedin Jobs as well to increase the sample size of my search.
Thank you for viewing!(:


<a id="point_6"></a>
## 6. Acknowledgement
This project would not have been possible without the resources shared by other Github members. There are 2 notable Github members I would like to thank, they are [Mr Ken Jee](https://github.com/PlayingNumbers) and [Mr Ömer Sakarya](https://github.com/arapfaik).


<a id="point_7"></a>
## 7. Files in this Repository
The files in this bullet points are ordered in a chronological order of usage for this project.
* "chromedriver": Needed for the webscraping algorithm in the 2nd bullet point
* "glassdoor_scraper.py" : The Glassdoor webscraping algorithm in Python
* "Part 1. Data Collection.ipynb" : The notebook where we call the webscraping algorithm for the different job titles
* "Part 2. Data Cleaning.ipynb" : The notebook with various cleaning algorithm after the data is collected
* "Part 3. Data Analysis.ipynb" :
* "Various Job Titles CSV Files" Folder : Folder containing the CSV files that we save after the Data Collection step in bullet 3
* "Various Graphical Visualisation" Folder : Folder containing the various Data Visulisation plots created during the Part 3. Data Analysis in .png format.
* "LICENSE" : MIT license for open source projects
* "README.md" : Documentation of the project
