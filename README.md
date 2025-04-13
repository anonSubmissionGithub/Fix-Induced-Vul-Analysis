**Vul-Fix-Vul**

Metadata of the dataset is available in merged_dataset_with_CVE_CWE.csv.

Metadata contains Project,	Commit,	Lines Added in Fixed Version,	Lines Deleted in Fixed Version,	Hunks in Fixed Version,	Github Link,	CWE ID	CVE ID


Full data can be downloaded here
https://drive.google.com/file/d/1ngsC_ES2G6OduJWVkuwvwyuuzPQvxyvn/view?usp=drive_link

Hierarchical format of the data.

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
