**Vul-Fix-Vul**

Metadata of the dataset is available in merged_full_dataset_with_versions_and_claude.csv.

Metadata contains Project,	Commit,	Lines Added in Fixed Version,	Lines Deleted in Fixed Version,	Hunks in Fixed Version,	Github Link,	CWE ID	CVE ID

Full data can be downloaded here
https://drive.google.com/file/d/1ngsC_ES2G6OduJWVkuwvwyuuzPQvxyvn/view?usp=sharing

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
Data Collection.ipynb file extracts all future versions from GitHub for future analysis. It starts with BigVul dataset. Processed commit information from BigVul dataset is provided in dfVulCWE.csv. The file can be downloaded using the link
https://drive.google.com/file/d/1LxkCphSaoUeb1CKaDf9kj8Rf1zHrTTKX/view?usp=sharing

Data_Process_FullyCleaned.ipynb file processed the data once the future versions are collected.
