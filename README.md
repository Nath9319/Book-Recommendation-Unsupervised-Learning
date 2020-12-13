# Book-Recommendation-Unsupervised-Learning

 Institut für Informatik, Universität Freiburg
 Book-Crossing Dataset ... mined by Cai-Nicolas Ziegler, DBIS Freiburg

Collected by Cai-Nicolas Ziegler in a 4-week crawl (August / September 2004) from the Book-Crossing community with kind permission from Ron Hornbaker, CTO of Humankind Systems. Contains 278,858 users (anonymized but with demographic information) providing 1,149,780 ratings (explicit / implicit) about 271,379 books.

[ ! ] Freely available for research use when acknowledged with the following reference (further details on the dataset are given in this publication):
Improving Recommendation Lists Through Topic Diversification,
Cai-Nicolas Ziegler, Sean M. McNee, Joseph A. Konstan, Georg Lausen; Proceedings of the 14th International World Wide Web Conference (WWW '05), May 10-14, 2005, Chiba, Japan. To appear.

Download: [ PDF Pre-Print ]

As a courtesy, if you use the data, I would appreciate knowing your name, what research group you are in, and the publications that may result.	


Format
The Book-Crossing dataset comprises 3 tables.
BX-Users
Contains the users. Note that user IDs (`User-ID`) have been anonymized and map to integers. Demographic data is provided (`Location`, `Age`) if available. Otherwise, these fields contain NULL-values.

BX-Books
Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (`Book-Title`, `Book-Author`, `Year-Of-Publication`, `Publisher`), obtained from Amazon Web Services. Note that in case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavours (`Image-URL-S`, `Image-URL-M`, `Image-URL-L`), i.e., small, medium, large. These URLs point to the Amazon web site.

BX-Book-Ratings
Contains the book rating information. Ratings (`Book-Rating`) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

Download
Various data format flavours are available. Note that all downloads are in .ZIP format
SQL Dump [26.391 KB]
Contains both schema information and data insertion statements. More convenient to use. Run as an SQL-script.

CSV Dump [25.475 KB]
Data as comma-separated values (CSV). The first line contains column names. Field separators are given by semicola, all entries are in quotes.

Other Datasets
MovieLens
Offers collaborative filtering (CF) datasets for movies. MovieLens datasets come in different sizes. Also links to the older EachMovie dataset that can be obtained upon request from Compaq.

Jester
Dense dataset for joke recommending. Large numbers of users, but small number of items (around 100 jokes) only.

[ IIF ]   [ DBIS ]   [ Cai-Nicolas Ziegler ]  
