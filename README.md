# data-512-a2
Assignment 2 template. See: https://wiki.communitydata.cc/HCDS_(Fall_2017)/Assignments#A2:_Bias_in_data

### Goal of this Project
For this assignment the task is to analyze "what the nature of political articles on Wikipedia - both their existence, and their quality - can tell us about bias in Wikipedia's content"*.

### Process and Contents
We gather data from mulitple sources to get information about a Country's population, number of political articles and number of high quality political articles. High-Quality is based of the ORES API described below. We then calculate both the percentage of artcles per population and percentage of high quality articles per total articles. There is a write-up at the end summarizing my opinion on the findings.


### License
Under MIT License (see license file)
CC-0
This data was provided by Wikimedia Foundation and can be found at the URLs below (API).

### APIs
[ORES API](https://www.mediawiki.org/wiki/ORES)  

### Data Sources (csv files)
[Page_data](https://figshare.com/articles/Untitled_Item/5513449).
[Population Mid-2015](http://www.prb.org/DataFinder/Topic/Rankings.aspx?ind=14).


### Output Columns
**country**
Country Name

**article_name**
Name of the (political) article

**revision_id**
Unique identifier used in ORES call. Also call last_edit.

**article_quality**
Predicted quality score for the article (revId) retrieved from the ORES API.

**population**
Population of the country


### Other Issues
During the merge of the datasets (Page_Data and Population) only rows with matching country names were kept.

