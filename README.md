Programmable Voice: Recording Application Server - Python
===
This repository contains the server-side web application required to run the 
[Server ](https://www.twilio.com/docs/quickstart/python/twiml/record-caller-leave-message) written in Python.



Prerequisites
---

* A Twilio Account. Don't have one? [Sign up](https://www.twilio.com/try-twilio) for free!

Up and running
---

This web application needs to be accessbile on the public internet in order to receive webhook requests from Twilio. Ngrok is a great options for getting this done quickly.

### Deploy locally using Python and [Ngrok](https://ngrok.com/)

For this option, you'll need to have the following tools installed on your development machine:

* [Python](https://www.python.org/) and `pip`
* [Ngrok](https://ngrok.com/)

Once you've got those, run the following command to install the required Python packages from within this project's parnet directory:

    pip install -r requirements.txt

Once that's done you can start the server by executing

    python server.py

And then, in a separate terminal window, make your server available to the public internet with the following:

    ngrok http 5000

You should see a dynamically generated public Ngrok URL in the command window. Ngrok will now tunnel all HTTP traffic directed at this URL to your local machine at port 5000.


### Deploy to the cloud using [Heroku](https://heroku.com)

Don't want to run the application server locally? You can also deploy it to the cloud using Heroku.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

Test the app
---

Add url from heroku add to Tools -> TwiML Apps -> Choose Phone ->Voice -> Request URL

---


License
---
MIT
