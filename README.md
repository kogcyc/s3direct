
# Upload an image file directly to S3 from the browser

### with help from Python

S3 allows files to be uploaded directly by using their REST API.

That process is detailed here: 
https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-authentication-HTTPPOST.html

This is a Python Flask app that renders a page which allows the user to enter the name of a file. Once the file name is selected, the page automatically calls back to the Flask app which then delivers the credientials needed for the page to send the file directly to S3.

To run this app locally, you will need to first set some environment variables:

- export AWS_ACCESS_KEY_ID=AKEYTHATISFAIRLYSECRET
- export AWS_SECRET_ACCESS_KEY=AreallySecretKeyJustInCase
- export S3_BUCKET=somebucket
- export FLASK_APP=app.py

Then run the Flask app:

- flask run
