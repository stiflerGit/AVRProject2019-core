# XVR-FirstPersonShooter



This project was born to accomplish the Virtual and Augmented Reality Class project assignment.



# Requirements



Starting from a base code the assignment requests to accomplish some points:



1. Improve collision detection

2. Implement shooting:

   - finite number of bullets

   - implement reload

   - implement collision detection bullet-enemy for all entities

   - implement multiple weapons:

     - railgun: faster but smaller radius of influence, 1 damage point

     - rocket launcher: slower but bigger, 5 damage point

    - implement collision detection bullet-walls

3. Random spawn of players (NOT INSIDE THE WALLS)

4. Implement walls of different height (use numbers in the level.txt)

5. Implement climbing, to go down: jumping, falling down or blocking

6. Implement first-person view

7. Implement multiplayer via networking



# Prerequisites

## Install XVR Developer Studio

**XVR Developer Studio** is needed to compile and run the project:

[XVR Developer Studio](https://sourceforge.net/projects/xvrstudio/)



## Project import



After installing XVR Developer studio we can import the project. To import the project follow steps below:



1. go to you XVR Developer Studio workspace and clone the repository `cd workspace/xvr; git clone https://github.com/stiflerGit/XVR-FirstPersonShooter.git`

2. from the main XVR DS window click *File*->*Import*

3. In the import window click on *Open an XVR 2.0 project in the workspace* and then on *Next*.

4. Select *Select root directory* click on browse and select the main project folder (XVR-FirstPersonShooter). In *Options* **check only *Search for nested projects***, ***Copy projects into workspace* and *Hide projects that already exist in the workspace* must be unchecked**. Now you can click on *Finish*.

5. You will see three new projects in the XVR workspace bar.



# Compile and Run



The project itself is divided into two further subprojects: **client** and **server**



To run the game:

1. Make sure that definiton of costants **CONF_SERVER_ADDRESS**, **CONF_SERVER_PORT**, **CONF_MAX_NPLAYERS** in the **AVRProject2109-server.s3d** file are equal to the same definitions in the **AVRProject2109-client.s3d** file.

2. Make sure contant **CONF_MULTIPLAYER** in the **AVRProject2109-client.s3d** file is set to **true**.

3. Run the Server, by clicking with the right button on the server project in the workspace view and click on run or debug. Wait for the server to be ready.

4. Run another instance of XVR Studio Developer and run the client (right-click on client project in the workspace view -> Run).

5. To connect other clients open other instances of XVR Developer Studio and run other clients.



## Single player

You can also run the client without connect to the server, just set **CONF_MULTIPLAYER** in the **AVRProject2109-client.s3d** to **false**.



However, this functionality is used only for debug scope, indeed bullets collisions with walls are not managed in this mode
