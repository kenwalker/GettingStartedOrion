Enable word wrap in Orion - Option-Cmd-W

Welcome to the Orion getting started Videos, this is the second in a series that will outline how to get started with Orion and lead you through the capabilities of our Online Web Development platform.

This video will show you how to change the user settings and cover the basics if using the Editor.

I'm assuming you already have an account at OrionHub and have covered Part 1.  After logging in, lets go right to the User Settings, available in the Options menu in the top right of any Orion page.

When you end up in the Settings Page, the categories of settings are displayed along the left hand side. This list may shrink or expand depending on what types of plugins you are running and whether or not those plugins expose additional configuration within the Settings page.

Let's look at the top item, which is the User Profile.  Here you can change your Full Name, your email address (requires re-confirmation) and your password.  In addition to logging into Orion with our credentials, you can also login with your Google ID, to associate your account with a Google ID, expand the "Linked Accounts" twisty and press the "google" icon.  After this is associated, you can login to Orion by choosing the Google button on our login page. To associate your Mozilla Persona, all that's required is that your email address matches your Persona email address. So there's no specific linking required, it just works.

On to Git settings.  On the Git server you typically use (Github for example), you'll have an ID and an email address.  Before you clone anything from your github account it's important to set this up and save it.  That way, when you commit changes, the fields will already be filled in.  Otherwise, you'll be prompted each time for the info.  The second option is to allow Orion to save your Git credentials in browser storage.  This does NOT store any credentials on the Orion server or on disk.  You have to enable this for every browser you use and if you clear local storage, this setting is wiped out.  If you use the same browser at work all the time with Orion, this setting will appear to be pretty consistent.  After allowing this, the next time you push a change from one of our git pages, you'll see a check box confirming that you want Orion to remember it.  More on that in a later video.

While we don't have a tonne of themes, you can change up the UI a bit to your liking.  There's a few canned options but we really haven't spent a lot of time tweaking them at the moment.

Editor themes are also available and you can choose one of our built in ones, tailor it yourself, or import one from the EclipseTheming site.  Orion doesn't have all the same theme settings so after importing one it might not look exactly the same.  Orion will improve our theming over time.

Editor Settings are growing over time as well.  One new setting is the option to enable auto-save.  After a pause in the editor your changes are persisted to the server. Additionally, if you enable auto-load then when you change focus to an Orion editor where the file has been changed out of scope it will load the changed file so that you do not end up out of sync. We're also working on key-bindings so the list here will likely change over time.  Currently in my example you see Emacs, but VI is also coming soon.

Plugins, show the list of installed and active plugins for Orion.  Plugins will be covered in more detail in a follow on video.

General currently has one setting which is to enable opening any "link" within Orion in the same tab or a new tab.  If you choose "new tab" you might end up with a lot of tabs open, however that's how a lot of people like to work.

Validation is related to our Java Script Lint plugin, not worth covering at this point.

Let's use the "hamburger" to get to the Navigator, and navigate into our "Testing" folder and choose "testing.html" so we end up in the editor.

In the first video we showed how to get the list of keyboard shortcuts using Shift-?, but in the editor we need a different key combination, and that's Shift-Ctrl-?.  If you can't remember it, the list is always available in the options menu in the top right.

Ok, that's a pretty big list and they'll not all be covered in this video but we'll cover a few of the typical ones.  First, there's content assist.  Now this feature is dependant on the support by plugins for particular file times.  By default Orion has some amount of content assist for HTML, CSS and JavaScript.  Since we're in an empty HTML file, choosing content assist (Cntl-Space) gives the option to create a Simple HTML document. You can see the cursor is placed at a spot to start entering the title and pressing Tab takes you to the next part of the content assist entry for a header.

We've made some changes to this file and the asterist next to the filename indicates the content is 'dirty'.  Press the "save" button.  A better way for some to work is to have auto-save on, and you can either go to your settings page or get to this setting using the "spanner" icon over on the right.  If you enable auto-save, the "save" button will disappear.  Now, ever time you pause in the editor, your changes will be saved and any plugins that parse the result of your file will update your markers. To see what I mean, delete the last > from the end of the file and wait for autosave.  You'll see that we have markers along side the editor for errors, warnings and information.  Plugins contribute to these markers but we have some defaults for HTML and JavaScript.

Ok, click on the "testing.js" file and we'll put in a little JavaScript code.  All the JavaScript code is parsed by JSLint and the errors or warnings that it generates will appear in the gutter. So if you typed in "console.log("hello");", after auto-save you'd have an error that console is not defined.

For JavaScript files we support the option to put a /*global console */ section at the top.  You'll see that the error goes away.  The JSLint and the other Orion tools don't have context outside of the file you're editing however we hope to improve our JavaScript toolign to include scope in the project you're working on.

I'm going to enter a bit of code and show some content assist.

function Point(x, y) {
	this.x = x;
	this.y = y;
}
var aPoint = new Point(1,2);
aPoint.x

It knows that there are the variables, but not the types, so adding a bit of JSDoc can help out here.

/**
 * @param {Number} x coordinate
 * @param {Number} y coordinate
 */
function Point(x, y) {
	this.x = x;
	this.y = y;
}
var aPoint = new Point(1,2);
var anX = aPoint.x;
anX.toExponential(1);

Again, this is only scope to the file you're editing, but the Orion team is working on improving our JavaScript tooling specifically content assist.

Let's look at some of the other standard features of any editor.  You can find and replace with Ctrl-F (or Cmd-F on Mac). There are even lots of options for searching and replacing including Regex expressions.

Ctrl-L is goto line.

If you select a line, you can use commands like Alt-Up and Down to move the lines up or down.

You can add your own TODO annotaions and navigate around annotations with Cmd+. or Cmd+,

/*global console */
console.log("hi");

/**
 * @param {Number} x coordinate
 * @param {Number} y coordinate
 */
function Point(x, y) {
	this.x = x;
	this.y = y;
}
//TODO rename this thing
var aPoint = new Point(1,2);
var anX = aPoint.x;
anX.toExponential(1);

//TODO Need more code

var i

var k

You can also either comment/uncomment or indent/unindent whole selections

There's also word wrap if you have really long lines and want to see the whole content.
