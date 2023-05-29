# Donation-Dashboard

## Pre-requisites

- Install below packages

```bash
sudo apt install python3-pip
sudo apt install git

pip3 install requests
pip3 install streamlit
pip3 install python-dotenv 
pip3 install regex 
pip3 install pandas 
pip3 install fuzzywuzzy 
pip3 install python-Levenshtein 
pip3 install nameparser 
pip3 install plotly-express 
pip3 install openpyxl
```

- Set up locale for Indian Currency
```bash
sudo apt install locales
sudo locale-gen en_IN.UTF-8
```

- Ensure and Set up proper system time on the server/machine
```bash
## Display Current Date and Time with timedatectl
timedatectl

## Sync Time to NIST Atomic Clock
sudo timedatectl set-ntp yes

## Set Timezone
sudo timedatectl set-timezone Asia/Kolkata

## Set Hardware Clock to Sync to Local Timezone
timedatectl set-local-rtc 1
```

- Create a .env file with below parameters. Replace # ... with appropriate values
```bash
AUTH_CODE= # Raiser's Edge NXT Auth Code (encode Client 
REDIRECT_URL=# Redirect URL of application in Raiser's Edge NXT
CLIENT_ID=# Client ID of application in Raiser's Edge NXT
RE_API_KEY=# Raiser's Edge NXT Developer API Key
MAIL_USERN= # Email Username
MAIL_PASSWORD= # Email password
IMAP_URL=# IMAP web address
IMAP_PORT=# IMAP Port
SMTP_URL=# SMTP web address
SMTP_PORT=# SMTP Port
SEND_TO='email_1, email_2' # Email ID of users who needs to receive the report
CC_TO='email_3, email_4' # Email ID of users who will be CC'd for the report
ERROR_EMAILS_TO=# Email ID of user who needs to receive error emails (if any)
```