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
* ```firebsase login``` ⇒ Login to Firebase
  * A url will generate on terminal..
  * Copy url from terminal to web browser and login to google account
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
