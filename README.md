Repo links:
https://liz-guenthner.github.io/TrainTimes/

https://github.com/liz-guenthner/TrainTimes

Portfolio links:


Application:
1. Train Times App is tied to Firebase Database so all data persists even when user refreshes page
2. Anyone with Train Times DB credentials can save data to DB
3. Users can enter new train data into DB:
    a. Train name
    b. Train destination
    c. First train time (military time)
    d. Frequency in minutes
4. Click "submit" to save user data to DB an display at top of page
5. Next Train Time calulated and displayed at end of line
6. Times converted and calculated using Moment.js
    a. First train time converted to hours and minutes
    b. Current time converted into hours and minutes
    c. Difference calculated in minutes as difference between "first train time" and "current time"
    d. Minutes until next train calulated as difference in time (in minutes) "first train time" and "current time" plus the remainder of minutes (after finding "modulo")