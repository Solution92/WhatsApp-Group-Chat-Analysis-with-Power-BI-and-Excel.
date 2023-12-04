# WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel.

## Table of Content
- [Project Objective](#project-objective)
- [Dirty Dataset!](#dirty-dataset)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Stage 1: Extracting Data](#stage-1-extracting-data)
- [Stage 2: Data Pre-cleaning](#stage-2-data-pre-cleaning)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Stage 4:The Power BI Magic](#stage-4-the-power-bi-magic)
- [Power Query Editor Process](#power-query-editor-process)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Individual Reports](#individual-reports)
- [Dashboard](#dashboard)
- [Final Recommendation](#final-recommendation)
- [Limitation](#limitation)
- [Reference](#reference)
  

### Project Objective

To learn and expand knowledge without limitation.

I am really excited to have discovered Data Analytics as a career. “Data is Everywhere”, according to Google Data Analytics Foundation Course.

WhatsApp has been a unique tool for end-to-end encryption and communication for both individuals and businesses. It will be difficult to believe that you can actually extract, Transform, Analyze, and Visualize all chart communication in your group.

Are mine right?

I saw that question in an interview and was shocked to the bone.

The question was “How can you Visualize your WhatsApp group chat?”

I must appreciate Egemolu Goodnews on Medium and LinkedIn. It was his information that inspired my further insights when I saw that question. Thanks, man, and more expansion.

As a Data Analyst, if you hear that question what will you answer and how will you handle it especially if you have not experienced it before?

#### Dirty Dataset!

Have you seen a dirty Dataset before? If No, then, follow me, I will show you one soon.

In this process, I am going to try as much as I can to be a little more detailed with screenshots so we can understand.


### Data Source

From my data Analysis WhatsApp group chart - The Data Musketeers

### Tools Used

Microsoft Excel and Poer BI

### Stage 1: Extracting Data

The first thing is to collect the data from your WhatsApp group chat. From your phone please, NOT computer, open the group chat, click on the three dots on the top right then click “More >”.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/d39c5fc8-5480-4722-b666-effa1ec52ca8)

Next, click on “Export chat” then select “Without media” then select Send Email.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/830a7d53-dafa-4c94-96a6-dddc75d7d935)

Send it to your own email address. At this point, you can switch to your computer.

![2](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/8b81c83d-919d-48b3-b58a-bf3e7f9d315a)

Now, go back to your email address and download it as a .txt file.

Next, copy it to your Notepad, it will look very, very dirty this… see Screenshot>

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/9d83be4e-5458-46aa-91f3-6be565795adf)

This is a practical example of a dirty Dataset.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/9a012072-fe6e-46a1-bc74-2c4a9b0aa811)

At this point this Dataset is ‘useless’, so we must clean it up before anything else.

### Stage 2: Data Pre-cleaning

This stage is one of the most difficult stages most Analysts don’t like. But you don’t have to like it, you must pass through the process.

Take a look at the screenshot, what did you see? A lot of inconsistent punctuation- comma, dash, colon, semicolon, full stop, and so on. On the notepad, I will use the “Replace” tab from the “Edit” tab, to do some cleaning. Replace comma (,) with a semicolon, replace dash (-) with a semicolon, etc., one after the other.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/5de964cd-dee2-46d5-9827-a5023a3ca3fb)

This process needs a lot of patience and attention to detail.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/7d79d9ca-a93b-446d-8c1b-1321d59309df)
Can you note the differences?

### Data Cleaning and Preparation

#### Stage 3: Excel — Import to Excel Sheet

This time we are going to import the .txt file to our Excel for further cleaning and transformation.

Open a new Excel sheet and click on the “Data” tab, click on “From Text” then select the .txt file from your computer where you saved it.

![Screenshot_121](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/7ab4f38a-63b4-4fe9-b636-522f5ab83111)

The window pops shows “Text Import Wizard — Step 1 of 3”

Check the “Delimited” box and click “Next” towards the down right hand.

![Screenshot_122](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/7b617dd6-afe9-45d1-bd9e-c78333fd7a05)

In the next step 2 of 3, under the “Delimiters”, uncheck the “Tab” box and check the “Semicolon” then click “Next”

![Screenshot_123](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/06615a2c-72b6-48b1-8db8-9f6f12a508a0)

Select a Date format from the “Date” drop-down arrow Select “MDY” — “Month, Day, Year” format. Then click on “Finish”.

![Screenshot_124](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/bd8d916e-1691-4725-beb8-99268dd0183e)

In the next box that appears click on “Ok”

As you can see, the Data is still very much dirty. No Column header title. It has about 16 Columns and 1047 rows.

![Screenshot_125](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/dbc63a30-007e-46b1-8861-11ab9d265617)

Now, Name the Title of the Column as follows: Date, Time, Time 1, User, Message, Message 1, Message 2, etc. But as you can see there is no empty row for that. To do that Highlight the First row, right-click on it, and then select “Insert”. A new row appears, then name the columns.

![Screenshot_126](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/b0e7beff-d48a-481c-88d2-da29de1bc991)

### Stage 4: The Power BI Magic — Real Data Cleaning. 

I will continue the next step using Power BI magical tools. As you may know, Power BI is the elder brother of Microsoft Excel Sheet. Now, save your table and Open it in the Power query editor.

![Screenshot_126](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/d36fb619-c341-4503-b817-e28e5b930e15)

Take a look at the screenshot, it has 16 Columns and 1M plus rows. Look at the Column quality where you have “Valid, Error, and Empty”, non of the Columns is up to 100%. There are Errors and Empty spaces. A whole lot of variables and abnormalities.

### Power Query Editor Process

 - Merge Columns — Merge columns with “null” cell Values, that is from “message” to column 16. I highlighted all the Columns, right-click on the header, and chose “Merge Columns”

![Screenshot_128](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/9b6e433c-ae17-412d-bf93-f50a00bfbf73)

Now, we are left with just 5 Columns — Date, Time, Time_1, User and Message. I will use the same process to merge the “Time and Time_1” Columns again the rename them “Time”.

![Screenshot_129](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/98edab27-7fb1-4b46-8f49-95544eb409ea)

 - Remove Errors — From the screenshot above you can see the “Valid” in “Users” and “Messages” Columns are not 100% yet. So, highlight both of the Columns, right-click on the header, and select “Replace Errors” and “Replace Empty” one after the other.

![Screenshot_129](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/e8208835-87e7-493b-b158-71d40497693f)

Our Dataset has gradually taken shape. As you can see, the Column quality is all 100%. From something that looks like a fatal accident to a final operation. Finally, we have 4 Columns and 650 rows. Ready for insight and Visualization.

Now, either from the “File” menu or the top left side of the screen, click on “Close & Apply”.

### Exploratory Data Analysis (EDA)
 
 #### Stage 5: Report and Dashboard

We are now on Power BI Desktop to complete the Analysis. We have a few questions to answer:

 - What is the Total No. of Users in the group?

 - What is the Total massage?

 - What is the Peak Chat Time?

 - Who is the Top Contributor in the Group?

 - What is the Total number of messages sent each day?

 - What is the No. of Users by Time?

Now, if you don’t know how to create a Report/Dashboard you may have to go to YouTube videos and learn because it’s going to be complicated explaining my process. I will only have to show screenshots with little insight.

 - First thing here I titled my report as WhatsApp Group Chat Analysis using the “Text Box” tab.

![Screenshot_131](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/3827620c-6bcb-4780-aaac-ed61def451e1)

 - I created my measures under the DAX table by first creating my DAX table from the “Enter Data” tab.

![Screenshot_132](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/cc1db5b4-28fa-4a35-890b-5b3529e8bb70)

 - I now created a New Measure to calculate the total number of users. Thus the calculation: Total No. of Users= DISTINCTCOUNT(WhatsApp_Scrap[Users]) = 7

In the same way, I created another Measure for the Total No. of Messages as 532

#### Individual Reports

Who is the Top Contributor in the Group?

![Screenshot_133](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/b80ae69a-2c26-41c1-bdaf-63ba994ea2fd)

What is the Peak Chat Time?

![Screenshot_134](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/366e78a3-156b-4a39-86b7-1dfcfbf16580)

What is the No. of Users by Time?

![Screenshot_135](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/b74aa9c5-6d04-48b7-b7b0-42d95931f5c9)

What is the Total number of messages sent each day?

![Screenshot_136](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/b3a42478-9ea4-4a88-80fa-0f5edf076428)

### Dashboard

![Screenshot_137](https://github.com/Solution92/WhatsApp-Group-Chat-Analysis-with-Power-BI-and-Excel./assets/144762124/17f589c0-c94d-4378-81dd-b993aa0b409d)

### Final Recommendation

I will encourage every Data enthusiast to practice Data Scraping of any group that you belong to, but make sure to ask for permanent. On a second note, practice that with Power BI because it has some hidden magic to discover only by practice.

The Top Contributor from the chat is the person I named Mr. Bassy, who did 188 messages in the group followed by Emmanuel with 153 messages, and so on.

Peak Chat Time is between 12:26 pm and 5:30 pm. This simply means that if you are in the group and you want your message to be read you must send your contribution within this time range.

The total number of Messages sent each day is 125 messages were sent on 16/09/23, followed by 59 on 4/10/23, and gradually it is reducing by the day.

### Limitation

The number of participant in the group were few

### Reference

[kaggle.com](https://www.kaggle.com/) will be a good place

Thank you!














