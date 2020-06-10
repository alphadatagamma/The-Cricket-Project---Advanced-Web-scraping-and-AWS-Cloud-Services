# The Cricket project
Cricket is a religion in India and I am a big fan of the sport. A game with more than a Billion fans worldwide and a global industry worth more than 100s of Billions of dollars.

This love for the game and the determination to apply some my Data Science skills has led to the inception of this project.

<b>Phase 1</b>: Web scraping data from various sources like ICC.com ESPN Cricinfo, CricBuzz.com (Python, Beautiful Soup, RegEx, and AWS EC2)

<b>Phase 2</b>: Data Processing and Cleaning and storing as comma separated in AWS S3

<b>Phase 3</b>: Setting up ETL jobs to create Relational database using AWS Glue and AWS Redshift


### Phase 1.  Webscraping
Webscraping scripts for The Cricket Project

## The following data sources are webscraped

1. https://www.icc-cricket.com/ - Mens cricket Test, ODI and T-20 Team rankings
2. https://www.icc-cricket.com/ - Mens cricket Test, ODI and T-20 Player rankings
3. https://www.espncricinfo.com/ - Player id, name and country details for all capped players, and their capping date and opposition
4. https://www.espncricinfo.com/ - For all the capped players(5740), we need details such as full name, their Date Of Birth, Place of Birth style of batting or bowling, whether the keep wickets, the role in the team(Bat/Bowl/All-rounder). Getting this data was particularly tricky as I had to extract each attribute separately, and combine it as a row of data for each player. The web scraping script runs for each player in the Capped players dataset to extract the attributes one by one. Doing it on the local machine takes a lot of time, so tried out various things : I tried using the Python 

- <b>AWS EC2, AWS- Sagemaker, Google Colab, Data Bricks</b> and noted the time for scraping 100 records. We will go with whatever wins. Also, will try to implement parallel processing to reduce runtime. - Multipurpose in python doen't seem to work

* My local system with 16 Gigs of RAM, scraps 50 records in 36 seconds
* Google colab with CPU runs it in 58 seconds
* Google colab with GPU runs it in 24 seconds
* Google colab with TPU runs it in 37 seconds, although we did achieve a significant reducction in runtime with GPU, but I was hoping for a 10X decrease. 

5. https://www.espncricinfo.com/



