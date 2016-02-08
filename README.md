# RoomEase
==========

Hi! This is the documentation of the RoomEase app.

----------------------
## USER

### Description of the Project:
RoomEase is a roommate communication app that makes communicating with roommates and managing your household a lot easier. It provides five main features: reserving household items or places at certain times, writing shared lists among roommates, managing fridge content, scheduling chores, and a reminders feed. We are well ahead of our competitors because of our cross-platform compatibility, by being an all-in-one app, and for the uniqueness of the features we support. 

*Available on both Android and iOS.*

### Obtaining the App: 
Currently, you can obtain RoomEase only on Android 4.0 of higher, by downloading the .apk file externally then installing it on your phone.

Obtaining and installing our app is as easy as one, two, three:

1. **Enable “unknown sources” on your phone.**

   Android is defaulted to forbid installing apps downloaded from outside of Google Play Store. To change that go to *Settings >          Security*, then check the box right next to *unknown sources.* Your phone now will allow apps to be installed from sources other       than the Play Store.

2.  **Download RoomEase.apk file on your Android.**

   Click here (TODO: add hyperlink) to download RoomEase.apk on your device. You could either download it directly from your phone browser or download it on your home machine then import it to your phone.

3.  **Install RoomEase.apk file.**
   Navigate to the directory where you saved RoomEase.apk. If you have not selected a specific directory then it will be available in *Downloads.* Press the app’s icon and an installation screen will pop-up. Tap *Install* and proceed with the installation. If Android was to issue any warnings during installation, ignore them and proceed.

Congratulations! Now you have RoomEase up and running on your device.

### Using the software: 

RoomEase consists of multiple views, each represents one of its main features. You can switch between views to add, modify, or delete items. Interacting with the app comes exclusively by pressing or hold-pressing items, and by typing. Although the different views look different, interactions with them are almost identical. Check the Using the software section for more info about how to use the RoomEase app.

To run RoomEase, you need to have an active Facebook account. After you have successfully downloaded and installed the app, you
should be able to access it by tapping on the RoomEase icon. RoomEase’s main screen will prompt you to login with your Facebook       account, click “login with Facebook” and type your login cardinals then hit “proceed.”  

![TO DO: GET WORKING PIC LINKs:](https://drive.google.com/file/d/0B90H4BTOhXjoaDN6ck5hZXNxWTA/view?usp=sharing)

The app’s main page is the **Feed** page. It will provide the user with a scroll-down list of nearly-expired food, approaching chores, today’s completed chores, and today’s reservations. At the bottom of the page, or by swiping left, you can choose from the Fridge View, the Chores View, the Reservation View, and the Lists View.

![TO DO: GET WORKING PIC LINKs:](drive/mockups/Fridge-01.jpg)

On the **Fridge View**, you could toggle left to see your own food, or right to see the apartment’s shared food. Press-holding on any fridge item will allow you to modify it or delete it. Press-holding an expired item will give you the extra option of adding it to your grocery list.

![TO DO: GET WORKING PIC LINKs:](drive/mockups/List-01.jpg)

From the **List View**, and every other view, you can tap on the big red plus sign on the bottom right allows you to add items to the displayed view.

![TO DO: GET WORKING PIC LINKs:](pic: drive/mockups/Scheduler-01.jpg )

On the **Scheduler View**, scheduled items and places are going to be displayed in order, nearest first. You either could add normally from the plus sign on the bottom right or choose to reserve a specific item by clicking on its icon on the top right.
For any more queries check our Reporting Bugs section.

### Reporting Bugs: 

In the rare case of bugs, please fill out [this form](https://docs.google.com/forms/d/1WoumJ1cuiM6K2ZyKYfMbsn028SNex2NL8RquFs0IH9I/edit)

It would be helpful, for us and for you, to consult a guide on how to write a good bug report before filling out the form. It will help you make your problem clearer and makes it easier for us to deliver a solution in no time. We suggest Oracle’s article on [How to Write a Good Bug Report](http://www.oracle.com/technetwork/articles/javase/bugreport-howto-135155.html). 






---------------------------
## DEVELOPER

### Obtaining source code:

First, ensure you have git installed. If not, run the following command: 
```
sudo apt-get install git-all
```
Then, run the following command: 
```
git clone https://github.com/roomeasedev/RoomEase.git
```


### Building From Source:
Since this project is a multi-platform project, there may be some additional
software that may need to be installed depending on the target platform.

First, ensure you have node.js installed by running
```
node -v
```
If not, run the following commands
```
sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install npm
```
Next, install phonegap (cordova) by running the following commands:
```
sudo npm install cordova -g
```
* *Note: There may be some modules that are not part of cordova by default that need to be installed manually.*
   *We personally had to run the additional command* `sudo npm install -g bplist-parser`
* *Also note: Depending on the version of node, you may see the following error:* 
    `The program ‘node’ can be found in the following packages.` 
    *To fix this, run the following command:* `sudo ln -s /usr/bin/nodejs /usr/bin/node`
`

Phonegap allows us to work with nearly any platform we want. To add a platform to build to, at the top directory 
of your project (you should see a config.xml) and run 
```
cordova platform add android
```
*To add the resources for ios, change from ios to android. There are more platforms than this that can be built to.*

Now to build to android run
```
cordova build android
```
You may see some errors regarding not having the correct versions of the android SDK installed. Usually these can be resolved by installing the android SDK and installing the latest SDK tools.

Great! If everything went well, the console should display where your .apk was built to! Try running it on your phone. You may or may not be able to receive any server data, for this app requires a database to operate. The testing plan gives some information on how the database works. You can run the server on localhost or on a hosted web service. We found it easy to use Azure and a virtual machine.


### Testing:

TO DO: Describe automatic testing
Describe automatic testing plan

RoomEase uses a NoSQL backend known as CouchDB. CouchDB can run on any server backend or on LocalHost. Typically, couchDB will run on localhost:5984 (we will assume this for our testing purposes). Below are the current steps to install CouchDB on a local machine. Be sure to have CouchDB running when running these tests. 


### Bug Tracking:
For all active/known bugs, please refer to [this spreadsheet](https://docs.google.com/spreadsheets/d/1TUz7qx3GqziUEGzJB6NABSbTz8rprz-C40Qe7xVgVIM/edit#gid=0)
