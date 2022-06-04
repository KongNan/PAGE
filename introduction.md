 PAGE - A Python GUI Generator

[![Download PAGE](https://sourceforge.net/sflogo.php?type=14&group_id=17014)](https://sourceforge.net/p/page/)

PAGE - Python Automatic GUI Generator - Version 7.4
===================================================

[![Download PAGE](https://a.fsdn.com/con/app/sf-download-button)](https://sourceforge.net/projects/page/files/latest/download)  
  
[![Download PAGE](https://img.shields.io/sourceforge/dw/page.svg)](https://sourceforge.net/projects/page/files/latest/download) [![Download PAGE](https://img.shields.io/sourceforge/dt/page.svg)](https://sourceforge.net/projects/page/files/latest/download)  
  
  [Sourceforge Summary Page](https://sourceforge.net/projects/page)  
  [Short Description](#Short_Description)  
  [Systems Supported](#Systems_Supported)  
  [Installation](#Installation)  
  [Documentation](#Documentation)  
  [Download](#Download)  
  [Small offerings for your consideration.](#Small_offering_for_your_consideration.)  
    [Vrex - Visual regexp written in Python](#Vrex_-_Visual_regexp_written_in_Python)  
    [Adages that have served me well](#Adages_that_have_served_me_well)  
  [Author](#Author)  

Short Description
-----------------

PAGE is a cross-platform drag-and-drop GUI generator, bearing a resemblance to Visual Basic. It allows one to easily create Python GUI windows containing a selection of Tk and ttk widgets. Required is a current version version of Python. PAGE is actually written in Tcl/Tk 8.6 which is embedded in tkinter. PAGE springs from Virtual Tcl, forked to generate Python modules that realize the desired GUI.

PAGE is not an end-all, be-all tool, but rather one that attempts to ease the burden on the Python programmer. It is aimed at the user who will put up with a less than completely general GUI capability in order to get an easily generated GUI. A helper and learning tool, it does not build an entire application but rather is aimed at building and organizing the GUI classes and the boiler plate code in Python necessary for getting the GUI on the screen.

Version 7.0 is a major release that allows the creation of GUI's with multiple Toplevel Widgets. Further, 7.0 drops support for Python 2. Change review:

*   The 4.2 release is a major release incorporating an approach to the rework problem.
*   The 4.3 extends the rework support to optionally upgrade an existing support module with Tk variables and skeleton functions newly required as a result of rework.
*   The 4.4 release supports popup or context menus. Also, support for ttk menubuttons has been removed pending more debugging. Finally, support for function definition and editing has been removed;
*   The 4.5 release supports the placement of the GUI at the default location as determined by the window manager.
*   The 4.6 release includes new function. a) Shows generated code in separate console windows. b) Allows loading of consol windows without geberating code. c) Allows the opening of users favorite IDE with saved versions of the generated code.
*   The 4.7 release includes support for binding events to top level windows and reorganizes the generated code for greater clarity and provides variable parameter lists for the init function in the support module using the Python convention of \*vargs, \*\*kwargs. Important fixes for Cut, Copy, and Paste and for the TCombobox widget.
*   The 4.8 release includes support for Custom widgets which are widgets for which the Python implementation is left to the user. Python 3 versions of the examples are included. The widgets handles have been enlarged and colored to facilitate selection. Numerous bugs have been fixed.
*   The 4.8.1 release fixes the bug which prevents PAGE from opening in Windows.
*   The 4.8.2 release fixes bug which prevents PAGE opening when a .pagerc file is missing.
*   The 4.8.3 release fixes bug which prevents opening existing project files.
*   The 4.8.4 release fixes bug which interferes with the saving of the support module in certain cases when PAGE should update the support module.
*   The 4.8.5 release fixes font bugs related to the About and the Error windows.
*   The 4.8.6 release fixes a Custom widget bug and has extensively revised documentation.
*   The 4.8.7 release fixes a Custom widget bug, includes modifications to font handling, context menus, Windows installation, and has updated documentation.
*   The 4.8.8 release fixes bugs occurring when .pagerc is missing.
*   The 4.8.9 release fixes a bug which is of interest to Windows users who install PAGE in custom locations where the path name includes blanks. Small changes to the documentation about event bindings. A new example has been added. A change has been made to the menu creation to avoid some confusing error messages.
*   The 4.9 release fixes bug related to state values of a few of widgets. It also improves the Widget Tree by changing the lables to display the class and the alias of the widget.
*   The 4.10 release includes a reuse facility which allows cut from existing projects and paste to the current project. This release also modifies the startup to automatically create the Toplevel widget and expands support for the Canvas widget and adds some checking of identifier syntax. In addition, there is a new custom version of the TNotebook widget which incorporates an icon for closing tabs.
*   The 4.11 release allows one to copy a menu bar from an existing project to the current project. An important addition is the inclusion of a tutorial written by Greg Walters.
*   The 4.12 release fixes several bugs related to placement, cut and paste, and borrowing.
*   The 4.13 release adds a search function to the Python Consols, fixes a syntax coloring problem, adds additional support for utf-8 encoding, and fixes some bugs.
*   The 4.14 release provides function to save the Widget Tree to a file and function to display callback functions. Fixes are also made for copy and paste as well as to relative placement.
*   The 4.15 release improves the use of the Binding Window, improves the display of callback functions, and the automatic saving of the project file. The ttk::separator widget is added and support of custom widgets expanded. Individual widget geometries can now be locked to prevent mouse changes.
*   The 4.16 release fixes an important bug in the support module update feature as well as improving the "Fill Container" function.
*   The 4.17 release displays the locked state of a widget in the Attribute Editor, adds a preference for setting the indentation, expands tabs when updating the support module, fixes a subtle bug with placement within labelframe widgets, and enhances the use of geometric attributes in the Attribute Editor.
*   The 4.18 release enhances the Scrolled widgets to support mousewheel scrolling, changes the style of tkinter imports, adds line numbering to the Python consoles, enables the context menu for Attribute Editor, and fixes bugs.
*   The 4.19 release provides Stash and Apply mechanism for transferring attributes from one widget to others, enables context menus in the Attribute Editor for transferring attributes from one widget to others - :ref:\`see the Attribute Editor \`, further enhances scrolling of PAGE windows, fixes bugs related to color preferences.
*   The 4.20 release fixes bugs related to the Scale widget and the Scrolledtreeview widget.
*   The 4.21 release includes Balloon Help (tooltips) for many of the supported widgets and bug fixes related to widget images.
*   The 4.22 release fixes several bugs.
*   The 4.23 release fixes several bugs, one related to the Scrolledtreeview, another to code generation in the absence of an IDE specification, and one related to changing relative size attributes in the Attribute Editor. The font support revealed errors and had to be fixed. Finally, the encoding problems and internationalization was addressed.
*   The 4.23a release fixes error that prevents code generation.
*   The 4.24 release includes further corrections for widget images, and font specification. It also facilitates the use of multiple initialization files.
*   The 4.25 release makes operation on 32 bit Windows system a whole lot better. It enables the opening of project files on drives different from the current drive, improves the "Stash and Apply" to facilitate widget alignment, changes the preferences function has to allow the saving of preferences to a named file, and fixes several bugs.
*   The 4.25.1 release fixes a bug affecting the Python generation for a number of ttk widgets when project have not been saved and reopened before generation of GUI module code.
*   The 4.26 release corrects several bugs related to widget handles, notebook, and menu generation. It also tentatively explores the ttkwidgets package.
*   The 5.0 release contains rewrite of the support module update code, provides limited functionality for multiple widget selection, adds the Scrolledwindow widget based on the canvas widget, adds New command to File menu in main menu, extends relative placement to the design phase of GUI development providing a WYSIWYG improvement, and fixes a number of bugs.
*   The 5.0.1 release repairs a mistake in the release of 5.0 documentation.
*   The 5.0.2 release corrects a mistake with busy cursors in PAGE windows.
*   The 5.0.3 release fixes bugs with relative placement and multiple selection.
*   The 5.1 release extends functions available in multiple selection, provides an experimental undo capability for certain operations, handles Windows device letters better, improves the resizing of panes in paned windows.
*   The 5.2 release fixes the saving of font specification for scrolled widgets, modifies the tooltip support, expands the multiple selection facility, and improves undo.
*   The 5.3 release fixes the use of arrow keys and extends their usage to changing sashes in paned windows, corrects some problems with paned windows, simplifies the specification of command attributes with arguments by generating lambda functions in some simple cases, and includes minor changes to the menu editor.
*   The 5.4 release changes the Menu Editor to more closely align with Tk menu capabilities, fixes a problem with font preferences, adds the Scrolledspinbox widget.
*   The 5.5 release fixes a problem with aliases in copy-and-paste operations, adds the capability to revert to default geometries for the principle PAGE windows, fixes problems with opening and saving projects, fixes a problem the Absolute/Relative code, makes minor improvement in the handling of fonts, reworks some of the examples for better presentation across OS's.
*   The 5.6 release fixes a problem with code generation for notebook widgets, fixes a problem with the presentation of the Attribute Editor in Windows, revises the command options.
*   The 6.0 release employs a Python wrapper which leads to a much simpler installation process, improves the error handling and display of PAGE errors, puts install directory in users PATH for Windows users, sets working directory of Windows icon to the users Desktop.
*   The 6.0.1 release fixes a bug with the separator widgets, and fixes problems with the Column Editor for Scrolledtreview widgets.
*   The 6.1 release introduces an autosave feature, accepts a nonexistance project file at invocation, and fixes several bugs.
*   The 6.2 release fixes several bugs.
*   The 7.0 release is a major release which
    *   Utilizes new formats for the generated GUI module and the support module which are simpler particulary for multiple toplevel GUI's. However, the new formats present some backward compatibility questions with existing support modules.
    *   Changes code for the skeletal callback functions.
    *   Drops Python 2 support.
    *   Updates examples to version 7.
    *   Updates and substantially enlarges the tutorials.
    *   Includes a discussion on migrating projects created in earlier versions of PAGE.
    *   Improves presentation of attribute errors.
    *   Allows user defined names for context menu function names.
    *   Corrects code for using images.
    *   Corrects code in notebook editor.
    *   Improves the handling of text and textvariable interactions.
    *   Adds support for the ttk::spinbox widget.
    *   Modifies the copy-paste to behave more naturally when borrowing toplevel windows.
    *   Corrects problems with copy-paste of toplevel menubars and context menus.
    *   Modifies the Widget Tree to behave more naturally when borrowing.
    *   Relegates backup files to the "backups" subdirectoy of project directory.
    *   Adds a preference to add custom sizes to the font selection dialog.
    *   Provides support for the labelanchor attribute with labelframe widgets.
    *   Support for inclusion of the post command for the ttk::combobox.
    *   Fixes miscellaneous bugs.
*   The 7.1 release:
    *   Improves behavior of Attribute Editor.
    *   Corrects bug that prevented creation of popup menus.
*   The 7.2 release:
    *   Corrects bugs related to the textvariable option with ttk widgets. Requires the user to disregard "::" artifact in Attribute Editor.
    *   Disallows the closing of the Widget Tree by the user.
    *   Now supports a variety of graphical formats including JPEG for most architectures and OS's.
    *   Uses tk widgets, in place of ttk widgets for dialogues.
    *   Corrects bugs in the update functions.
    *   Corrects bug with selecting TLabel widgets.
*   The 7.3 release consists mostly of bug fixes.
*   The 7.4 release:
    *   Cleans up color handling and can lead to a "Dark" mode for PAGE.
    *   Supports the location of rc files to be in any writable directory.
    *   Added some capability to modify global colors when reopening existing projects.
    *   Includes a new example which shows all of the supported widgets and shows some useful tips.

Systems Supported
-----------------

Currently PAGE and the resulting GUI windows have been tested on Linux running Python 3.9 running on Linux, and Windows 10, In the recent past it has been tested on OSX and Raspbian using Python 3.9. PAGE no longer supportd Python 2.

Widgets Supported
-----------------

*   Toplevel
*   Button
*   Canvas
*   Checkbutton
*   Entry
*   Frame
*   Label
*   Labelframe
*   Listbox
*   Message
*   Popupmenu
*   Radiobutton
*   Scale
*   Spinbox
*   Text

as well as the following ttk widgets:

*   TButton
*   TCheckbutton
*   TCombobox
*   TEntry
*   TFrame
*   TLabel
*   TLabelframe
*   TNotebook
*   TPanedwindow
*   TProgressbar
*   TRadiobutton
*   TScale
*   TSeparator
*   TSizegrip

and the scrolled widgets based on ttk widgets based on pyttk examples by Guilherme Polo:

*   Scrolledentry
*   Scrolledlistbox
*   Scrolledtext
*   Scrolledtreeview
*   Scrolledwindow

and finally

*   Custom widget
*   PNotebook
*   Balloon Help - Tooltip Support

Other features:

*   Menu Editor for creating menus.
*   Attribute Editor to easily modify widget attributes.
*   Editor for Event binding.
*   Editor for specifying Notebook pages and Panedwindow panes.
*   Balloon help (Tooltips) support.
*   Column Editor for specifying column attributes in treeview widgets.

Installation
------------

The required packages for executing PAGE are:

*   PAGE 7.0 or greater - This is the GUI generator. Actually one should be using the latest version.

All that is required for executing the python code generated by PAGE is a recent version of Python 3. The current version of the Python tkinter package includes the ttk widget set.  One does not have to install PAGE to execute programs containing GUI's generated by PAGE. All that is necessary is a Python version which includes the ttk widgets.

On Linux one downloads PAGE-xxx.tgz and expands it in a directory - usually the home directory. It is recommended that a bash alias be created with a command such as "alias page="python3 ~/page/page.py"; one can then invoke page with the command "page".

In Windows download and execute PAGE-xxx.exe creating the directory c:\\page and an onscreen icon for executing PAGE. The installation of PAGE adds the installation directory to the PATH enviromnent variable. One can invoke page with the command "page".

Documentation
-------------

[Users Documentation](html/index.html) which is also included in the package. There is now an [Epub](PAGE.epub) version of the documentation.

The tutorial subdiretory, "page/docs/tutorial" contains a tutorial, discriptive information, and sample code written by Greg Walters.

The documentation on this site may be more recent than that included with the package. When a package is released, it will definitely include the most recent documentation and I always try to provide up-to-date documentation for all features released. If you have suggestions for improving the documentation I definitely would like to hear about them.

Download
--------

To download Page, go to the [Source Download Page](https://sourceforge.net/projects/page) from which you can download the most recent version or

[![Download PAGE](https://a.fsdn.com/con/app/sf-download-button)](https://sourceforge.net/projects/page/files/latest/download) .  

### Tcl Debugging Functions

Similar to above I wrote a series of [Tcl debugging functions](debug.tcl) which make it easier to insert debugging statements into a tcl program.

Small offerings for your consideration.
---------------------------------------

#### Vrex - Visual regexp written in Python

This is example code based on Visual REGEXP. It is a tool for constructing and testing Python regular expressions. It has been updated to use ttk::panedwindow's and it [Vrex](vrex.html) provides most of the obvious facilities of that program, hence the lower case in the name. It is a tool that I use all the time. It will run under Python 2.7 and 3.2.

### Adages that have served me well

From a career of programming I have observed some things that have helped me quite a bit. See [adages](adages.html).

Author
------

PAGE's Author is Don Rozenberg. He encourage you to contact me with any problems, comments or suggestions. Keep those cards and letters coming; they are the only feedback he gets.

**Email**: <!-- emailE=('Don' + '.Rozen' + 'berg' + '@' + 'gma' + 'il' + '.com') document.write('<a href="mailto:' + emailE + '">' + emailE + '</a>' + '<br>') //-->
