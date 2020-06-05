# Evaluating Code Readability and Legibility: An Examination of Human-centric Studies
In this repository are found some additional materials about the research.

## [Search string per engine (SS)](/AllPhasesMergedPapers-Part1.md)

Each search engine has its own form of advanced search, so the search string must be adjusted for each of the devices used in the review. Therefore, the search strings used in each machine are listed below.

* ACM:

          acmdlTitle :( "code comprehension" "code understandability" "code understanding" "code readability" "program comprehension" "program understandability" "program understanding" "program readability" "programmer experience" "readability") OR keywords .author.keyword :( "code comprehension" "code understandability" "code understanding" "code readability" "program comprehension" "program understandingability" "program understanding" "program readability" "programmer experience" "readability")

* IEEE:
        
        (("Document Title": "code comprehension" OR "code understandability" OR "code understanding" OR "code readability" OR "program comprehension" OR "program understandability" OR "program understanding" OR "program readability "OR" programmer experience "OR" readability "OR (" Author Keywords ":" code comprehension "OR" code understandability "OR" code understanding "OR" code readability "OR" program comprehension "OR" program understandability "OR" program understanding "OR" program readability "OR" programmer experience "OR" readability "))

* Scopus:

         TITLE ("programmer experience") OR TITLE ("program comprehension") OR TITLE ("code comprehension") TITLE ("code readability") OR TITLE ("code understandability") OR KEY ("code comprehension") ) OR KEY ("program comprehension") OR KEY ("program understandability") OR KEY ("readability")

## List of papers (LP)
In this directory, there is a list of all the papars found in each search engine. This directory is organized according to the exclusion phase and inclusion phase. The criteria evaluated in each phase are listed below.

* Study Exclusion

 ID | Description 
--------- | :------
 EC1 | The paper is outside the scope of this study. It is not primarily related to source code comprehension, readability, or legibility, does not involve any comparison of different ways to write programs, neither direct nor indirect, or is clearly irrelevant to our research questions. For instance, we exclude studies focusing on high-level design, documentation, and dependencies (higher-level issues). 
 EC2 | The study is not a full paper (e.g. MSc dissertations, PhD theses, course completion monographs, short papers) or is not written in English. As a rule of thumb, we consider that full papers must be at least 5 pages long. 
 EC3 | The study is about readability metrics without an experimental evaluation. 
 EC4 | The study is about program comprehension aids, such as visualizations or other forms of analysis or sensory aids (e.g. graphs, trace-based execution, code summarization, specification mining, reverse engineering). 
| EC5 | The study focuses on accessibility, e.g., targets individuals with visual impairments or neurodiverse developers. 

* Study Inclusion

ID | Description 
--------- | :------
IC1  (Scope) | The study must be primarily related to the topics of code comprehension, readability, legibility, or hard-to-understand code.
IC2 (Methodology) | The study must be/contain at least one empirical study, such as controlled experiment, quasi-experiment, case study, or survey involving human subjects.
IC3 (Comparison) | The study must compare alternative programming language constructs, coding idioms, or coding styles in terms of code readability or legibility.
IC4 (Granularity) | The study must target fine-grained program elements and low-level/limited-scope programming activities. Not design or comments, but implementation.

## Study quality assessment questionnaire (QA)
In the quality assessment stage of primary studies included in the systematic review, we used a questionnaire as a guide. This questions used in this phase are listed below.


ID | Questions for quality assessment for study 
--------- | :------
Questions about design

QA1 | Are the aims clearly stated?
QA2 | Are the independent variables adequately defined?
QA3 | Are the dependent variables adequately defined?

Questions about analysis and rigor
QA4 | Are the data collection methods adequately described?
QA5 | Are the study participants or observational units adequately  described? For example, SE experience, type (student,  practitioner, consultant),  nationality, task experience and  other relevant variables.
QA6 | Were the collected data adequately described (e.g., descriptive statistics)? 
QA7 | Did the study employ statistical methods to analyze the data?


Questions about conclusion 
QA8 | Is there a clear statement of findings, i.e., are all study questions answered?
QA9 | Do the researchers explain the threats to the study validity?



## Data extraction questionnaire (DE)
The data extraction step was also conducted through a questionnaire. In this directory are found the questions used in this phase.  
