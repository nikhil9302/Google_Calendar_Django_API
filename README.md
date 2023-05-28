# Google_Calendar_Django_API
## Working
First download this repo, and install dependencies by running `pip install requirements.txt`
Then, run `python manage.py runserver`, and go to the endpoints :
1) /rest/v1/calendar/init/ -> GoogleCalendarInitView() <br>
This view should start step 1 of the OAuth. Which will prompt user for
his/her credentials
2) /rest/v1/calendar/redirect/ -> GoogleCalendarRedirectView()<br>
This view will do two things: <br>
  i) Handle redirect request sent by google with code for token. You
  need to implement mechanism to get access_token from given
  code <br>
  ii) Once got the access_token get list of events in users calendar
  Screenshots of working of the API provided
