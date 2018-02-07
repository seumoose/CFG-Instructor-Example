# Session 1 - Getting Started and HTML
Within this branch I'll be briefly discussing the slides and going over the homework set at the end of session 1.

## The slides
##### _Basics of a website_
A website is constructed using HTML (HyperText Markup Language) which describes the structure of the page, CSS (Cascading Style Sheets) which describes the presentation of the page and optionally JS (JavaScript) which allows for user interactivity (making the website more dynamic).

Each page in the website is a seperate file and is defined in the URL as the final element e.g. 'http://www.examplewebsite.com/pages/ **first_page**

In brief: websites are a collection of pages (files) that linked together with various stylings applied to them to create a better user experience.

##### _Folder Structure is Important!_


##### _What is GitHub?_
GitHub is a widely used repository and version control service used by small start-ups all the way to large global conglomerates.
GitHub essentially allows users to upload their work, compare and collaborate with team members and, most importantly, allows changes to be rolled back for every version committed (imagine being able to undo specific changes made to a file where the changes are grouped together every time the file is saved).

## Installing Google Chrome
With any luck you will already be using Google Chrome. However another modern browser (Firefox, Safari etc.) will work perfectly – it’s entirely up to you on what you prefer to use.

If you do want to install it simply head over [here](https://www.google.com/chrome/browser/desktop/index.html "Google Chrome Download").

## Installing a Text Editor
Any text editor will work (Notepad, Notepad++, Atom etc.) however I would recommend the free version of Sublime text 3 in conjunction with the Emmet plugin.

Links to both items can be found [here](https://www.sublimetext.com/3 "Sublime Text Download") and [here](https://github.com/sergeche/emmet-sublime/archive/master.zip "Emmet Download") respectively.

Once you have successfully downloaded and installed Sublime Text 3 and the Emmet .zip file simply navigate to **Preferences -> Browse Packages** and extract the plugin (unpack the zip file) in the folder which opens.

Once complete, restart Sublime Text and auto-complete features should be enabled.
Auto complete works and operates in exactly the same way as it might on a mobile the only difference being you will be writing in html.
To select a highlighted option you can either click it with the mouse cursor (slow) or press `tab` or `enter` (fast).
To highlight different options simply use `up` or `down` `arrow keys`.

To finish off the installation of Sublime Text, navigate to **Preferences -> Key Bindings** and paste `{"keys": ["alt+shift+f"], "command": "reindent", "args": {"single_line": false}}` in to the right-hand window.
This allows for auto-indentation (I'll talk about this at greater lengths later on) which will make any html produced much more readable simply by pressung `Alt + Shift + f`.

_Optional_: You can also paste in the following codes in the key bindings section to make the tabs behave in the same way modern browsers work (i.e. move forwards and backwards by pressing `ctrl + tab` and `ctrl + shift + tab` respectively) - `{"keys": ["ctrl+tab"], "command": "next_view" },` and `{"keys": ["ctrl+shift+tab"], "command": "prev_view" }`.

_Note_: If you're following the CF:G guide and decie to use [Atom](https://atom.io/ "Atom"), an easy to install package for code indentation can be found [here](https://atom.io/packages/atom-beautify "Atom Beautify").

## Installing a GitHub Desktop Client
Later on in the course we will start using GitHub so it's a good idea to have everything prepaired in advance.
I would personally suggest (and will be using) [GitKraken](https://www.gitkraken.com/download "GitKraken Download"); however there are many alternatives including the oficial [GitHub Desktop Client](https://desktop.github.com/ "GitHub Desktop Download") and [Sourcetree](https://www.sourcetreeapp.com/ "Sourcetree Download").

All of the aforementioned options do exactly the same this but have slightly different user interfaces.
