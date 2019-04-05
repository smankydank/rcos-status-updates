## Last Week's Accomplishments
This week I mainly worked on the frontend for the post page. Continuing where I left off last week, I implemented functionality to the date text field and the time text field. A lot of the front end functionality involves ensuring proper format when the post button is pressed. 

(1) For the date field, I had the string getting read in and checking for the proper format 'mm/dd/yyyy', if this is not recognized, an error message is sent to the screen to correct the user format. Also for the date, I check to ensure that the date entered is either the current date, or a date in the future since we cannot have past rides being put up. To do this I split the inputted string, assuming valid format, into month, day, and year variables. Then, using a date object, i got the current month, date, year and only allowed for the logic to proceed if the entered month, date, year, was greater than or equal to the current month, date, year for all three fields. 

(2) For the time field a similar process was followed to the date field. This time I tried to ensure a valid format of hh:mm was entered. I then extracted the hour and minute fields from the input string and ensured that hours was <= 12 and > 0 and that minutes was < 60 and >=0. Then I checked the hour and minutes against the current hour and minutes and made it so the post had to be for at least 10 minutes in the future (subject to change).

(3) For the am/pm picker, I simply had to extract the current state of the switch and return a string either stating am or pm

If any of the data above failed or was invalid, an alert is sent to the screen and the field that failed was cleared. All variables (hour, minutes, month, day, year, am_pm, message) were stored in the post_action so that they could properly be sent off to the database whenever that is ready. 

## This Week's Plan
This week we will be doing RCOS branch presentations to go over everything that we have done during the semester. I plan on working on the powerpoint with my group and possibly doing some fine-tuning to the posting and/or hub page. 

## Anything Blocking?
Exams, just finished so nothing much. However, most of my focus will now be on IED.
## Notes
nothing to report
