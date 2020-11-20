# Web-Scraping-and-Textual-Analysis-on-Gov-Regulations
Web Scraping on "regulations.gov"; textual Analysis on Comments on Bank Regulation


There are a total of 4 Jupyter Notebooks:
1.	all_docket_id.ipynb: collect all docket ids for any html main page input. Usually, you are expected to type in something (such as ‘OCC’) in the search bar on ‘regulations.gov’, then paste the main page after the search into the input of this notebook. It will generate all docket ids related to this search.
2.	Summary_Table.ipynb: input for this notebook is the docket id table generate from step 1. The output is one summary table with 1. The name of the regulation; 2. The Docket ID and RIN number; 3. The summary. 4. What PDF documents we collected (such as supporting documents, comment letters, proposed rule, final rule of the regulation).
3.	PDF_download_func.ipynb: input for this notebook is the docket id table generate from step 1. After running this code, all documents related to the dockets will be downloaded into your desired location on your machine. 
4.	Textual Complexity Analysis.ipynb: run Textual Complexity Analysis on all textual files (convert PDF downloaded in step 3 into text files first using Adobe Acrobat). The output is a json file (dictionary structure) storing 'number of vocabulary', 'word complexity', 'sentence complexity', 'unique words percentage' for every document. 
