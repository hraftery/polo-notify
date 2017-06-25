# polo-notify
Python3 Script to check Poloniex for trades and either send an email via Sendgrid or send a notification via Pushed.

# Requirements

`python-poloniex` - to install: `pip3 install https://github.com/s4w3d0ff/python-poloniex/archive/v0.4.4.zip`
`sendgrid` - only for email notification method

# Configuration

Change the following values in the configuration section of the script:

1. Poloniex API and Secret  
1. Set balance reporting to true to get currency balances with the notifications
1. Update period in seconds
1. Notification method 'email' or 'pushed'
1. For email:
  1. Sendgrid API  
  1. Email address for from and to  
1. For Pushed notification:
  1. Pushed app\_key and app\_secret

# Python

Use the script directly with `python3 polo-notify.py`

# Docker

1. `docker build -t polo-notify .`
2. `docker run -it polo-notify`
