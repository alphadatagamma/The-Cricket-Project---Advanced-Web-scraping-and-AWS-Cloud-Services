# The-Cricket-Project---Webscraping
Webscraping scripts for The Cricket Project

## The following data sources are webscraped

1. https://www.icc-cricket.com/ - Mens cricket Test, ODI and T-20 Team rankings
2. https://www.icc-cricket.com/ - Mens cricket Test, ODI and T-20 Player rankings
3. https://www.espncricinfo.com/ - Player id, name and country details for all capped players, and their capping date and opposition
4. https://www.espncricinfo.com/ - For all the capped players(5740), we need details such as full name, their Date Of Birth, Place of Birth style of batting or bowling, whether the keep wickets, the role in the team(Bat/Bowl/All-rounder). Getting this data was particularly tricky as I had to extract each attribute separately, and combine it as a row of data for each player. The web scraping script runs for each player in the Capped players dataset to extract the attributes one by one. Doing it on the local machine takes a lot of time, so tried out four things - AWS EC2, AWS- Sagemaker, Google Colab, Data Bricks and noted the time for scraping 100 records. We will go with whatever wins. Also, will try to implement parallel processing to reduce runtime.
5. https://www.espncricinfo.com/



