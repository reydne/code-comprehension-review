# Evaluating Code Readability and Legibility: An Examination of Human-centric Studies
[IEEE publication link](https://ieeexplore.ieee.org/document/9240710)

[Arxiv link](https://arxiv.org/pdf/2110.00785.pdf)

In this repository are found some additional materials about the research.

## Search string per engine (SS)

Each search engine has its own form of advanced search, so the search string must be adjusted for each of the devices used in the review. Therefore, the search strings used in each machine are listed below.

* ACM ([CSV](csv/Engine-Result-ACM.csv)):

          acmdlTitle:("code comprehension" "code understandability" "code understanding" "code readability" "program comprehension" "program understandability" "program understanding" "program readability" "programmer experience") OR keywords.author.keyword:("code comprehension" "code understandability" "code understanding" "code readability" "program comprehension" "program understandability" "program understanding" "program readability" "programmer experience")

* IEEE ([CSV](csv/Engine-Result-IEEE.csv)):
        
        (("Document Title":"code comprehension" OR "Document Title":"code understandability" OR "Document Title":"code understanding" OR "Document Title":"code readability" OR "Document Title":"program comprehension" OR "Document Title":"program understandability" OR "Document Title":"program understanding" OR "Document Title":"program readability" OR "Document Title":"programmer experience") OR ( "Author Keywords":"code comprehension" OR "Author Keywords":"code understandability" OR "Author Keywords":"code understanding" OR "Author Keywords":"code readability" OR "Author Keywords":"program comprehension" OR "Author Keywords":"program understandability" OR "Author Keywords":"program understanding" OR "Author Keywords":"program readability" OR "Author Keywords":"programmer experience"))

* Scopus ([CSV](csv/Engine-Result-Scopus.csv)):

         ( TITLE ( "code comprehension" )  OR  TITLE ( "code understandability" )  OR  TITLE ( "code understanding" )  OR  TITLE ( "program comprehension" )  OR  TITLE ( "program understandability" )  OR  TITLE ( "program understanding" )  OR  TITLE ( "program readability" )  OR  TITLE ( "programmer experience" ) )  OR  ( KEY ( "code comprehension" )  OR  KEY ( "code understandability" )  OR  KEY ( "code understanding" )  OR  KEY ( "program comprehension" )  OR  KEY ( "program understandability" )  OR  KEY ( "program understanding" )  OR  KEY ( "program readability" )  OR  KEY ( "programmer experience" ) )  AND  ( LIMIT-TO ( DOCTYPE ,  "cp" )  OR  LIMIT-TO ( DOCTYPE ,  "ar" ) )  AND  ( LIMIT-TO ( SUBJAREA ,  "COMP" ) )

## List of papers and Selection (LPS)
In this directory, there is a list of all the papers found in each search engine. This directory is organized according to the exclusion phase and inclusion phase. The criteria evaluated in each phase are listed below.

* All Papers (after merge all engines results)
  * Csv: [All documents](csv/MergedDocuments-Raw.csv) | [Manual included papers](csv/ManualPapersFound-Raw.csv)
  * Pages (with informations about all phases): [Part 1](list-papers/AllPhasesMergedPapers-Part1.md) | [Part 2](list-papers/AllPhasesMergedPapers-Part2.md) | [Part 3](list-papers/AllPhasesMergedPapers-Part3.md) | [Part 4](list-papers/AllPhasesMergedPapers-Part4.md) | [Part 5](list-papers/AllPhasesMergedPapers-Part5.md)


* Study Exclusion (Result after this phase: [csv](csv/Triage-Raw.csv) | [page](list-papers/Triage.md))

 ID | Description 
--------- | :------
 EC1 | The paper is outside the scope of this study. It is not primarily related to source code comprehension, readability, or legibility, does not involve any comparison of different ways to write programs, neither direct nor indirect, or is clearly irrelevant to our research questions. For instance, we exclude studies focusing on high-level design, documentation, and dependencies (higher-level issues). 
 EC2 | The study is not a full paper (e.g. MSc dissertations, PhD theses, course completion monographs, short papers) or is not written in English. As a rule of thumb, we consider that full papers must be at least 5 pages long. 
 EC3 | The study is about readability metrics without an experimental evaluation. 
 EC4 | The study is about program comprehension aids, such as visualizations or other forms of analysis or sensory aids (e.g. graphs, trace-based execution, code summarization, specification mining, reverse engineering). 
| EC5 | The study focuses on accessibility, e.g., targets individuals with visual impairments or neurodiverse developers. 

* Study Inclusion (Result after this phase: [csv](csv/First_Selection-Raw.csv) | [page](list-papers/First_Selection.md))

ID | Description 
--------- | :------
IC1  (Scope) | The study must be primarily related to the topics of code comprehension, readability, legibility, or hard-to-understand code.
IC2 (Methodology) | The study must be/contain at least one empirical study, such as controlled experiment, quasi-experiment, case study, or survey involving human subjects.
IC3 (Comparison) | The study must compare alternative programming language constructs, coding idioms, or coding styles in terms of code readability or legibility.
IC4 (Granularity) | The study must target fine-grained program elements and low-level/limited-scope programming activities. Not design or comments, but implementation.

## Study quality assessment questionnaire (QA)
In the quality assessment stage of primary studies included in the systematic review, we used a questionnaire as a guide. This questions used in this phase are listed below.

* Questions about design: QA1, QA2, QA3
* Questions about analysis and rigor: QA4, QA5, QA6, QA7
* Questions about conclusion: QA8, QA9

ID | Questions for quality assessment for study 
--------- | :------
QA1 | Are the aims clearly stated?
QA2 | Are the independent variables adequately defined?
QA3 | Are the dependent variables adequately defined?
QA4 | Are the data collection methods adequately described?
QA5 | Are the study participants or observational units adequately  described? For example, SE experience, type (student,  practitioner, consultant),  nationality, task experience and  other relevant variables.
QA6 | Were the collected data adequately described (e.g., descriptive statistics)? 
QA7 | Did the study employ statistical methods to analyze the data?
QA8 | Is there a clear statement of findings, i.e., are all study questions answered?
QA9 | Do the researchers explain the threats to the study validity?


## Data extraction questionnaire (DE)
The data extraction step was also conducted through a questionnaire. Below are found the questions used in this phase. 

* Assessment method: 10-15
* Results: 16 and 17

Question | Possible answers
--------- | :------
1- Title 
2- Authors 
3- Publication Year 
4- Publication Venue 
5- What is the topic of the study? | - Readability - Legibility - Both
6- What exactly is being compared? | Code construct more generally, what are the independent variables? constructs (for vs. while loops, ifs vs. ternary expressions, etc.) Coding style formatting (indentation, spacing, how to lay out the code, naming conventions) coding style (same constructs, different ways of using them, e.g., reassigning to the same variable vs. assigning to different variables)
7- What code attributes are captured by them (independent variables) ? | Blank lines, number of keywords, code length, number of atoms of confusion or whether the code exhibits or not atoms of confusion.
8- What were the targeted languages? | Java, C, C++, Haskel, Python, others.
9- What are the research questions of the study? | In case there are no explicitly stated research questions, we can just write the general goal of the study.
10- What is the assessment methodology? | (Quasi-) Experiment, opinion survey, some form of case study Based on http://www.cs.utoronto.ca/~sme/papers/2007/SelectingEmpiricalMethods.pdf
11- What was the sample of the evaluation? | Human subject/system subject Students, professionals, software systems.
12- What activities did the subjects have to perform? If the sample consists of software systems, what activities involving these systems were conducted?
13- What attributes are being measured (dependent variables)? | Time to complete, number of errors, brain activity, pieces of the code that are being inspected/eye tracking, opinions of grades, preexisting readability metrics (e.g., Buse and Weimer's work), etc.
14- How are they being measured? | (e.g., if it's number of errors, how does the paper assess whether the subject erred? In case it is eye tracking, what metrics/qualitative evaluation is being derived from the eye tracking information?)
15- Did the paper use statistics? How? What has been tested? What kind of data correction was applied?  If multiple tests were applied for the different RQs, please discuss all of them.
16- What did the paper find out? What are the answers to the research questions?
17- How the statistics tests infers in the results?

