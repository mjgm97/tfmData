User manual
===========

In this appendix, we are going to explain how to use the code to
reproduce our work with any corpus of documents available. To use the
framework, we will need two types of files: the papers (PDF) and the
metadata (CSV or XLS).

Metadata
--------

Once we have the PDF files that we want to analyze, the next step is to
get the metadata corresponding to those PDFs. To get the metadata, we
have two options: Scopus and Web of Science.

### Get metadata from Scopus

To get the metadata we need from Scopus, we need to log in the web page
(<https://www.scopus.com/search/form.uri?display=basic#basic>). You will
need to log in through your institution or your own account to start
searching. If we want to search for an individual paper, we can search
within “Article title”, as shown in the image below. If we have
several papers from the same source (i.e., conference, journal, book...)
we can search within “Source title” instead and get a set of results at
the same time.

![image](anex1.png)

Once we have located our papers on Scopus, we have to download their
metadata. To export the metadata as a CSV file, we have to click on “CSV
Export”, and then select which fields do you want to be exported, as
shown in the image below. For our analysis, we need to select the
fields “Author(s)”, “Document title”, “Year”, “Source title”, “Citation
count”, “Source & document type”, “Abstract”, and “Author keywords”. If
you export more fields, the framework will filter them and only show the
fields needed.

![image](anex2.png)

### Get metadata from Web of Science

To get the metadata from Web of Science, we need to log in the webpage
(<https://www.webofscience.com/wos/woscc/basic-search>). You will need
to log in through your institution or your own account to start
searching. If we want to search for an individual paper, we can search
within “Title”, as shown in the image below. If we have several
papers from the same source (i.e., conference, journal, book...) we can
search within “Publication Titles” instead and get a set of results at
the same time.

![image](anex3.png)

Once we have located our papers on Web of Science, we have to download
their metadata. To export the metadata as a XLS file, we have to click
on “Export” -\> “Excel”, and then select the full record to be exported,
as shown in the following image:

![image](anex4.png)

Paths and variables
-------------------

`Fontana` has been designed to be used in a Python notebook, since we
have integrated all the functionalities in the same environment. To be
able to use the framework, you will need to define the following paths
and variables:

-   `metadataPath`. This is the path where the CSV and XLS files,
    corresponding to the metadata, are located.

-   `papersPath`. This is the path where PDF files are located.

-   `metadataPath`. This is the path where the TXT files will be
    created.

-   `nTop`. The number of topics of the LDA model.

We can see how those variables are defined in the image below. Since
the framework will use every file that matches the format expected (for
example PDF files for full-text papers), we recommend to use separate
folders for each path.

![image](anex5.png)

And that is all! Now "Fontana" is ready to be used, and the only thing
you need to do is to navigate through the notebook and observe the
results produced. We can see some examples of the framework working live:

<span>0.49</span> ![image](anex6.png)

<span>0.48</span> ![image](anex7.png)

