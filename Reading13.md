# Class 13

## Local Storage and its use on Websites

Cookies:  A cookie is a text file hosted on the user’s computer and connected to the domain that your website runs on. 

Cookies have a few limitations though:
They add to the load of every document accessed on the domain.
They allow up to only 4 KB of data storage.
Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

They add to the load of every document accessed on the domain.
They allow up to only 4 KB of data storage.
Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

## Past, Present, and Future of Local Storage for Web Applications

Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
What we really want is

a lot of storage space
on the client
that persists beyond a page refresh
and isn’t transmitted to the server


HTML5 STORAGE SUPPORT
IE	FIREFOX	SAFARI	CHROME	OPERA	IPHONE	ANDROID
8.0+	3.5+	4.0+	4.0+	10.5+	2.0+	2.0+
From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.


STORAGEEVENT OBJECT
PROPERTY	TYPE	DESCRIPTION
key	string	the named key that was added, removed, or modified
oldValue	any	the previous value (now overwritten), or null if a new item was added
newValue	any	the new value, or null if an item was removed
url*	string	the page which called a method that triggered this change
* Note: the url property was originally called uri. Some browsers shipped with that property before the specification changed. For maximum compatibility, you should check whether the url property exists, and if not, check for the uri property instead.
The storage event is not cancelable. From within the handle_storage callback function, there is no way to stop the change from occurring. It’s simply a way for the browser to tell you, “hey, this just happened. There’s nothing you can do about it now; I just wanted to let you know.”