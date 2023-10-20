================
**KookaBlockly**
================


A stand-alone graphical visual editor for the Kookaberry
This document provides a quick overview of KookaBlockly.  More detailed information about KookaBlockly 
may be found the KookaBlockly Reference Guide.



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


Installing KookaBlockly
-----------------------

KookaBlockly runs as a stand-alone program on a Windows 10 or MAC based personal computer.  
The latest version of KookaSuite, which includes KookaBlockly, can be downloaded 
from the Kookaberry Github repository - 
https://github.com/Kookaberry

Using KookaBlockly
------------------

**Download KookaSuite** 


Download KookaSuite from the GitHub repository and install on a Windows 10 or 11 PC or on a MAC.

**User Screen Display**


Run KookaBlockly on your computer and the following screen display will be presented.

.. image:: images/KB_Init_Display.png
    :alt:  Initial Display
    :width: 640px
    :align: center


* *Revision Level* 

            The Revision Level of KookaBlockly is shown at the top left-hand side of the display

* *Task Bar*     
            The Task bar is divided into two areas.  The first area comprises script command buttons 
            on the left-hand side of the display.  With the second area comprising, display and script 
            loading commands on the right-hand side of the display.

            With the second area comprising, display and script loading commands on the right-hand side of the display.


.. image:: images/Command_Buttons_left.png
    :alt:  Command Buttons left-hand
    :width: 500
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

**Print** button

This button allows a user to print a script that is in the current Workspace.  Move the cursor to this button, press 
click on the mouse and the following will be displayed.

.. image:: images/Print_Display.png
    :width: 350
    :height: 300
    :align: center
    :alt: Print display pane

A printer may now be selected and the script printed.
Note - only the visible area of the workspace will be printed.  Zoom the view of the KookaBlockly script in or out to 
size it appropriately for printing.  The Print dialogue provides a preview of the page to be printed.

**Run** button

This button allows a user to run a script that is in the current Workspace on the attached Kookaberry.  Move the cursor 
to this button, ensure that a Kookaberry is connected via the USB port, press click on the mouse and the script will 
be sent to the Kookaberry and run.

**Stop** button

This button allows a user to Stop a script that is currently running on the Kookaberry.  Move the cursor to this button, 
press click on the mouse and the currently running script on the Kookaberry will stop.

**Serial** pane and drop down list

This display shows whether a Kookaberry is connected to the USB port of the computer and the serial port being used.  
“Auto-connect” shows that the PC / KookaBlockly is waiting for a Kookaberry to be connected to the USB port.  When a 
Kookaberry is connected the Serial: will show the com: port connection such as Kookaberry on \\.\COM8.  The com: port 
selected will be automatically selected via the operating system of your computer.
If, on rare occasions, the Kookaberry becomes unresponsive, click on the drop-down list and select the Auto-connect 
option to cause the connection to be renewed.

**Scripts** pane and drop down lists

Press the down arrow in the Scripts pane and select from the available folders. Scripts is the default folder and 
users may create additional folders.

.. image:: images/Scripts_Folders.png
    :width: 350
    :height: 150
    :align: center
    :alt: Scripts folder dropdown selection

The pane to the right of the Scripts folder selection gives access to available scripts

.. image:: images/Scripts_Avail.png
    :width: 350
    :height: 250
    :align: center
    :alt: Available scripts drop down menu selection

Pressing the down arrow shows the available scripts that may be downloaded to the KookaBlockly Workspace.  Moving the 
cursor over the desired script and clicking will load the selected KookaBlockly script to the KookaBlockly workspace.  
The loaded KookaBlockly script will replace the contents of the current Workspace.  Please ensure that any unsaved work is 
saved prior to using the Scripts list to load.  This behaviour differs from using the Load button where the KookaBlockly 
is added to the current workspace.

**Show Script** button

This button allows a user to display the MicroPython script generated from the graphical script that is in the KookaBlockly 
workspace.  Move the cursor to this button and press click on the mouse and the MicroPython script will be displayed.  
The size of the display pane showing the script can be adjusted by clicking on and dragging the edges of the script window 
using the cursor.

**Show Display** button

This button allows the user to show what is being displayed on the attached Kookaberry’s display in a small pane on the 
computer’s display.  Move the cursor to this button, press click on the mouse and the display will appear on the computer 
in a separate window.  The size of this window can be adjusted by the user by clicking on and dragging the window edges 
using the cursor.

Buttons A, B, C and D replicate the buttons on the Kookaberry and may be used on the Display to in a similar manner to 
the Kookaberry.

The Kookaberry Reset button performs a software reset to the Kookaberry.

The Kookaberry Menu displays the internal Kookaberry menu


*Workspace*

The Workspace is the area where the graphical blocks are dragged and dropped to.  A MicroPython script is automatically 
generated from the graphical blocks in the Workspace.

*Sliders*

Sliders are on the bottom and the right-hand side of the KookaBlockly display and can be used with the mouse to reposition 
the blocks on the KookaBlockly display. An alternative method is to click the cursor on a blank area in the workspace 
and drag it until the script is conveniently positioned.



*Icons* located on bottom right of the workspace

.. image:: images/Target_Icon.png
    :width: 50
    :height: 50
    :align: center
    :alt: Target icon

This icon centres the graphical display that is in the current workspace.  
Hover the cursor over the icon and click the mouse.  The workspace graphical blocks will be centred.

.. image:: images/Zoom_Icon.png
    :width: 50
    :height: 70
    :align: center
    :alt: Zoom icon

This icon allows the user to zoom in or out on graphical blocks.  It can be used in conjunction with the sliders to 
position blocks in the workspace.  Alternatively use the wheel on the mouse to zoom in and out.

.. image:: images/Recycle_Icon.png
    :width: 80
    :height: 80
    :align: center
    :alt: Recycle Bin icon

This is the Recycle Bin icon.  KookaBlockly blocks can be dragged and dropped 	into the bin 	to delete them.  
Blocks remain in and can be retrieved from the Recycle Bin by dragging 	until KookaBlockly is closed.


**Categories**

There are a number of **Categories** of blocks located on the left hand side of the KookaBlockly workspace.  These Categories contain 
**blocks** that can be selected and placed in the Workspace.

A **Category** can be selected by placing the cursor over the Category and making a single click.
Some categories contain standard Blockly blocks whilst others contain blocks specific to the Kookaberry

The *Categories** may be summarised as follows:

.. image:: images/Category_List.png
    :width: 200
    :height: 300
    :align: center
    :alt: Category list


* *Control*

The Control category mostly contains blocks that are standard within Blockly with the exception of the blocks used to get 
the Real Time Clock (RTC) information from the Kookaberry.

* *Clock*

The Clock category allows access to both the internal clock and an external clock based on the DS3231 clock. The internal 
clock is set to the time set in the PC at the time of running KookaBlockly.  This time may be set and read for use within 
scripts.  An external clock based on the DS3231 clock may be set and read.

* *Display*

The Display category contains blocks that are used for the Kookaberry display

* *Buttons*

The Buttons category contains blocks that are used to control the four buttons, A, B, C and D, on the Kookaberry board.

* *LEDs*

The LEDs category contains blocks that are used to control the here LED’s, Red, Orange and Green, on the Kookaberry board.  
It is also used to control Neopixel LED displays.

* *Pins*

The Pins category contains blocks that control the I/O pins on connectors P1, P2, P3, P4 and P5 on the Kookaberry board.  
The blocks facilitate the assignment of GPIO functions to the pins as well as analogue inputs to P1, P2, P4 and P5.  
Pulse Width Modulation (PWM) may be assigned to the pins on connectors P1, P2, P3, P4 and P5.

* *Sensors*

The Sensor category contains blocks that allow for different sensors to be used with the Kookaberry.  The blocks allow 
usage of the internal accelerometer and compass as well as external connection of DHT11 and 22 temperature and humidity 
sensors plus a DS18x20 sealed temperature sensor as well as a Negative Temperature Coefficient (NTC) temperature sensor.

* *Actuators*

The Actuators category contains a block that allows the connection off a small hobby servo to connectors P1, P2, P4 and P5.
Both the 180 and 360 degree Hobby Servos are supported.

* *Radio*

The Radio category contains blocks that allow use of the Nordic nRF51 and nRF52 packet radio.  It also supports the HC-12 
radio via a serial UART port.

* *Logging*

The Logging category contains a block that allows for a dat.csv file to be created for the purpose of logging data.  
The dat.csv file may be displayed on a spread sheet.

* *Boolean*

The Boolean category contains blocks that perform standard logical operations of Blockly

* *If-Else*

The If-Else category provide the standard logical loop functionality of Blockly. The blocks may be customised by the user.

* *Loops*

The Loops category provided the standard loop facility of Blockly.

* *Strings*

The Strings category provides blocks that allow strings to be text, an integer and or a floating point number.

* *Lists*

The Lists category provides the standard Blockly blocks that a allow working with lists with a list being a set of 
variable of any type.

* *Math*

The Math category provides blocks that allow working with numbers.  It also provides a block for scaling a number.

* *Variables*

The Variables category provides a block that allows a user to define a variable

* *Functions*

The Functions category provided blocks that allow users to create and call functions which can be 
useful for structuring and multiple use of repeatable logic.

* *Advanced*

The Advanced category provides blocks for importing MicroPython code into KookaBlockly


**Using KookaBlockly**
----------------------

KookaBlockly is a graphical visual editor based upon Google Blockly.  It allows program scripts to be constructed visually 
by connecting blocks together by users who have little or no programming skills. Blocks are divided into colour-coded 
categories according to their purpose or function and snap together into sockets like a jigsaw pieces.  The shapes of the 
blocks vary and not all blocks will snap into a socket of another block.  

If the blocks fit together the scripts will still run and KookaBlockly will generate syntactically correct code.  However 
logical errors can still arise.

KookaBlockly contains three basic block shapes:

* **A C-shaped block**

        A C-shaped block directs program flow and contains a sequence of action blocks. The C-shaped block may be a loop, 
        or may be a sequence of blocks that are run conditionally subject to one or more logical tests.

.. image:: images/C_Shaped_Block.png
    :width: 375
    :height: 140
    :align: center
    :alt: C Shaped Blocks


* **An Action or "do" block**
  
        An action or “do” block which performs an operation.  The block has an indent in the top border and a matching 
        protrusion on the bottom border.  These blocks click together like jigsaw pieces and may be placed in a vertical 
        column and within a C-shaped block.



.. image:: images/Action_Block.png
    :width: 300
    :height: 200
    :align: center
    :alt: Action Block

* **A Value block**

        A value block which has a jigsaw tab on the left-hand edge.  These blocks evaluate an expression and assign an 
        output value to the blocks to which they are connected.  Some value blocks have a matching receptacle on the 
        right-hand edge which accepts other value blocks.


.. image:: images/Value_Block.png
    :width: 400
    :height: 200
    :align: center
    :alt: Value Block


* **Block Selection**
        

        Blocks are selected by first selecting a category and then clicking on a block.  The block will be placed or can 
        be dragged and dropped into the workspace and can then be moved around via the cursor.   The action is to click 
        on a block and hold the mouse down.  Then drag and drop the block on the workspace.  If the block is close to a 
        compatible block it will snap into a socket with an audible click.  If there is no click then the blocks are not 
        compatible.

        Holding the cursor over a block and right clicking the mouse will bring up a menu which allows further management 
        of the block.  The following is an example of such a menu.


.. image:: images/Management_Block.png
    :width: 300
    :height: 200
    :align: center
    :alt: Management Block

*Duplicate*

        Click on Duplicate to create a duplicate of the block and any connected sub-blocks in the workspace.  Sub-blocks 
        for example are all the blocks nested within a control block, or any value blocks connected to an action block.

*Add Comment*

        Click on Add Comment and a circle with a question mark will appear in the block.  
        Click on the question mark and an area pane is provided for a user to enter in a comment.  
        This comment will be included in the MicroPython script generated by KookaBlockly. 
        Comments are very useful for describing parts or portions of the script for later reference by subsequent users 
        of the script.

.. image:: images/Add_Comment.png
    :width: 300
    :height: 200
    :align: center
    :alt: Add Comment Block



*       Collapse Block*

        Click on Collapse Block to truncate the block.  This is useful when a large number of blocks are in the workspace 
        and the user wants to make a block smaller so that it is easier to see other blocks.  The user can restore the 
        collapsed block at any time

*       Disable Block*

        Click on Disable Block to make the block turn white and it will not be included in the script.  This is similar 
        to “commenting out” lines of scripts when writing MicroPython code.

*       Delete Block*

        Choose a block by clicking on it.  Right click on the block and then choose Delete Block to delete the block from 
        the script or press the Delete key on the keyboard.   Blocks can also be deleted by clicking on a block, separating 
        it from the graphical script and dragging it into the recycle bin.









































  





































