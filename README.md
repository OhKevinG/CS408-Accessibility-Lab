*******************
* Kevin Gutierrez
* Accessibility Lab
* CS408 Web Development
* 02/13/2025
*******************

REPORT
 
 COLOR:

  Contrast was checked with WebAim Contrast Checker using the green(0, 128, 0) background and black text. Test failed and Contrast Ratio was 4.08:1. Changed to lightsteelblue(176, 196, 222).

 SEMANTIC HTML:

  1.) When navigating with the keyboard only the web page will tab through the nav links, but skips over all the main content and some information cannot be read. The tab key will stop at the audio player, but it has no description when hovering over it with a screen reader so there is no way to tell what it is for. None of the page links or the links in the list cannot be selected with the enter/return key.

  2.) The article has several accessibility issues that makes it hard to use with a screen reader. For one there are no header tags or paragraph tags, and therefore these sections have no natural flow and a screen reader will just read it all in one big chunk instead of announcing where a new header is leading to a new section. Added heading tags and paragraph tags and now it is much easier to navigate and tell where you are at on the page when using a screen reader.

  3.) The navigation menu could be made more accessible by using the HTML nav tag which has built in accessibility features. The change was made.

 IMAGES:

  Images do not contain alt text and was completely skipped over by the screen reader. Alt text was added and now an audio description of each is output by a screen reader.

 THE AUDIO PLAYER:

  1.) The audio player has no transcript which would make it accessible to hearing and impaired people. A button was added that when pressed will reveal the transcript.

  2.) A download link was added to the audio element in case someone's browser does not support html audio.

 THE FORMS:
  
  1.) To add a label without adding text that will be seen we can use the WAI-ARIA property aria-label which will read a label from a screen reader, but will not affect the page visually at all.

  2.) The two input elements in the comments were given a <label> html tag that attaches them to the input elements.

 THE SHOW/HIDE COMMENT CONTROL:

  To make the comment control button accessible via the tab key I added the property tabindex="0" and then added some basic JavaScript to main.js to ensure that all interactive elements on the webpage can be selected with the Enter/Return key.

 THE TABLE:

  I added a caption to the table that gives a brief description of the information in the table. I also changed the <td> elements in the <thead> block into <th> elements to give them a clear emphasis. Same with the two Bear types for emphasis on the columns. I then added the scope property to each <th> element to make it a lot easier to navigate the table using a screen reader.

