## Last Week's Accomplishments
- Scroll and load: When the user scrolls to the bottom of the app, new cells are inserted. The number of cells in the table is dependant on the number of usernames/messages in arrays added to the hubviewcontroller. This works by detecting that the last cell in the table has been scrolled on. If this is the case, the current index in the table is found and 10 new cells are created with unique user data (still needs implementation ie. grab data from database). Then the new cells are added to the bottom of the table and the table scrolls us to the previously last cell. The table will also display a spinning wheel at the bottom when cells are being created and added. This is useful so the user does not need to load hundreds or thousands of posts from online at any one time. It will only be useful for the user to see the most recent posts.


## This Week's Plan
1) solve the issue with scrolling to the bottom of the table described in "Anything Blocking"
2) implement the barebones of a searching feature to skim through all the posts in the database (if database is ready)
3) prepare skeleton for posting feature to the main page


## Anything Blocking?
On major issue i am running into with the scrolling and loading view is that using the function involving "willdisplaycell" which is supposed to work with tableview.beginupdates, does not product the desired result Beginupdates is meant to allow realtime animation for inserting and deleting cells at specific points in the table. This would avoids having to reload the table every time the bottom of the tableview is reached. As one can imagine, the more posts are scrolled on the less desirable reloading everything would be. Currently the interaction makes it so the cells are inserted, but do not show. This problem will need to be solved in the coming week. 


## Notes
nothing to report
