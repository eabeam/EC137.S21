# R Troubleshooting

Compiled list of issues 

[TOC]



## Cannot find data 

Look at the working path on RStudio. It's right below the tab. Make sure your data file is in that folder. 





## Cannot knit! 



### Need to comment out `install_packages()`

```
Error in contrib.url(repos, "source") : 
  trying to use CRAN without setting a mirror
Calls: <Anonymous> ... withVisible -> eval -> eval -> install.packages -> contrib.url
Execution halted
```

Your markdown file includes a command to install a package (something like `install_packages()`. You should comment out the command or delete it.



## Cannot upload output to Blackboard

Blackboard can only accept .doc or .pdf files. If you want to upload an html file, you must compress it first and upload a `zip` file instead.







