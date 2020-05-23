# Data Analyst Job Landscape in Singapore for 2020

## Methodology
* [1. Background](#point_1)
* [2. Usage](#point_2)
* [3. Files in this Repository](#point_3)
* [4. Data Collection Approach](#point_4)
* [5. Findings](#point_5)
* [6. Conclusions](#point_6)
* [7. Acknowledgement](#point_7)

<a id="point_1"></a>
## 1. Background
As graduation approaches for me, I decided that it would be beneficial to get an overview of the Data centered jobs in Singapore. Therefore, I decided to web scrap the popular job site, Glassdoor, to gather data on the jobs on the market and have the bigger picture of the job market.

During the course of the project, I made several key assumptions which I believe should be important to lay out before going into the project.
<br> Key Assumptions:

<a id="point_2"></a>
## 2. Usage
The project is written in a Jupyter Notebook file in the Python Language, for easy viewing of the project sections, I have included a viewer website that contains these Jupyter Notebook. I have split the notebooks into the various overarching task I perform for this project.
* [Part 1. Data Collection](https://nbviewer.jupyter.org/github/jamesgsw/Data-Analyst-Job-Landscape-in-2020/blob/master/Part%201.%20Data%20Collection.ipynb)
* [Part 2. Data Cleaning](https://nbviewer.jupyter.org/github/jamesgsw/Data-Analyst-Job-Landscape-in-2020/blob/master/Part%202.%20Data%20Cleaning.ipynb)
* [Part 3. Data Analysis](https://nbviewer.jupyter.org/github/jamesgsw/Data-Analyst-Job-Landscape-in-2020/blob/master/Part%203.%20Data%20Analysis.ipynb)

<a id="point_3"></a>
## 3. Files in this Repository
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


<a id="point_4"></a>
## 4. Data Collection Approach
I chose Glassdoor as the website to attain my data due to the depth and breadth of companies posted. The anonymity nature of Glassdoor further compelled me to use this website to attain job information as it would mean that the information is less skewed towards any party.
<br> Unfortuantely, Glassdoor do not have any public API avaiable, therefore we needed to scrap the data to collect the information on the postings on the site. I utilised selenium package within Python to scrap the website as Glassdoor renders it webpage with Javascript instead of HTML, therefore, we needed the user input function selenium has to offer.
<br> The data was pulled on the 22nd May 2020.

<a id="point_5"></a>
## 5. Findings
<br>
<h3> 5.1 Minimum Education Level Required </h3>
I found that most jobs posting for data-driven jobs look for hires with Bachelors Degree. However, it can be noted that there's a sizeable numbers of employers looking for masters and PhD level of qualification. There's a sizeable portion of employers who do not specify university level of qualification either as they do not require a university qualification or they omitted the education level in the Job Description.

![Minimum Education Level required](https://user-images.githubusercontent.com/36501392/82721446-bf5ecf80-9cef-11ea-9f57-d48ad5d65426.png)


<h3> 5.2 Technical Skills Requested for Jobs </h3>
As I expected Python was the most requested skillset that employer wanted prospective hires to have, it's closely followed by SQL. Big data platforms such as Apache Spark and Hadoop alongside Scala are relatively high in demand as well.
I was very surprise to see that R was not highly requested in the technology industry but I postulate that R is used greater in academic circles.

![Technical Skills requested for Job](https://user-images.githubusercontent.com/36501392/82721458-cd145500-9cef-11ea-80fe-48f0f39d6865.png)


<h3> 5.3 Academic Skills Requested for Jobs </h3>
Unsurprinsingly, the top academic skill set looked for by employers is Machine Learning with predictive analysis. However other academic skills sets such as DevOps, Statistics and Database Management is actually rarely mention, and Calculus was not mention at all.
I postulate that many employers believe that these skills should be instilled into them during their academic training. Therefore, in the next sub-section, I'll investigate the education level that employers expect.

![Academic Skills requested for Job](https://user-images.githubusercontent.com/36501392/82721464-d3a2cc80-9cef-11ea-8ca8-1f0f14cb75db.png)


<h3> 5.4 Hires by ownership type </h3>
We found that by ownership, the biggest hire of data driven jobs is the private sector. Followed by public companies and government firms. This is not surprising that private and public company are the biggest players, as they are profit driven and would want to capitalise on new technology and skill set that can help to streamline their operations.

![Screenshot 2020-05-23 at 12 32 40](https://user-images.githubusercontent.com/36501392/82721645-8de70380-9cf1-11ea-9747-a1f81a8023db.png)

<h3> 5.5 Job Description Word Cloud </h3>
In the job description, we find that the knowledge in machine learning is the most popular skill that is requested by employers. Other notable skills are data mining, predicitve modeling, data pipline, natural language processing and big data.

![Job Description Word Cloud](https://user-images.githubusercontent.com/36501392/82721433-a9e9a580-9cef-11ea-86df-defbd17b1b34.png)

<a id="point_6"></a>
## 6. Conclusions
Overall, I'm satisfied with the outcome of this project where I was able to fufil my 2 goals of the project and have a better understanding of the Data centric Job Market. However, I would like to note that there are assumptions and limitations to the dataset that I would like to improve for future improvements, where I would like to gather data from Linkedin Jobs as well to increase the sample size of my search.
Thank you for viewing!(:

<a id="point_7"></a>
## 7. Acknowledgement
This project would not have been possible without the resources shared by other Github members. There are 2 notable Github members I would like to thank, they are [Mr Ken Jee](https://github.com/PlayingNumbers) and [Mr Ömer Sakarya](https://github.com/arapfaik).
