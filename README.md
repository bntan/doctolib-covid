## Doctolib COVID

This script sends email alerts (using Google SMTP server) when vaccination appointments can be taken on Doctolib.

## Prerequisites
 
- Python 3

## Download dependencies

`$ pip install -r requirements.txt`

## Execution

- Set the vaccination centers close to your location in [centers.txt](../master/centers.txt)

- Set environment variables
  - DISABLE_EMAIL: set to true to disable email alerts
  - SENDER_EMAIL: the sender email address
  - SENDER_PASSWORD: the associated password
  - RECEIVER_EMAIL : the receiver email address

- Execute command
`$ python doctolib-covid.py`

## Cron

The cron [cron-doctolib-covid.yml](../master/.github/workflows/cron-doctolib-covid.yml) executes the script every 15 minutes
