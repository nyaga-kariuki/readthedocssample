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
                       
* pattern: Pandas Dataframe, this is the the pattern one is looking to be recognized with a label for the category, stored as DataFrame i.e. {'Termination':['K']}
* rejectLevel: Integer, this describes degree to which pattern must match to be a "match".
* searchData: Pandas Dataframe, The KhipuData being examined, this can be filler when retrivel = True
* retrieval: Boolean argument to describe whether input khipus will be manually descibed. If True all following arguements must be filled out.
* columninfo: This is a list of string for each coloumn name used for specificaiton, i.e. [Termination,
* valueinfo: This specifies which values are acceptable for each column name.
* info: String, which info to collect, the deafult is "*" which will give back all data in database.
* level: String, level of database to examine. This is very important since 
* listTitle: DONT KNOW WHAT THIS IS

Output
******

Usage
******

The primary use of these functions is use of this is to find a some pattern in a dataset. Let us consider the general format than a specific example.
::
    patterndict = {'Category1': [list of values1],'Category2': [list of values2],...} # dictionary for creating Dataframe
    patterndf = pd.DataFrame(patterntestlist) #DataFrame for input into function
    
    reject = n #depends on your desired accuracy 

    sum,test = findGeneralPattern(patterntestdata,reject, searchData = patterndf, retrieval = False)
    
    
The sum and test will be as described above
