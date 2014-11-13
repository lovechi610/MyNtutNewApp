FLASH PAGE FLIP DOCUMENTATION (Free Version)

www.FlashPageFlip.com

//////////////////////////////////////////////////

ADD PAGES
---------
Please refer to included XML file to see examples.


PAGE ONVISIBLE
--------------
Place functions called onVisible and onInvisible in your page SWFs.

function onVisible() {
	trace("Just turned to this page!");
}

function onInvisible() {
	trace("Just left this page!");
}


GO TO PAGE NUMBER
-----------------
To use the links on pages, please refer to the sample file (02.fla) in the "/Source" folder.
Place following code in your buttons actions.

on(rollOver, dragOver){
	_root.canflip=false; // flipping passive
}
on(rollOut, dragOut, releaseOutside){
	_root.canflip=true; // flipping active
}
on(release){
	_root.canflip=true; // flipping active
	_root.gotoPage(8,true); // go to page (8 is page number, true is directly go to page number, use false for flipping animation)
}


USE LINKS
---------
To use the links on pages, please refer to the sample file (11.fla) in the "/Source" folder.
Place following code in your buttons actions.

on(rollOver, dragOver){
	_root.canflip=false; // flipping passive
}
on(rollOut, dragOut, releaseOutside){
	_root.canflip=true; // flipping active
}
on(release){
	_root.canflip=true; // flipping active
	getURL("http://www.google.com", target="_blank"); // open link in new window
}


USE ANIMATIONS
--------------
To use the animations on pages, please refer to the sample file (09.fla) in the "/Source" folder.


USE VIDEO
---------
To include video, please refer to the sample file (07.fla) in the "/Source" folder. The video doesn't have to be embedded on the timeline as I've shown (dynamically loading an FLV or SWF would work fine too) but the key is that the video CAN'T start on the first frame.  This WILL cause problems.  I'd recommend using the onVisible and onInvisible functions mentioned above to control the video playback.


CHANGE THE COLORS
-----------------
To change the colors of flash page flip, please edit to Pages.xml file in the "xml" folder.
Please specify to following variables hexadecimal codes of your selected colors.

bgcolor="cccccc" loadercolor="ffffff" panelcolor="5d5d61" buttoncolor="5d5d61" textcolor="ffffff"


CHANGE THE LANGUAGE
-------------------
To change the language of flash page flip, please edit to Lang.txt file in the "txt" folder.


FAQ
---
http://www.flashpageflip.com/FAQ.asp?do=Show-All


SUPPORT
-------

PAY ATTENTION!

The same questions will not be replied which there are on the online FAQ system.

We appreciate your interest in us. Surely we reply to your inquiry however unfortunately we won't respond if there are same questions and answers on the FAQ page. Therefore please firstly look at the About FPF, Documentations and Product's pages. If you have any question please search in the FAQ system. If you cannot find any solution please summarize and send us a short email. The content of your e-mail is being considered and we will get back to you soonest.

support@flashpageflip.com