================
**KookaBlockly**
================


A stand-alone graphical visual editor for the Kookaberry
This document provides a quick overview of KookaBlockly.  More detailed information about KookaBlockly 
may be found the KookaBlockly Reference Guide.


Installing KookaBlockly
-----------------------

KookaBlockly runs as a stand-alone program on a Windows 10 or MAC based personal computer.  
The latest version of KookaSuite, which includes KookaBlockly, can be downloaded 
from the Kookaberry Github repository - 
https://github.com/Kookaberry



Introduction
------------

KookaBlockly is a stand-alone graphical, drag and drop, editor for the Kookaberry and related microprocessor 
boards.  It is based upon the open source Google Blockly (Apache 2 license) which is a library from Google 
for building beginner friendly programming languages.  It was written by Damien George 
( George Robotics – MicroPython)  in conjunction with Kookaberry Pty Ltd, the AustSTEM Foundation and 
supported by the Warren Centre and the Vonwiller Foundation.

KookaBlockly allows the creation of syntactically correct scripts and programs even if the user does not 
know any program language.  KookaBlockly converts the assembled graphical blocks into structured MicroPython 
(Python 3.0) code which is then able to be saved, downloaded and / or run on a Kookaberry, Raspberry Pi Pico 
or related RP2040 boards

Working with KookaBlockly allows the user to drag and drop graphical code blocks into a workspace.  
The blocks can be graphically interlocked or snapped together using sockets (socketed) to represent code 
concepts such as program controls (activation, termination, loops and decisions), actions, and result 
computations (variables, values, mathematical and logical expressions).  This graphical process allows 
users to apply programming concepts and principles to designing scripts or programs without having to be 
concerned about the syntax and semantics of MicroPython.


Using KookaBlockly
------------------

**Download KookaSuite** 

Download KookaSuite from the GitHub repository and install on a Windows 10 or 11 PC or on a MAC.

**User Screen Display**

Run KookaBlockly on your computer and the following screen display will be presented.

.. image:: images/KB_Init_Display.png
    :alt:  Initial Display
    :width: 640px

*Revision Level*    -   The Revision Level of KookaBlockly is shown at the top left-hand side of the display

*Task Bar*     
            The Task bar is divided into two areas.  The first area comprises script command buttons 
            on the left-hand side of the display.  With the second area comprising, display and script 
            loading commands on the right-hand side of the display.

            With the second area comprising, display and script loading commands on the right-hand side of the display.


.. image:: images/Command_Buttons_left.png
    :alt:  Command Buttons left-hand
    :width: 500
    :height: 150
    :align: center
                 
            
.. image:: images/Command_Buttons_Right.png
    :alt:  Command Buttons right-hand
    :width: 500
    :height: 150
    :align: center

The individual button controls are described in the following paragraphs

**New** button 

This button starts a new script and any script on the display will be cleared. Move the cursor 
to this button, press click on the mouse and the following will be displayed.

.. image:: images/Start_New_Pgm.png
    :width: 300
    :height: 150
    :align: center
    :alt: Start New Program ?

Press **Yes** to start a new script / program or **No** to revert.  Caution - this will erase the current workspace and any 
work not saved will be lost.  Please be careful to save any work that is to be retained.

**Load** button

This button allows the user to select a KookaBlockly program to be loaded into the Workspace.  Move the cursor to this 
button, press click on the mouse and the following file dialogue will be displayed:

.. image:: images/Load_Display.png
    :width: 400
    :height: 200
    :align: center
    :alt: Load button display

The default directory within the current user’s account is /KookaberryScripts/KookaBlockly and the user can navigate away 
from this as desired.  Selecting a script and pressing the **Open** button, or alternatively double-clicking on a selected 
KookaBlockly script will place a copy of that script in the KookaBlockly Workspace from where it can be modified, saved 
and run on the Kookaberry.

If the workspace is not empty, and new KookaBlockly script is loaded, it will be added to the current workspace.  This is 
useful where frequently used snippets of KookaBlockly are stored away in their own script files for reuse in other scripts.

**Save** button

This button allows a user to save a script that is in the Workspace.  Move the cursor to this button, press click on the 
mouse and the following will be displayed:

.. image:: images/Save.png
    :width: 300
    :height: 200
    :align: center
    :alt: Save screen pane

The default directory is  /KookaberryScripts/KookaBlockly within the current user’s account and the user may navigate 
away from this as desired.  After typing in a name for the script, or clicking on a pre-existing script to be overwritten, 
then pressing Save the KookaBlockly script will be saved in the selected directory.  Note:  In saving a KookaBlockly script 
KookaBlockly will add a .kby to the file identify the file as one that can be loaded onto KookaBlockly.  A typical file name 
could then be say test.kby.py































