# modal
 modal windows
triggerSelector is a button that opens a modal window when clicked
modalSelector - modal window
modalTimerId is a timer that opens a modal window after a fixed period of time

I am creating a modal function.
1) I go to HTML and select the buttons that will be responsible for calling the modal window, assign them data-attributes (open)
and do the same with the classes that will close the modal windows (close).
2) Now I use these data-attributes in the script.
3) I create two functions:
The first function will be responsible for opening modal windows when the button is clicked
The second function will be responsible for closing the modal windows.
4) I make it so that when the modal window is opened, the page is fixed and does not scroll
5) I go through all the buttons responsible for calling the modal window
6) I make the modal window close when clicking outside of it or when the esc key is clicked, 
and I make the modal window respond to the esc key only when it is open
7) I make it so that when the user scrolls the site to the end, a modal window appears
8) I create setTimeout - in order for the modal window to open after a certain period of time, 
if the user has already opened the modal window, then cancel modalInterval.

*In order to track how the user scrolls the page, we use an event called scroll.
*scroll hangs on the global window object
*pageYOffset - tracks how many px from above the user has scrolled along the Y axis
*scrollHeight - we get the full height of a certain element, taking into account scrolling from above and the visible part
9) The functions responsible for opening (openModal) and closing (closeModal) modal windows are outside the modal function
