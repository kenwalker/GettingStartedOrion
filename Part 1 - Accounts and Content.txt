Enable word wrap in Orion - Option-Cmd-W

Welcome to the Orion getting started Videos, this is the first in a series that will outline how to get started with Orion and lead you through the capabilities of our Online Web Development platform.

Let's start with the real basics which is how to create an account at OrionHub.org and how to get content into the IDE.

First, navigate to OrionHub.org and select the "Create a new account" button.  There you'll need a username that's not already taken, a password and an email address.  We take that email address to allow you to reset your password and to also assist in associating your account with the Mozilla login service.  Once you've submitted the information, you'll need to confirm your email address by clicking the link you receive.  You can now login to your OrionHub account.

When you login, you'll end up in the Navigator.  A pretty baren place at the moment because you have no folders or content. Let's ignore that for a moment and look around at what's available to you in the UI.  On the top left you have what's called in the industry, the "Hamburger".  I'll describe that a bit later.  On the top Right, you have the "Options" menu, it looks like the top of a person. If you choose that, there's our online help, the keyboard shortcuts available for the page you're on, user settings, and where to sign out.  We'll cover User Settings in Episode 2 and keyboard shortcuts a little later on.

The bottom of the Orion window shows the build you're running, and a couple of links related to the terms and copyrights of the code that represents Orion.  Another important link is the "Bugs" link.  Anyone can report a bug against Orion, it just requires an Eclipse Bugzilla ID that you have to create.  Orion is an Open source project so the bug logging and tracking is all in the open just like the code.  A great way to participate is to log a bug... then fix it and submit a patch request to the team. This is how we all got our commit rights, including myself.

Ok, back to content. The team is working on a more convenient method of getting some basic examples into Orion but for now lets just do it manually. 

On the left of the Navigator, click the "New" button and choose "Folder", then enter a name like "Testing".  Just for your information, you can't create files in the root of the workspace.  Before you navigate into the Testing folders, lets look at how navigation vs. selection works in Orion because it's a bit different that a standard IDE because we're following a web model here.  The standard pop-up menu (right click) is NOT how we choose actions, Orion does not override the default browser behaviour for content menus. Instead, if you click slightly to the right of the word Testing, you'll notice that the row (or the Tested folder) is selected.  If you pop up the Actions menu, you can now see the actions that can be performed on this folder such as copy, and move, import contents, etc.

Now, if you click on the word Testing, we navigate into the folder.  Again it's a bit empty because there's no files in there yet. However, in the middle of the window at the top you can see the breadcrumb of navigation starting to build. If you want to navigate up in that chain you can just select a previous folder from that list to go "up".

Let's navigate back into the Testing folder and create a file. Choose the New File option and type in testing.html then enter. You can see that a file is created, you can see the time and size of the file in the Navigator.  Again, select this file and choose the actions for it.  You can again see copy, move and additional actions. If a plugin for Orion was added that provided additional functionality on HTML files, it might present options in this menu.  This is one of the menu places the Orion UI can be extended by 3rd parties including yourself.

Let's create another file, called "testing.js". Once it's created let's open it in the editor by clicking on the filename.

You're now in the the Orion editor.  We're not covering the editor in this video but we want show how the Navigator in the Editor is similar to the Navigator page.  First, you can switch between editing each file by clicking on the file names.  You can see the breadcrumb at the top change as you do that.

If you select a file, vs clicking on it, then you can get to the actions by selecting the "Gear" icon.  Again you can see the same actions you had in the Navigator like copy, rename, etc.

You can also use the "plus" icon to create folders and files while in the Editor page.

If you pick the "Go Up" bent arrow, what you're doing is changing the Editor navigator context around but not changing the file you're editing.  That still shows in the breadcrumb at the top.  You can use the little triangle to open and close folders without navigating into them and pick and choose files to edit.

Ok, lets talk about something that's important with respect to Orion navigation and that's the concept of "Related Pages".  Since Orion is not trying to represent an entire IDE within one page, the user needs a convenient way of finding related tasks based on the context of the current resource they're working on.

For example, lets select "testing.html" and then choose what's known in the industry as the "hamburger". What's displayed are two things.  The "Main Pages" are like landing pages, they'll come with no context and just put you in the root of that page.  The "Related Links" are context sensitive with respect to either the folder you're in or the file you're editing.  So for example, if you choose "Navigator", you're taken to the Navigator page and placed in the "Testing" folder.  Use your browsers "back" button to take you back to where we were in the editor.  Now choose the "Hamburger" Main Pages "Navigator".  Now you're placed at the root of the file system with no specific context.  Again press your browsers "Back" button or use the shortcut key for it.

We've show a couple of things here.  That depending on what you're editing, or what context you're in on an Orion page, the "Related Links" menu will dynamically change to represent tasks or workflows you might be interested in. So if the file you were editing was part of a Git project, one of these items would be a link to the Git log for that file.  The other is that we always have the main pages available for quick reference to get to the root of those pages, like ALL your git repositories vs just the one for the file you're editing.  Another concept we showed is that Orion behaves like any other web page.  You can use the forward and back browser features and bookmark capabilities on any of our pages.  We behave just like you would expect a browser app to.

Let's show how to get some code in and out of Orion from your Desktop. To do this, use the Hamburger menu to get to the Navigator.  You want to select the Testing folder then choose the action "Export as ZIP".  That should have downloaded a ZIP file to your downloads folder.  I'm assuming you know where that is.  Still in the Navigator, make sure you deselect the Testing Folder and then choose the action to create a new folder called "Testing2". Select that folder, and choose the Action "Import from local file". We're going to want to leave the checkbox to unzip the contents checked because that's what we want to do.  Either use the "Choose File" dialog or drag and drop the zip we already downloaded onto that dialog.  You should be able to navigate into "Testing2" and see the two files we just imported.

If you have an existing JavaScript or other project somewhere, this is an easy way to get the content into Orion.

Now that we at least have a few files in your Workspace lets look at a handy shortcut.  To see what keyboard shortcuts are available to you, press SHIFT-?.  If you're in the editor, that becomes SHIFT-CTRL-?.

You can see that there's a Find File, for me on the Mac, that shortcut is Command-Shift-F.  I can just start typing and files matching will be displayed.  Start typing "test"  or "*.js" and the matches will be displayed.  To save time, don't bother reaching for the mouse or trackpad, just use the cursor to navigate and then press enter. You'll open in the editor in the right file.  Even there you can then again choose Command-Shift-E to navigate to another file.

Alright, that's the first step in Using Orion covered, creating an account, getting content in and out, main and related pages, navigation and a few keyboard shortcuts.

Have a go at Episode 2 for User settings and the basics around using the Editor.
