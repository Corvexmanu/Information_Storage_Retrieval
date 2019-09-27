# SEARCH ENGINE

Implement an information search and retrieval system in C# using Lucene.NET 3.0.3;

• Implement changes to the application to differentiate it from the baseline system. As part of these changes you must: (See Section 3 for more details)

Pre-process the information need to create a query as the input into the application. Query creation must be automated and require no manual input from the user.

Implement one or more sensible and justifiable changes to Lucene’s “DefaultSimilarity Class”
• Evaluate the performance of the application and compare it to the baseline system;
• Produce a written report that describes, amongst other things, the design, testing, performance and instructions on how to use your application.


- INDEXING	Set Directory Paths	As a user, I want to specify two directory paths. The first directory path will contain the source collection. The other directory path will contain the location where a Lucene index will be built.

- INDEXING	Create Index	As a user, I want to be able to indicate that I would like to create the index from the specified collection (e.g. through a button click or similar) which is then done programmatically.

- INDEXING	Report Indexing Time	As a user, I want that the application report me the time that  it takes to build the index.

- INDEXING	Build Index	As a programer, I need that the system built an index in the path specified and also it records the time spent. All of the text should be indexed as a single field

- INDEXING	Baseline indexation	As a user, I want that For each file in the collection, all of the text be indexed as a single field. Also, the index does not save information related to field normalisation.

- INDEXING	Baseline Analysing	As a user, I want that The Analyzer used during index and search is the Lucene.Net.Analysis.Simple analyzer. Also, The index does not save information related to term vectors.

- SEARCHING	Able to Search	As a user, I want to be able to search the index once it has been built. 

- SEARCHING	Searching and Ranking	As a programer, I need that the application  match the final query to relevant documents and rank the documents according to relevance. 

- SEARCHING	Report Searching Time	As a user, I need that the application  report how long it took to search the index and display this on the GUI (include the time  equired for query creation).
10	SEARCHING	Display Ranked Documents	As a user, I need that the application display in the GUI how many relevant documents were returned from the search and should present a ranked list of the top 10 relevant documents. Each ranked document should present the title; The author/s;  Bibliographic information (journal abbreviation, volume/number, year of publication, page number); The first sentence of the abstract. 

- BROWSING	Browsing Results	As a user, I need to be able to select the following 10 most relevant result and display in groups of 10 the subsequent most relevant result. Also, I need to move forward and backward thorough the ranked list of results, viewing 10 results at a time.

- RETRIEVING	Retrieve Results	As a user, I want to view the entire abstract by using an appropriate interface control, this can either open in the existing window or a new window.

- RETRIEVING	Save list	As a user, I need to have the option of saving the list of the retrieved results in a text file. I want to specify the name of the file to save the results and query identification.

- RETRIEVING	Append new results	As a user, I need that new results should be appended to the end of an existing results file, and The format of the text file should be compatible with the trec_eval program (TopicID, Q0, DocID,rank, score, student numbers and name all separated by whitespaces and unix formated file)

- SEARCHING	Multi-term and/or Multi-phrase	As a user, I want to have the option via a checkbox/radio button or similar control to submit multi-term and/or multi-phrase queries “as is” with no pre-processing

- SEARCHING	Enter information need	As a user, I should be able to enter a natural language information need into a search box. So that…..

- SEARCHING	Process Information need	As a programer, I need that the application process the information need of the user to create a final query that is submitted into the application automatically.

- SEARCHING	Display Query	As a user, I want that the  final query created programmatically from the natural language information need  be displayed on the GUI (a simple display of the query object submitted).
18	SEARCHING	Processing information	As a programer, I need to define how the application processes the information need entered by the user

- SIMILARITY	Improve baseline scoring.	As a programer, you need to make sensible and justifiable modifications to the Lucene scoring function by implementing a custom similarity class which inherits from the “DefaultSimilarity” base class.

- CHANGES	Changes in baseline	As a programmer, You should try to implement 2 changes that improve the performance of your application with respect to the baseline system.

- IMPROVEMENTS	Lexical Database	As a user, I need that the application connect a lexical database (e.g.: WordNet) to perform query expansion in the searching operations. 

- IMPROVEMENTS	Linguistic levels	As a user, I want that the  system should include set of customizable options to select different linguistic levels in your query expansion.

- IMPROVEMENTS	Wight of query	As an user, I need that  address the problem of ranking higher documents that contain a query expansion more than the original query, so that you give more weight to the original term.

- IMPROVEMENTS	Demonstrate query expansion	As a programer, You should have an option in your system to demonstrate these options with Query Expansion and weighted queries.

- IMPROVEMENTS	Boosting query	"As a programmer, you should Implement the Field level boosting for your search queries using the two fields, Title and the
Author available in your collection. You should be able to show the different set of results for two different field level boosting."


The present project was a colaborative effort done by the following students of Master of information technology in Queensland University of Technology, Brisbane Australia:

Manuel Villamil   N10080236
Chen-Yen Chou     N10030581
Shih-Hang Lee     N9802614
