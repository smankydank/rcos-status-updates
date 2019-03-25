## Last Week's Accomplishments
- UITextView/Posting: This week I mainly focused on creatinga  barebones for posting to the hub page in the app. I added a UITextView and did research on functions that would allow me to create a text box similar to that of twitter which limits the number of characters. Initially there is a placeholder text which I had to figure out how to add in programatically since there is no built in feature. In addition, a label exists in the bottom right hand corner which counts the number of characters in the text view and displays that number of of 500. The user cannot type more than 500 characters for a post as of now. I also disabled scrolling in this view. Finally I added a feature where pressing the return key would close the keyboard. This is important because before adding this feature, it was impossible to have the textview resignfirst responder. Essentially I had the field detect a '\n' character and end editting accordingly. This also helps to limit the number of lines and characters so as to not be able to be able to go bellow the view. 

- Date Picker: The last thing I did was add a date picker with very basic function


## This Week's Plan
This week I plan to finish up the post page so that the date picker, text field, and button all work together. If possible I would like to send this data off to the database but that depends on whether it is up and working properly. If this is the case, I may also try to download the data to the hub and actually add it into the scrolling cells.

## Anything Blocking?
This week  I have an exam and a competition I am participating in. In addition the database may or may not be setup.

## Notes
nothing to report
