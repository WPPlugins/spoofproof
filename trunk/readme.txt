=== SpoofProof===
Contributors: Jerry Hayward
Tags: SpoofProof, Security, injection, anti-injection, anti-javascript-Injection, anti-PHP-injection
Requires at least: 4.3
Tested up to: 4.6
Stable tag: 4.6
License: GPLv2 or later

SpoofProof alters the login screen using a web service detecting if you are being attacked by spoofing, phishing, Brute Force or Man in the middle.

== Description ==

SpoofProof alters the WP login screen using a web service to verify that you are not being attacked by  spoofing, phishing, Brute Force or Man in the middle.  We also strip javascript and sql tags from posts that would otherwise infect your site with bad code, or just lose you infromation.

We are a **light weight** plugin.  It is a practical impossiblity to attack only one (or all but one) page of a web site; By detecting only on the login page, we let the rest of your site run without interferance, having validated at the point of entry you know you are safe.  the Injection stopper runs entirely on your site and cleans all posts that go through the API as they are supposed to.

== Frequently Asked Questions ==

Q. *How can I know it is working?*

A. Attack your web site :-) 
	1. We have a check box to mess up your login attempt and have it look like an attack.
	2. If you log in and fail enough times, it will look enough like a brute force attack that we will block you (for a few minutes).
	3. copy some javascript from somewhere and post it as a comment like a user would (if the admin has to approve coments no one will see it.) You can see that we strip the javascript tags.

Q. *What is spoofing?*

A. Spoofing is when soimeone tries to make a site that lloks like yours, but it's just there to collect information, like usernames and paswords.

Q. *What is Phishing?*

A. When someone tries to send people to a site that is not yours, by climin they need to reset a password or something.

Q. *What is Man In the Middle?*

A. a Man In the Middle (MITM) attack is when someone gets betewwn you and the server you want to talk to and pretends to be the server to you, and you to the server.  if done well, it is impossible to detect from inside the communication channel.  That is why we use a web service to examine your login connection for MItM signitures.

Q. *What is a Brute Force attack?*

A. A Brute Force atack is when someone just starts running combinations of letters and numbers at your username an password fields until they get in.  It can be stopped by timing out an attempt from a machine and making them wait, that makes the attack take too long, and since we are logging the effort, they have been identified.

Q. *Can anyone else do this?*

A. No, CipherTooth's methodology recently was reccomended for release by the patent examiners office which meens in a short time we will have a full utility patent, not just be patent pending.

Q. *Does your plugin stop me from using a capcha, paswword visibility plugin, or theming my logins?*

A. no as long as you follow the WordPress standard and the API to d oyour customizations, it should be compatible... but no guarentees, not everyone who publishes a plugin follows the API.

== Installation ==

**Automated:**
1. Go to the Plugins -> Search for "SpoofProof".
2. Click install SpoofProof.
3. Activate SpoofProof.

**Manual:**
1. Go to the Plugins -> Add New -> Upload.
2. navigate to where your "SpoofProof.zip" is and upload it.
3. Click activate.

1, 2, 3: You're done, and your site is protected.

you should probably go to your user and set your settings now so that you are not using the default image and phrase :-)

== Change log ==

= 1.0.0.4 =
*Released 09/05/2016
1. Fixed compatibility issues with changes to login screen.
2. Fixed compatibility with paths for changes made by 4.6.
3. Hid the "Remember me" check box by default because it is a security hole.
4. Fixed capitalization issues that were causing images on some installations not to display.

= 1.0.0.3 =
*Released 01/09/2016
1. Fixed compatibility issues with changes to login screen.
2. Fixed compatibility with paths for changes made by 4.1.
3. Fixed API changes that were causing images on some installations not to display.

= 1.0.0.2 =
*Released 11/15/2015
1. Bug fixes for some installs not creating all required directories.

= 1.0.0.1 =
*Released 11/13/2015
1. Fixed bugs with Brute Force detection.
2. Fixed bugs in MITM detection service that misreported some attacks.
3. Fixed interface bugs which stripped colors from text that were for emphasis.
4. Altered the way internal paths were red from Word Press to support installations in non standard directories.


= 1.0.0.1 =
*Released 11/5/2015
1. Added features to the Account screen.
2. Fixed bugs in the reporting of some events to the database.
3. Adding a version number to the zip file caused some issues with the correct location of image files. Ver 1.0.0.1 has no version number in the zip files.

= 1.0.0.0 =
*Release 10/10/2015

== Upgrade Notice ==
= 1.0.0.1 =
Fixed several bugs with images, made compatible with 4.6
= 1.0.0.0 =
Just released!