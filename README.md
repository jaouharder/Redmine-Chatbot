
![redchatlogo2](https://user-images.githubusercontent.com/58748867/82519266-c976a780-9b10-11ea-8bb6-c25d4aaed1a4.png)

### Table of Contents
 
- [Description](#description)
- [Requirements](#Requirements)
- [How to install](#How-to-install)
- [Quick start](#Quick-start)
- [Authors information](#Authors-information)

---

## Description

This chatbot is made using Xatkit bot platform, in this chatbot we can interact with [redmine project management](https://www.redmine.org/) using their java based API 
here's examples of what she can do :

1.Creating an account or login using API ACCESS KEY

2.View all or specific users (requires admin privileges)
+ To view all of them type *view all users*
+ To view details about a user type *show* **HisFirstName HisLastName** *details*

3.Create new projects (requires admin privileges)
+ type *create project*

4.View all or specific projects
+ To view all of them type *show all projects*
+ To view details about a projet type *show project* **ProjectName**

5.Update an existing project(If user is an admin)
+ type *I want to update a project*

6.Create new issues (requires admin privileges)
+ type *create* **IssueName** *in project* **ProjectName**

7.View all or specific issues
+ To view all of them type *show all* **ProjectName** *issues*
+ To view details about an issue type *show issue id =* **IssueID** *details*

8.Update an existing issue (requires admin privileges)
+ Type *On issue id=* **IssueID** *update* **WhatToUpdate** *:* **UpdatedValue**
+ WhatToUpdate can be *privacy*, *estimated_hours*, *tracker* or *priority*

9.Create new group and add users to it (requires admin privileges)
+ To create group type *Create group using name* **GroupName**
+ To add users type *on group* **GroupID** *add user* **UserID**
+ To show all groups type *show all groups*

10.Assign group or user to project (requires admin privileges)
+ Type *I want* **USERID/GROUPID** *to work in project* **ProjectName**

## Installation

### Requirements

+ [Xatkit](https://github.com/xatkit-bot-platform/xatkit/wiki/Build-Xatkit)


### How to install

+ Download or clone this repository 
+ Cut and paste or extract Redmine-Chatbot-master **folder COMPONANTS** (examples, bin and plugins) in ```xatkit-directory/build``` (allow to replace) 

### Quick start

On Redmine go to ***Administration --> SETTINGS --> API*** and make sure that ***Enable REST web service*** is enabled

To start the chatbot :

***On windows*** 

Open Git Bash as administrator and change the current working directory to xatkit directory and type :

```git
    cd build/bin/

    ./start-xatkit-windows.sh ../examples/RedmineExample/RedChat.properties
```
***On Ubuntu***

Navigate to ```xatkit/build``` directory and type :

```git
    cd bin/

    ./start-xatkit-linux.sh ../examples/RedmineExample/RedChat.properties
```


Open your browser and navigate to http://localhost:5000/admin to test it

[Back To The Top](#Redmine-Chatbot)

---
#### Authors information
Done by 

[DERROUICH Jaouhar ](https://www.facebook.com/jaouharderrouich/)

and

[Outtaleb Mohamed ](https://www.facebook.com/mohamed.naya/)

Under supervision of 

 EL HAMLAOUI Mahmoud
 
[Back To The Top](#Redmine-Chatbot)

___
