# Jira: An Alternative Issue Tracking Dataset
Source:
* https://arxiv.org/abs/2201.08368
* https://scholar.googleusercontent.com/scholar.bib?q=info:pY93oSnluIUJ:scholar.google.com/&output=citation&scisdr=CgXU7pQTELHQ9Z13O0c:AAGBfm0AAAAAYhtxI0eXhr40J1ORT97-YL1AbDsrHp-z&scisig=AAGBfm0AAAAAYhtxI2yrtUF5FOf2IpbP6N4p9QVXCK4T&scisf=4&ct=citation&cd=-1&hl=en

## Analysis
*  Data overview:
    * 16 public Jira repositories, in total containing:
    * 1822 projects
    * 2.7 million issues with in total:
        * 32 million historical records of changes 
        * 9 million comments, and 1
million issue links that connect the issues in multiple ways. 
* "Over the last two decades, software engineering research has intensively studied issues and issue trackers, often based on Bugzilla and GitHub."
* "The primary research focus has been on the specific issue type of bug reports: the understanding and improvement of information quality therein and the prediction of bug properties such as severity, assignee, and duplicate reports for supporting software evolution and maintenance."
* The authors suggest Jira as an alternative data source for these types of research.
* Jira is the most prominent tool used nowadays (slintel6, Datalyze7, and Enlyft8), so it makes sense to use it as main data source
* It has historically been used less in existing literature [9]
* Jira also allows the creation of issue maps from their internal dependencies on each other, a possibly strong feature.
* They mention that "More research is needed to understand how issue linking works, what effect links have on the issue tracking ecosystems, and how they can be leveraged to create more productive and efficient development environments." However, choetkiertikul2015predicting has done such a somewhat similar study where "networked" data created from linked issues was used to predict issue delay.


## Research gap
* As this is not a traditional paper with new findings, the research gaps are little and of a different nature
* The authors notice the flaw in the dataset due to two of the repositories (MariaDB and Mindville) no longer being available in between the different times they retrieved the data.
* Another flaw is that due to the nature of Jira, customized attributes exist not only inside different repos, but also inside different projects inside a repo. "For this reason, the data is
richer, but also more complex and hard to unify. We have made a first attempt at unifying the major components by starting with the issue and link types."
* "Future improvements to the data can certainly be made. This includes additional qualitative labelling, cleaning based on use cases, and finding more Jira API hooks worth pulling data from to add to the breadth of data available for each repo."
