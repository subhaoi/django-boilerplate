## Nsync
Skill assessment platform

**Setup**

```sudo apt install python3-virtualenv```

```virtualenv venv```

```source venv/bin/activate```

```pip install -r requirements.txt```

```sudo apt-get install libpq-dev postgresql postgresql-contrib```

```sudo su - postgres```

```psql```

```create database nsync_dev_db;```

```create user nsync_admin with password 'we_believe_in_quality_over_quantity';```

```alter role nsync_admin set client_encoding to 'utf8';```

```ALTER ROLE nsync_admin SET default_transaction_isolation TO 'read committed';```

```alter role nsync_admin set timezone to 'Asia/Kolkata';```

```GRANT ALL PRIVILEGES ON DATABASE nsync_dev_db to nsync_admin;```

**API**

***Login and Signup***
 1. /login 
 2. /signup
 3. /generate-otp
 4. /verify-otp

***Dashboard***
 1. /get-recommended-tests
 2. /get-all-tests
 3. /retrieve-results
 4. /show-results

***Personal Details***
 1. /get-phone-number
 2. /get-home-address
 3. /get-office-address
 4. /edit-phone-number
 5. /edit-home-address
 6. /edit-office-address

***Social Details***
 1. /get-facebook-details 
 2. /get-linkedin-details 
 3. /get-google-details
 4. /connect-facebook 
 5. /connect-linkedin 
 6. /connect-google
  
***Professional Details***
 1. /get-resume 
 2. /save-resume 
 3. /get-skillset 
 4. /add-skillset
 5. /get-current-company 
 6. /edit-current-company 
 7. /get-employment-type
 8. /edit-employment-type  
 9. /get-current-salary 
 10. /edit-current-salary
 11. /get-expected-salary 
12. /edit-expected-salary
 

**Settings**

 1. /get-username 
 2. /edit-password 
 3. /get-subscription
 4. /get-notification-preferences 
 5. /edit-notification-preferences
 

**Payment**

 1. /start-transaction 
 2. /get-transaction-status

 **Test**

 1. /start-test 
 2. /end-test 
 3. /save-results

