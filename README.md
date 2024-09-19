


<h1>Cyber-Forensics Project</h1>


<h2>Description</h2>
An oil company needs a forensic investigation conducted on one of its employees named John Smith. For this prooject we are going to use Autopsy to determine if the user has taken or accessed any proprietary information from the oil company. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Autopsy</b> 

<h2>Environments Used </h2>

- <b>Microsoft Virtual Machine</b> 


<h2>Project walk-through:</h2>

**Part 1:**

1.  Open - Autopsy64 – located on the desktop as a shortcut.
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/1st.png)
  
  

2.  Create a New Case on Autopsy.
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191228.png)


  
  

3.  Enter Case Information
    

    Case Name: JSmith\_Case

    Base Directory: C:/Users/LabUser/Desktop/Evidence Files
<br >

    Click Next >

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191302.png)  
  


  
  

\* **Add Case Number & Examiner’s Name.**

  
 ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191322.png)



  
  

4.  Select - Generate new host name based on data source name.
    

    Click – Next >

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191343.png)
  

  
  
  

5.  Select Data Source Type
    

    Click – Disk Image or VM File

    Click – Next >

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191407.png)
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

  
  

6.  Browse to Path: C:/Users/LabUse/Desktop/Evidence Files/JSmith\_Q1.001
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191434.png) 
  
  
  

7.  Configure Ingest
    

    Keep selected default settings.

    Click – Next >

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191457.png)
  




8.  Add Data Source (no action need)



    Click - Finish

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191520.png)  
  



9.  We can begin the analysis now that the data sources are available, located at on the left side.
    

  
  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191540.png)
  

  
  

10.  During the investigation we will extract files (right click on file name) and save them to**:** **C:\\Users\\LabUser\\Desktop\\Evidence Files\\Example\\Export**
    

  
  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191557.png)  
  

  

Part 2:

  

1.  Before starting the analysis, it is important to do an integrity check of the source and image file’s hashes. For this I used the MD5 checksum hash from JSmith\_Q1.001.txt to verify that it was an exact match to the image made for the autopsy investigation. The MD5 hash of the image on autopsy can be found in the metadata “File Metadata” tab when clicking on the image.
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191615.png)

  

2.  To keep the important findings in a centralized location I created a “Tags” folder and named it: Investigate further and check the notable box in the prompt. We will be using this folder for PDF that will need to be extracted to investigate. For the photos to be extracted, we will use the default tags notable folder in autopsy.
    

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191636.png)

  

  

3.  Next, we will go to the System Volume Information folder, there we will find the “Parent Volume”.
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191652.png) 

  


4.  Inside the “Parent Volume” folder we see everything that is in the image for JSmith\_Q1.001. I went through and tagged the PDFs to the Investigate further folder and the photos to the notable folder.
    

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191704.png) 

  


  

\*Photos Tag Folder

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191732.png)  


  

\*Investigate Further Tag Folder


  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191748.png)

  

  

5.  I extracted all the PDFs and JPGS to the “Export” folder, making a separate folder for the JPEGS for the sake of organization.
    

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191809.png)

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191827.png)

  

  

6.  The exported PDFs found on the image are as follows.
    

  

     “The best way to hide something, is in plain sight. Crypto laundering.”
    

  

  

  
   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191841.png)

  

  
  

7a.  “Transaction Mixer: How to Hide “Dirty” Bitcoins”
    

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191902.png)
  

  

  

 7b. “How to buy and pay with bitcoin anonymously”
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191915.png) 

  

  

 7c. “6 Ways To Make Untraceable Bitcoin Transactions”
    

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191928.png)
  

  

  

7d.  “Oil Company (Labeled: CONFIDENTAIL Restricted) Oil Strategies 2021 Field 007-A”
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191942.png)

  

  
  

7e. “Oil Company (Labeled: Confidential – No Release) Strategic Business – Data Management and Analytics”
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20191957.png) 

  

  
  

7f. “Oil Company (Labeled: CONFIDENTIAL Restricted) Business Strategies 2021”
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192009.png)

  


  

 7.1 The JPEGS found on the image are the following:
    

  

  

7.1.a   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192026.png)

  


  

7.1.b   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192045.png)
  

  


7.1.c   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192105.png)


  

  
8.  Next, we looked at the metadata of the files to look for the owner of the PDFs. The owner of the PDFs “Oil Company data strategy”, “Business Strategy”, and “Drilling Methodology” is Mike Morris.
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192138.png)

  


  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192205.png)

  

  

9.  We checked the deleted files folder for any other data that was removed and found the same PDFs and JPGs that we had seen on the parent folder.
    

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/Screenshot%202024-09-18%20192221.png)  

   
  

10.  Lastly, we ran a keyword search on the saved image for “confidential” and found this:
    

  

  

   ![image alt](https://github.com/Miguel-Manriquez-Tapia/Cyber-Forensic-Project/blob/main/last.png)

  



Summary:

  

  

In the case of JSmith, we found three PDFs classified as confidential that have proprietary company information. The PDFs are named “Business Strategy”, “Drilling Methodology”, and “Oil company data strategy”. Along with those PDFs, the disk image had multiple photos saved related to the company’s industry, these pictures do not have a sensitivity label. The PDFs found and retrieved from the deleted files folder, indicate that Mr. Smith’s actions were deliberate to take intellectual property from the oil company.
