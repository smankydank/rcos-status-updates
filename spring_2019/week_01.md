## Last Week's Accomplishments

In the previous weeks I was able to successfully implement segues from the login screen to the hub and other viewcontrollers in the app. In addition, I added the settings slider menu. 

1) Segues/Login: segues were created by learning about reuse identifiers and presentview functions in swift. In case of failed segues, such as on login, a popup error alert was prompted to the user. For example, if the username and password were incorrect, 'Invalid Username/Password' is prompted to the user. I had to learn how to make this popup occur

2) Settings Menu: The settings menu is something added to the hub. When the user slides from the left side of the screen, the menu comes out and displays a list of options to the user in a UITableView Subview. This task proved to be much more difficult that expected. To Began by having the user press a simple button and an animation moves the menu into either the open or close position depending on the current state of the menu. From there I began to implement dynamic menu positioning. Basically, the user could swip fom the left side of the screen and bring the menu out to a maximum distance of its width. As the menu is pulled out, a coverview UIView that I added changes its alpha value to give the effect of the background dimming. This is gradual and is done using a linear function 'Cover_View.alpha = (0.6 / Settings_Table.bounds.width) * (Settings_Table.center.x + Settings_Table.bounds.width / 2)'. A UIPanGestureRecognizer was used to detect if the view was being touched. This view could also detect large velocity pans. If the view was panned really quickly, it would automatically go to the open or closed position depending on the current state. If the view detects low velocity, the view follows the finger and will only go to the other position is passing a certain cutoff which i set to the width of the view - 50. Lastly, the user can tap the coverview to close the settings view.

3) pull to refresh: Implemented a gesture recognizer that could detect a user refresh request on the main hub page.

## This Week's Plan

In this week, I plan to turn the tableview cells in the settings controller into segues to the respective view controllers. In addition, I want to further develop the hub page. 

## Anything Blocking?

The main blocker for progress is my group members. As I have previous experience with IOS I am a little bit bottlenecked and am taking on the more research intensive and complex tasks. I have a lot of work in my other classes which could interfere with my ability to research the next steps.

## Notes
