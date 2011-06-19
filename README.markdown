## Overview

*		What:		HTML and CSS mockup
*		Who:		2011 Web Raising team (principle design work by JD Vorheis, coding by Nate Goldman and JD Vorheis)
*		Why:		Redesign and migration of the Portland PC Users Group website to concrete5 CMS

## Developer Notes

### Thurs 6/16/2011
VIOLENTLY STRONG SUGGESTION: for member content styling, if a member.css conditional stylesheet is not an option, just add a .member class to the container:

	<div id="container" class="member">

All public content can just be default without a specific identifier -- a .member prefix will override the default. So you could style a member element like so:

	.member #content { property: value; }

kthx
-nate

### Fri 6/17/2011
I completely agree with the .members being added to a new #container. I think we agreed it would be easier just to point to one css file. So I created a new #container with .member as a class. 

I updated the following:

*		Added target="_blank" to the links in the footer on both the home and members templates. 
*		Added new CSS for the member area.
*		Create an index.html page for members home page.

-jd

### Sat 6/18/2011
Updates:

*		Redid a tiny bit of the member CSS
*		Reworked some CSS defaults for optimization
*		Stubbed out the public homepage
*		Added some fake form functionality to link public & member indexes
*		Added some fake search functionality to send "search" clicks to a blank search page
*		Added placeholder jQuery plugin so HTML5 input placeholder text shows up on legacy browsers
*		Created a github repo so we can more easily track updates and changes

-nate

### Sun 6/19/2011
Updates:

*		Changed the logo back to white witha  rollover of orange
*		Removed PC-Grapevince from public
*		Removed the about PPCUG from public and moved the thanks column info over
*		Resized the footer to have a min-height of 190px to give a little more breathing room
*		Removed PC-Grapevine from the footer nav
*		Changed the left right padding of #footer td.divider to 8px
*		Added Sigs area in member section
*		Added contentBody for copy area in members section, NOTE: We should use this in the public area too. Not on the home page though. 
*		Updates the sigs image, there were a few that were off by 1px in the hover state in the image not the css. Css was good. 
*		The #contentBody is not expanding... min-height is set to 400px but it does not grow... what am I missing?
*		Updated the main bg.png - it had a little bit of a white border