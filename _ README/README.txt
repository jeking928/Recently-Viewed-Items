Recently Viewed Items v2.3
Original Mod Author:  Absolute Solutions

Released under the General Public License
This script is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
FITNESS FOR A PARTICULAR PURPOSE.

====================
  PURPOSE & AIM
====================

A simple but effective sidebox module that displays recently viewed items. Also included is an optional installation file to display recently viewed items in a centerbox. Ultimately, you can choose to display your recently viewed items in a sidebox (default), a centerbox (optional), or both (optional).

====================
  FILES LIST
====================

New Files Added
------------------
includes/extra_datafiles/recent_products.php
includes/languages/english/extra_definitions_YOUR_TEMPLATE/recent_products.php
includes/modules/sideboxes/YOUR_TEMPLATE/recent_products.php
includes/templates/YOUR_TEMPLATE/sideboxes/tpl_recent_products.php
includes/templates/YOUR_TEMPLATE/templates/tpl_modules_recent_products.php


Template Files Modified
---------------------
/includes/templates/YOUR_TEMPLATE/tpl_product_info_display.php

====================
  INSTALLATION
====================

**ALWAYS - BACK UP YOUR FILES & DATABASE BEFORE INSTALLING AN ADDON**
 
1. Extract the contents of the zip file to a temp directory on your PC, leaving the folder and file structure intact

2. Rename all instances of YOUR_TEMPLATE to match the name of your template override folder

	- Required Installation Files/includes/languages/english/extra_definitions_YOUR_TEMPLATE
	- Required Installation Files/includes/modules/sideboxes/YOUR_TEMPLATE
	- Required Installation Files/includes/templates/YOUR_TEMPLATE
	- Optional Installation File/includes/templates/YOUR_TEMPLATE

3. If you or another addon have made any changes to the file below, you will need to use a file merging software like WinMerge or BeyondCompare to merge the file changes together.

	- Optional Installation File/includes/templates/YOUR_TEMPLATE/tpl_product_info_display.php
	
	- This file was changed in Zen Cart 1.5.3. If you're using Zen Cart 1.5.3+, use the file in:
	2_Optional_File\zen153\includes\templates\YOUR-TEMPLATE\templates

	- The changes to this file is easy to locate because it is clearly commented as follows:

  	 	<!--bof recent products module-->
   
   	 	<!--eof recent products module-->


4. Once your file merges (if any) are complete, use your favorite FTP program to upload the CONTENTS of the Required_Installation_Files folder (not the folder itself)

5. If you want to add the option of having recently viewed items displayed in a centerbox, instead of or in addition to having them displayed in the sidebox, then upload the CONTENTS of the Optional_Installation_Files folder (not the folder itself)

6. Install the SQL file, located in SQL/install.sql
	- Using Notepad or some other text editor, open the install.sql file & copy the contents
	- Log in to your store's admin
	- Navigate to Admin > Tools > Install SQL Patches
	- Paste the contents of the file into the box & click "Send"

=====================
USEAGE & CONFIGURATION
=====================

To set the maximum number of items that can be shown in the sidebox, navigate to Admin > Configuration > Maximum Values > Maximum Display of Recently Viewed Products. The default value is 3, but you can change it to whatever you like. 

Then navigate to Admin > Tools > Layout Boxes Controller, select the recently_viewed box, and turn the sidebox option to YES & select the sort order of your choice.

To set the maximum number of items that can be shown in the centerbox, navigate to Admin > Configuration > Maximum Values > Maximum Display of Recently Viewed Products on Product Page. The default value is 3, but you can change it to whatever you like. 

To set the maximum number of items that can be shown per row in the centerbox, navigate to Admin > Configuration > Maximum Values > Maxium Display of Recently Viewed Products per row. The default value is 3, but you can change it to whatever you like.



===============================
 ACKNOWLEDGEMENTS & CREDITS
===============================
Credit for original contribution goes to Absolute Solutions
All thanks go to nigelt74 for contributing the technical aspects of the update & resolving multiple issues in V2.
Special thanks to gjh42 & DivaVocals for helping me learn more about Zen Cart coding

===============================
CHANGE LOG, ACKNOWLEDGEMENTS & CREDITS
===============================
v2.3 updated by jeking
- updated for Zen Cart 1.5.3 and 1.5.4
- rewrite of ReadMe

v2.2 by harolds
- fixed the queries so that they include the selected language (otherwise you would see the product in every
activated language)
- added the maximum number of items on product page
- added CSS classes to the images (so you can easily style them as you see fit)
- made the SQL a bit easier to import (no configuration_id anymore, it will be autofilled)

v2.0 for Zen Cart v1.5.0
Updated by nigelt74 & ScriptJunkie 
Updated for Zen Cart v1.5.0
Added tpl_product_info_display.php because it was missing from previous version.
Fixed Centerbox issue (centerbox would not display) by adding includes/extra_datafile/recent_products.php & fixing dozens of syntax errors in modules/recent_products.php
Cleaned up the folder/file structure in the download package to bring it up to date with current standards. 
Clarified the installation instructions. 
Cleaned up the readme file and brought it up to date.


v1.1 for Zen Cart v1.3.8
MotoCC added centerbox functionality


v1.0 for Zen Cart v1.3.8
Updated by Mukesh Waghmare


v1.0 for Zen Cart v1.3.5 
Original contribution by Absolute Solutions