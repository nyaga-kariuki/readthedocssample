Khipu Retrieval Functions
##########################

Introduction
*************

These functions takes in specifications and return Khipu data. Helper functions are explained at the end.

Arguements
***********

This is the function parameters 
::
  findGeneralPattern(pattern, rejectLevel, searchData = pd.DataFrame({'fill':['fill-value']}), 
                       retrieval = True , columninfo = [], valueinfo = [], 
                       info = "*", level = "knot", listTitle = True)
                       
* pattern: This is the the pattern one is looking to be recognized with a label for the category, stored as DataFrame i.e. {'Termination':['K']}
* rejectLevel: Integer, this describes degree to which pattern must match to be a "match".
* searchData: The KhipuData being examined, this can be filler when retrivel = True
* retrieval: Boolean argument to describe whether input khipus will be manually descibed. If True all following arguements must be filled out.
* columninfo: This is a list of string for each coloumn name used for specificaiton, i.e. [Termination,
* valueinfo: This specifies which values are acceptable for each column name.
* info: String, which info to collect, the deafult is "*" which will give back all data in database.
* level: String, level of database to examine. This is very important since 
* listTitle: DONT KNOW WHAT THIS IS


Usage
******

The easies use of this is to
