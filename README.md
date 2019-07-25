Repo links:
https://liz-guenthner.github.io/TrainTimes/
https://github.com/liz-guenthner/TrainTimes

Resume links:
https://liz-guenthner.github.io/lizGuenthnerResume/
https://github.com/liz-guenthner/lizGuenthnerResume


Application:
1. Users can enter new train data into DB:
    a. Train name
    b. Train destination
    c. First train time (military time)
    d. Frequency in minutes
2. Click "submit" to save user data to DB an display at top of page
3. Next Train Time calulated and displayed at end of line


Problem:
1. How to create a FireBase DB.
2. How to persist data on web page.
3. How to display dynamic content of new train info.
4. How to calculate time of new train.


Solution/Technical Approach:
1. Creat FireBase DB and share creds so that users can input/output data for persistence.
2. Create form to capture user info and store data via FireBase Config creds and code in js file.
3. Submit button uses jQuery to push input to DB and display new data with dynamic row insertion in table.
4. Moment.js calculates time as follows:
    a. First train time converted to hours and minutes
    b. Current time converted into hours and minutes
    c. Difference calculated in minutes as difference between "first train time" and "current time"
    d. Minutes until next train calulated as difference in time (in minutes) "first train time" and "current time" plus the remainder of minutes (after finding "modulo")