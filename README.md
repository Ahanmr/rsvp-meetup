# RSVP Meetup for Events

An app for people to RSVP an event in meetup.com built in Python.
* Needs Chrome for working.
* Selenium tool for automation of task.


### Improvements not addressed yet
There are some other minor features I would like to add:
- send email or SMS for RSVP success
- more browsers options to use
- multiple events options
- save and load credentials feature


# How to install dependencies
I use 3.5. Other python versions might work too.
### install Selenium
For Mac OS X, I put it here
```shell
/usr/local/bin/
```
Make sure you choose the same version like your Chrome version
[how to install selenium](https://selenium-python.readthedocs.io/installation.html)

# How to set Credentials
Make a json file root/rsvp_meetup/data/user_account.json with the following content and save.
```shell
{
"USER_NAME" = "your_email_address@gmail.com",
"PASSWORD" = "your_password",
"ACCOUNT_ID" = "meetup_account_id"
}
```
Make a json file root/rsvp_meetup/data/group_list.json with the following content and save.
```shell
["Name-of-your-meetup-group-you-want-to-RSVP-to"] # make sure your group target only has one event at a time.
```

# Setup and Run
After all of the dependencies are installed and the credential file is ready, then install and run
```shell
git clone https://github.com/Ahanmr/rsvp-meetup
cd rsvp-meetup/rsvp_meetup
python __init__.py
```

