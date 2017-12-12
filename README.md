# OTP via React-Native & Firebase
## Setup Firebase
### Create Firebase Cloud Project
* Go to: http://firebase.google.com
* Click "Get Started"
* Click "Add Project"
* Type a name to the project

### Setup Firebase Local Env.
* ```npm install -g firebase-tools```
* ```firebase``` ⇒ Verify firebase installed
* ```mkdir otp_server```
* ```cd otp_server```
* ```firebsase login``` ⇒ Login to Firebase
  * A URL will generate on the terminal..
  * Copy the URL from terminal to a web browser and login to google account
* ```firebase init``` ⇒ Generate local Firebase boilerplate
  * Select this options:
  * ***Firebase cli*** ⇒ select: ***functions***
  * ***Associate*** ⇒ select: ***[don’t setup]***
  * ***Database rules*** ⇒ press *enter*
  * ***Install dependencies with npm?*** ⇒ select: ***yes***
  * Wait 2 min… :)
  * ```firebase use --add``` ⇒ link you local project to cloud project
    * ***Which project do you want to add?*** ⇒ select the project created in cloud
    * ***What alias do you want to use for this project?*** ⇒ type any name
  * ```firebase deploy``` ⇒ deploy local project to cloud project
  * https://console.firebase.google.com/project/<my_proj_name>
  ```firebase deploy --project my_proj_namne```

## Configure Twilio
* Go to: http://www.twilio.com
* Login
* Pick American phone number
* Twilio Credentials http://www.twilio.com/console
