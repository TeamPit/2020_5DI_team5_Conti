# Software Requirements Specifications

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABLUAAAACCAIAAAAhJ3mxAAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAACA773I2j4AAACwbwCxlwXLwNuWHAAAAABJRU5ErkJggg==)

Version 1.0,

prepared by TheFlippedCompany



Table of Content

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABN0AAAACCAIAAADjFz01AAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAAAAlrzI2j4AAADwrwHEUwXL08N7EgAAAABJRU5ErkJggg==)

1. Introduction_[pag. 2]_1 Overview

1.2 Goals

1.3 Definitions

1. General Design Constraints_[pag__. 3]_1 OnGo Application Environment

2.2 User Characteristics

2.3 Mandated Constrains

1. Nonfunctional Requirements _[pag. 4]_1 Operational Requirements

3.2 Performance Requirements

3.3 Security Requirements

3.4 Documentation and Training

3.5 ​External Interface

3.5.1 User Interface

3.5.2 Software Interface

1. Functional Requirements _[pag. 6]_1 Required Features

4.1.1 Use Case 1 - Create a Folder

4.1.2 Use Case 2 - Tranfer a file to the origin

4.1.3 Use Case 3 - Require a file from the origin

4.2 Optional Features

4.2.1 Use Case 1 - Send a command from a CLI

4.2.2 Use Case 2 - Create a file with content







​Pag. 1

1. Introduction

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABN0AAAACCAIAAADjFz01AAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAAAAlrzI2j4AAADwrwHEUwXL08N7EgAAAABJRU5ErkJggg==)



**1.1** ​ **Overview**

The OnGo is an application that provides you access to all the files stored on your personal computer from ​_any device__​_you want.

This document provides informations on the requirements for the OnGo application.

Project goals, scope and definitions are given in the ​_introduction__​_.

_Design constraints __​_and​_application environment__ ​_are described in the followingsection.

_Nonfunctional requirements__​_are outlined for later verification.

_Functional requirements__​_are given to show the system features and expected userinteraction.

The ​_Software Project Management Plan__​_will give specifics on project budget and schedule.

**1.2** ​ **Goals and Objectives**

The main objective of this project is to allow users to have an easy and quick access to any file stored on other devices. The OnGo application is expected to:

- .function in an simple and intuitive manner

- .provide an easy access to the user&#39;s files without uploading them first, as cloud services require to.
- .work on any operative system and device

**1.3** ​ **Definitions**

Origin - It&#39;s the computer on which files are ​_actually __​_stored, your &quot;​_home pc__ ​_&quot; if you want to.

User - It&#39;s the person that&#39;s trying to get to the ​_origin__​_via OnGo





​Pag. 2

## 2. General Design Constrains

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABN0AAAACCAIAAADjFz01AAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAAAAlrzI2j4AAADwrwHEUwXL08N7EgAAAABJRU5ErkJggg==)



**2.1** ​ **Application Environment**

The OnGo product includes:

- .A desktop application of our design that has to be installed on the _origin_ system

- .A web application of our design that is used by the _user __​_to interact with his own registered _origin__ ​_system

Both applications interact with our ​[Web Api](https://us-central1-web-ftp-ongo.cloudfunctions.net/api)​that will handle the communications between the user and the corresponding origin.

**2.2** ​ **User Characteristics**

Users will need to have a valid ​[account](https://www.theflippedteam.altervista.org/)​in order to download the OnGo origin program and they will also need to use their accounts to log into the user web application in order to use it. There is ​_no limitation__​_on the device that the user can use.

**2.3** ​ **Mandated Constrains**

The whole system has to work via HTTP connection (https). This is mandatory because the ​_origin__​_machine will probably be inside a private network and it might not be allowed to host a server accessible from the public internet due to several security issues or privacy policies.





















​Pag. 3

3. Nonfunctional Requirements

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABN0AAAACCAIAAADjFz01AAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAAAAlrzI2j4AAADwrwHEUwXL08N7EgAAAABJRU5ErkJggg==)



**3.1** ​ **Operational Requirements**

The user web application has to provide an easy to use interface and should be simple enough to let every user connect to it&#39;s own origin without any serious problems.

The origin main application has to generate and give the code to the user in the most clear way possible. The user will still need to remember that code by himself.

**3.2** ​ **Performance Requirements**

When a file is ​_downloaded __​_/ ​_uploaded__ ​_, the system has to deliver the whole document without losing any part regardeless of the file dimension.

**3.3** ​ **Security Requirements**

The first versions of the OnGo application will only require:

- .User login and registration (to download the origin application and to use the user web app)

**3.4** ​ **Documentation and Training**

The OnGo application ​_itself__​_will not include any documentation or training for the final user but video tutorials will be available on the ​[team website](https://www.theflippedteam.altervista.org/)​and on the official [YouTube channel](https://www.youtube.com/)​.

**3.5** ​ **External Interface**

**3.5.1** ​ **User Interface**

The interface will be ​_eye-catching __​_in order to let the user interact with a ​_familiar__ environment__​_.

The interface will be easy to use on any device since it will resemble a ​_Windows-like __operating system UI__ ​_.



Pag. 4

**3.5.2** ​ **Software Interface**

The ​[OnGo Api](https://us-central1-web-ftp-ongo.cloudfunctions.net/api)​works as an interface between the origin application and the user application. It handles and direct all the communications between the ​_users __​_and their corresponding ​_origin__ ​_system.





















































Pag. 5



4. Functional Requirements

 ![](data:image/*;base64,iVBORw0KGgoAAAANSUhEUgAABN0AAAACCAIAAADjFz01AAAAK0lEQVRYhe3OSQ0AIAwAMEjw73bHczL2oFXQG9kHAAAAlrzI2j4AAADwrwHEUwXL08N7EgAAAABJRU5ErkJggg==)



**4.1** ​ **Required Features**

**4.1.1** ​ **Use Case 1**

Description: Create a new folder and navigate inside it

Actors: OnGo ​_User_

Basic path ​_origin__​_:

1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code

1. The user can now decide when to start working on his other devices

Basic path ​_user__​_:

1. The user goes to [ur website](https://www.theflippedteam.altervista.org/)
2. The user clicks on the _OnGo Application Icon_

1. The user _logs into__​_his account

1. The user prompts the _previously given__​_code

1. The system provides an _accurate view__​_f the user&#39;s origin system

1. The user navigates to the desired folders by _double-clicking__​_n them

1. To create a new folder, the user _right-clicks __​_n the page and clicks on &quot;_New__ folder__​_&quot;

1. The user decides a proper name and then clicks _create_

1. A new folder has just been created on the origin system

















Pag. 6

**4.1.2** ​ **Use Case 2**

Description: Transfer a file from the User to the Origin

Actors: OnGo ​_User_

Basic path ​_origin__​_:

1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code

1. The user can now decide when to start working on his other devices

Basic path ​_user__​_:

1. The user goes to [ur website](https://www.theflippedteam.altervista.org/)
2. The user clicks on the _OnGo Application Icon_

1. The user _logs into__​_his account

1. The user prompts the _previously given__​_code

1. The system provides an _accurate view__​_f the user&#39;s origin system

1. The user navigates to the desired folders by _double-clicking__​_n them

1. To transfer a document, the user _drags and drops__​_the desired file from the local system to the web application

1. A new file has just been transfered to the origin system































Pag. 7

**4.1.2** ​ **Use Case 3**

Description: Require a file located in the Origin as a User

Actors: OnGo ​_User_

Basic path ​_origin__​_:

1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code

1. The user can now decide when to start working on his other devices

Basic path ​_user__​_:

1. The user goes to [ur website](https://www.theflippedteam.altervista.org/)
2. The user clicks on the _OnGo Application Icon_

1. The user _logs into__​_his account

1. The user prompts the _previously given__​_code

1. The system provides an _accurate view__​_f the user&#39;s origin system

1. The user navigates to the desired folders by _double-clicking__​_n them

1. The user, to require a file, _right-clicks __​_n the desired document and clicks on &quot;_Download__ ​_&quot;

1. After a few seconds, the required file is downloaded on the user&#39;s system





























Pag. 8

**4.2** ​ **Optional Features**

**4.2.1** ​ **Use Case 1**

Description: Send a full proper command through a DOS emulator. Computer shutdown from CLI

Actors: OnGo ​_User_

Basic path ​_origin__​_:

1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code

1. The user can now decide when to start working on his other devices

Basic path ​_user__​_:

1. The user goes to [ur website](https://www.theflippedteam.altervista.org/)
2. The user clicks on the _OnGo Application Icon_

1. The user _logs into__​_his account

1. The user prompts the _previously given__​_code

1. The system provides an _accurate view__​_f the user&#39;s origin system

1. The user clicks on the _CMD__​_icon on the top-left corner

1. A CLI will appear in the view and the user will be able to send proper commands
2. To shut the system down in 60 seconds, the user types _sudo shutdown -s -t__60_

1. The system will be shut down and the connection will be closed

**4.2.2** ​ **Use Case 2**

Description: Add a new file with content in it

Actors: OnGo ​_User_

Basic path ​_origin__​_:

1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code

1. The user can now decide when to start working on his other devices





Pag. 9

Basic path ​_user__​_:

1. The user goes to [ur website](https://www.theflippedteam.altervista.org/)
2. The user clicks on the _OnGo Application Icon_

1. The user _logs into__​_his account

1. The user prompts the _previously given__​_code

1. The system provides an _accurate view__​_f the user&#39;s origin system

1. The user navigates to the desired folders by _double-clicking__​_n them

1. To create a new file, the user clicks on the _Notepad__​_icon on the top-left corner

1. When the web editor loads up, the user will be able to type and save the document in the desired format by clicking the &quot;_save__​_&quot; button
2. The user will then type the desired name and extension in the modal

1. A new file with content _has been added__​_to the origin system in the desired path











































Pag. 10
