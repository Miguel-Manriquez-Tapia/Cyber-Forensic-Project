














<h1>Cyber-Forensics Project</h1>


<h2>Description</h2>
An oil company needs a forensic investigation conducted for one of its employees named John Smith. For this prooject we are going to use Autopsy to determine if the user has taken or accessed any proprietary information from the oil company. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Autopsy</b> 

<h2>Environments Used </h2>

- <b>Microsoft Virtual Machine</b> 


<h2>Project walk-through:</h2>

Part 1:

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/1st.png)Open  

1.  Open - Autopsy64 – located on the desktop as a shortcut.
    

  
  

2.  Create a New Case on Autopsy.
    

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_cb8fb71a.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

3.  Enter Case Information
    

Case Name: JSmith\_Case

Base Directory: C:/Users/LabUser/Desktop/Evidence Files

 ![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_a99e81ad.png)Click - Next >

  
  

  
  

  
  

  
  

  
  

  
  

  
  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_793ab594.png)  
  

  
  

  
  

  
  

\* **Add Case Number & Examiner’s Name.**

  
  

  
  

  
  

  
  

4.  Select - Generate new host name based on data source name.
    

Click – Next >

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_fdb9ebca.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

5.  Select Data Source Type
    

Click – Disk Image or VM File

Click – Next >

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_e745d2ac.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

6.  Browse to Path: C:/Users/LabUse/Desktop/Evidence Files/JSmith\_Q1.001
    

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_96b60d5.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

7.  Configure Ingest
    

Keep selected default settings.

Click – Next >

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_ff335ee4.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

8.  5\. Add Data Source (no action need)
    

Click - Finish

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_1c61a9aa.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

9.  We can begin the analysis now that the data sources are available, located at on the left side.
    

  
  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_2d718985.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

10.  During the investigation we will extract files (right click on file name) and save them to**:** **C:\\Users\\LabUser\\Desktop\\Evidence Files\\Example\\Export**
    

  
  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_af6cbf0c.png)  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  

  

Part 2:

  

1.  Before starting the analysis, it is important to do an integrity check of the source and image file’s hashes. For this I used the MD5 checksum hash from JSmith\_Q1.001.txt to verify that it was an exact match to the image made for the autopsy investigation. The MD5 hash of the image on autopsy can be found in the metadata “File Metadata” tab when clicking on the image.
    

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_3f0fd59.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

2.  To keep the important findings in a centralized location I created a “Tags” folder and named it: Investigate further and check the notable box in the prompt. We will be using this folder for PDF that will need to be extracted to investigate. For the photos to be extracted, we will use the default tags notable folder in autopsy.
    

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_524da79.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

3.  Next, we will go to the System Volume Information folder, there we will find the “Parent Volume”.
    

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_467a3774.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

4.  Inside the “Parent Volume” folder we see everything that is in the image for JSmith\_Q1.001. I went through and tagged the PDFs to the Investigate further folder and the photos to the notable folder.
    

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_5c32cc28.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_6953b82b.png)  

  

\*Photos Tag Folder

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_4243d5c5.png)  

  

  

  

  

\*Investigate Further Tag Folder

  

  

  

  

  

  

  

  

  

  

  

  

5.  I extracted all the PDFs and JPGS to the “Export” folder, making a separate folder for the JPEGS for the sake of organization.
    

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_cd29073c.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_4bfa4f20.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

6.  The exported PDFs found on the image are as follows.
    

  

1.  “The best way to hide something, is in plain sight. Crypto laundering.”
    

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_a1324758.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

2.  “Transaction Mixer: How to Hide “Dirty” Bitcoins”
    

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_ebb57d27.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

3.  “How to buy and pay with bitcoin anonymously”
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_a8155b91.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

4.  “6 Ways To Make Untraceable Bitcoin Transactions”
    

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_a344e2bb.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

5.  “Oil Company (Labeled: CONFIDENTAIL Restricted) Oil Strategies 2021 Field 007-A”
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_d7633e8f.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

6.  “Oil Company (Labeled: Confidential – No Release) Strategic Business – Data Management and Analytics”
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_d5582ada.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

7.  “Oil Company (Labeled: CONFIDENTIAL Restricted) Business Strategies 2021”
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_fbc9b784.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

7.  The JPEGS found on the image are the following:
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_aef746ee.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_d28fa15c.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_a47660d2.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

8.  Next, we looked at the metadata of the files to look for the owner of the PDFs. The owner of the PDFs “Oil Company data strategy”, “Business Strategy”, and “Drilling Methodology” is Mike Morris.
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_5dfcda5f.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_c9f4dc52.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_3626191e.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_c3c5b071.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

9.  We checked the deleted files folder for any other data that was removed and found the same PDFs and JPGs that we had seen on the parent folder.
    

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_6475cef6.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

10.  Lastly, we ran a keyword search on the saved image for “confidential” and found this:
    

  

  

![](file:///C:/Users/migue/AppData/Local/Temp/lu5414440namq.tmp/lu5414440namv_tmp_ce62726a.png)  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

  

A3.)

  

  

In the case of JSmith, we found three PDFs classified as confidential that have proprietary company information. The PDFs are named “Business Strategy”, “Drilling Methodology”, and “Oil company data strategy”. Along with those PDFs, the disk image had multiple photos saved related to the company’s industry, these pictures do not have a sensitivity label. The PDFs found and retrieved from the deleted files folder, indicate that Mr. Smith’s actions were deliberate to take intellectual property from the oil company.
