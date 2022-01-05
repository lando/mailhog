MailHog Example
===============

This example exists primarily to test the following documentation:

* [MailHog Service](https://docs.devwithlando.io/tutorials/mailhog.html)

Start up tests
--------------

Run the following commands to get up and running with this example.

```bash
# Should start up successfully
lando poweroff
lando start
```

Verification commands
---------------------

Run the following commands to validate things are rolling as they should.

```bash
# Should have the mhsendmail binary
lando ssh -s php -c "ls -lsa /usr/local/bin | grep mhsendmail"

# Should have the MH_SENDMAIL_SMTP_ADDR set
lando ssh -s php -c "env | grep MH_SENDMAIL_SMTP_ADDR=sendmailhog:1025"

# Should be serving the admin interface on port 80
lando ssh -s php -c "curl mailhog | grep MailHog"

# Should have mailhog set as the meUser
lando ssh -s mailhog -c "id | grep mailhog"

# Should be able to collect messages sent from php
lando ssh -s php -c "php /app/mail.php"
lando ssh -s php -c "curl sendmailhog/api/v2/messages | grep leiaorgana@rebellion.mil"
```

Destroy tests
-------------

Run the following commands to trash this app like nothing ever happened.

```bash
# Should be destroyed with success
lando destroy -y
lando poweroff
```



