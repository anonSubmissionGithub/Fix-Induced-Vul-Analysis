**Fix2Fix**

Metadata of the dataset is available in Insight_Mapped_With_CWE_Pair_Insights_Full.xlsx.

Metadata contains Project,	Commit,	Lines Added in Fixed Version,	Lines Deleted in Fixed Version,	Hunks in Fixed Version,	Github Link,	CWE ID	CVE ID, Next CWE ID, 1-line description of the change, High-level pattern of the change

Full data can be downloaded here
https://drive.google.com/drive/folders/1kV_KN_iUNk59oMYPrNo7BYe77ROJ83La?usp=sharing

Hierarchical format of the data.

```
|--- Project_Name1/
|   |
|   |--- Project_Name_CommitHash1/
|   |   |
|   |   |--- all_versions/
|   |   |   |--- File_v1_DATE_TIME.txt
|   |   |   |--- File_v2_DATE_TIME.txt
|   |   |   |--- File ....
|   |   |
|   |   |--- commit_messages/
|   |   |   |--- File_v1_DATE_TIME_commit_msg.txt
|   |   |   |--- File_v2_DATE_TIME_commit_msg.txt
|   |   |   |--- File ....
|   |   |
|   |   |--- file_changes_in_versions/
|   |   |   |--- File_changes_v1_v2_DATE_TIME.txt
|   |   |   |--- File_changes_v2_v3_DATE_TIME.txt
|   |   |   |--- File ....
|   |
|   |--- Project_Name_CommitHash2/ ....
|   |
|--- Project_Name2/  ....
```

**Dataset creation code**


The dataset provided is ready to use. Here, the  details are provided about the data collection process. If you just want to use the dataset, this part is not required. 
Data Collection.ipynb file extracts all future versions from GitHub for future analysis. 


Data_Process_FullyCleaned.ipynb file processed the data once the future versions are collected.

**Use case**
To collect next vulnerability information from GPT, "GPT_nextVulPrompt-Cleaned.ipynb" is used. You need to add your API key.

https://drive.google.com/drive/folders/1WaeLvuX8o17zxjrLtet11PfZjQcz-8Bf?usp=sharing
