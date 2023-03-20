# Setting up the Progress Bar for the GSA Survey

Most of the functionality is already there for implementing the survey progress bar, we just need to setup a Google Doc website that shows the current number of responses to the survey and then adjust the current number of students in the program in the `survey_progress.html` document.

1) In the new survey google form that you are going to send out, go to the responses tab and create a google sheet for the form responses
2) Create a second page on the google form and name it something like `responsecount` (not sure that the name really matters here)
3) In cell `A1` of the `responsecount` page create an equation of the form
    ```
    =COUNT('Form Responses 1'!A:A)
    ```
    It should read whatever number of responses the form currently has.
4) In the help bar of the google sheet, search for "Publish to web" and then publish ONLY the `responsecount` page as a web page.
5) Copy the URL of the published web page.
6) Edit the `survey_progress.html` page and change the URL in the javascript to the published page that you just copied.
7) Then adjust the `totstu` variable to the current number of students in the program.
8) Update the year in the header to the current year.
9) (Optional) Adjust the success text to whatever the reward is for reaching 80% participation
