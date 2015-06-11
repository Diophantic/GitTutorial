# Git tutorial

There are numerous git tutorials out there already, so why create another one? Basically this tutorial is a way for me to extract and test all the knowledge I have about git and merge it with GitHub so that other people, mostly from IQuality, can share this knowledge with me.

This article is not about source control ing eneral. I will not focus on propper project management whilst using a SCMS; but this articel is about how to technically use git in small to large projects. I will address merging, cloning and GitHub and I'll try and focus on the technical issues and choices you must make.

## git init
It all starts with the command ```git init```. This command initializes a git database in a local directory on your computer. Imagine that the ```~``` sign in a path means your personal directory in your preferred OS. Now imagine, if you are running on Windows that you've created an alias for the ```dir``` command called ```ls``` and now we are good to go.

## git add
Whenever you add, remove or change a file this file will be staged for the next commit. Because we do not want to to willy nilly commit every change we make we will have to tell git which changes to commit. We can do this with the ```git add <filename>``` command. If you want to add every change of the current working tree you can use ```git add .```

It is of course possible to git a specified path or pattern to the files you want to add, so if, for example, you only wanted to add the ```*.js``` files after you run some sort of compiler or transpiler you might want to do: ```git add **/*.js```.

## git commit
After the index of the working tree has been updated to include your targeted changes you can commit your changes. This will 
store the current contents of the index in a new commit along with a log message from the user describing the changes. In less technical terms this means that we can commit the changes to our git database allong with a message explaining the changes. For example, we can commit our previously updated index like so: ```git commit -m "Fixed a bug in the routing engine"```.



