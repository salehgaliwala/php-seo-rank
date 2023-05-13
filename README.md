# php-seo-rank
SEO suite php developed in laravel
Installation
Creating the database
Create a new MySQL database.
Create a new MySQL username and password.
Assign full privileges to your database username.
Useful resources
cPanel - MySQL database wizard
Plesk - Website databases
Uploading the files
Before starting to upload the files, please make sure your file explorer has the option to view hidden files turned on. On some operating systems, the dotfiles are hidden by default.

Upload what's inside the Software folder on the web root folder of your domain. This folder is generally called public_html, html, or example.com, but depending on your server's configuration, it might be named differently.

Useful resources
cPanel - File Manager
Plesk - Uploading content with File Manager
Configuring the files
Set the access permissions (CHMOD) to 775 to the following files and folders:

Files
.env
Folders
bootstrap/cache
lang
public/uploads/brand
storage
storage/framework/
storage/framework/cache
storage/framework/cache/data
storage/framework/sessions
storage/framework/views
storage/logs
Useful resources
cPanel - Update file or folder permissions
Plesk - Setting file and directory access permissions
Changing the public directory
Configure your web server's document / web root to point to the public directory of the software. For example, if you've uploaded the software in example.com folder, your web directory should be changed to example.com/public folder.

Useful resources
cPanel - New document root
Plesk - Defining a custom document root
Finishing the installation
Go to https://example.com/install and follow the installation wizard to complete the installation.
After you've installed the software, login into your user account.
Once logged-in, go to https://example.com/admin and activate your License Key.
Useful resources
Envato - Retrieving the license key
Configuration
Cron job
The software requires a cron job task to be set up on your server in order to automate some of its functions.

Go to Admin Settings Cron job.
Copy the Command field and set up a cron job for it that runs every minute.
Useful resources
cPanel - Cron jobs
Plesk - Scheduling tasks
Emails
Go to Admin Settings Email.
Change the Driver field value to SMTP.
Fill in the rest of the fields with the SMTP credentials from your SMTP provider.
Captcha
The Captcha system relies on Google reCAPTCHA's API.

Login into your Google reCAPTCHA account.
Create a new reCAPTCHA v2 Invisible Badge.
Fill all the other fields with the requested information.
Copy the Site key and the Secret key in Admin Settings Captcha.
Payment processors
To enable any of the payment processors, an Extended license is required. The payment processors can be enabled from Admin Settings Payment processors.

PayPal
Login into your PayPal account.
Go to the My apps & credentials section, click on Live button and then on the Create app button.
Copy the Client ID and Secret in Admin Settings Payment processors PayPal.
Go to the My apps & credentials section, click on Live button and then select your app.
Scroll down to LIVE WEBHOOKS and click on the Add webhook button.
On the Webhook URL field paste your webhook URL. This can be found on Admin Settings Payment processors PayPal.
Under the Events types select All events and save your changes.
Go to the My apps & credentials section, click on Live button and then select your app.
Copy the Webhook ID in Admin Settings Payment processors PayPal.
Stripe
Login into your Stripe account.
From the menu bar, go to the Developers section of the Stripe dashboard and click on API Keys.
Copy the Publishable key and Secret key in Admin Settings Payment processors Stripe.
From the menu bar, go to the Developers section of the Stripe dashboard and click on Webhooks.
Click on Add a new endpoint.
On the Endpoint URL field paste your webhook URL, which can be found on Admin Settings Payment processors Stripe.
On the events to listen to field, click on Select all events, and click on Add events button.
Click on Add endpoint button to create your webhook endpoint.
Copy the Signing secret in Admin Settings Payment processor Stripe.
Razorpay
Login into your Razorpay account.
From the menu bar, go to the Settings section of the Razorpay dashboard and click on API Keys.
Click on Generate key button.
Copy the Key ID and Key secret in Admin Settings Payment processors Razorpay.
From the menu bar, go to the Settings section of the Razorpay dashboard and click on Webhooks.
Click on Add new webhook.
On the Webhook URL field paste your webhook URL, which can be found on Admin Settings Payment processors Razorpay.
On the Secret field add your own secret passcode.
On the Active events field select all the Payment events and Subscription events.
Click on Create webhook button to create your webhook endpoint.
Copy the Secret passcode in Admin Settings Payment processor Razorpay.
Paystack
Login into your Paystack account.
From the menu bar, go to the Settings section of the Paystack dashboard and click on API Keys & Webhooks.
Copy the Public key and Secret key in Admin Settings Payment processors Paystack.
From the menu bar, go to the Settings section of the Paystack dashboard and click on API Keys & Webhooks.
On the Webhook URL field paste your webhook URL, which can be found on Admin Settings Payment processors Paystack.
Coinbase
Login into your Coinbase account.
From the sidebar, go to the Settings section of the Coinbase dashboard and scroll down to API keys.
Create an API key, and copy the key in Admin Settings Payment processors Coinbase.
From the sidebar, go to the Settings section of the Coinbase dashboard and scroll down to Webhook subscriptions.
Click on Add an endpoint.
On the Endpoint URL field paste your webhook URL. This can be found on Admin Settings Payment processors Coinbase.
From the sidebar, go to the Settings section of the Coinbase dashboard and scroll down to Webhook subscriptions.
Click on Show shared secret.
Copy the Webhook shared secret in Admin Settings Payment processors Coinbase.
Crypto.com
Login into your Crypto.com account.
From the menu bar, go to the Integrations section of the Crypto.com dashboard and click on API Keys.
Copy the Publishable key and Secret key in Admin Settings Payment processors Crypto.com.
From the menu bar, go to the Integrations section of the Crypto.com dashboard and click on Webhooks.
Click on Add webhook button.
On the Payload URL field paste your webhook URL, which can be found on Admin Settings Payment processors Crypto.com.
Copy the Signature secret in Admin Settings Payment processor Crypto.com.
Bank
All fields are optional.
Advanced
Google Custom Search
Follow the Google Custom Search guide to obtain a Search Engine ID and an API key.
Enable the Search the entire web when creating or editing your search engine.
Copy the Search engine ID and the API key in Admin Settings Advanced Google Custom Search.
KeywordsEverywhere
Follow the KeywordsEverywhere guide to obtain an API key.
Copy the API key in Admin Settings Advanced KeywordsEverywhere.
Thum.io
Login into your Thum.io account.
From the sidebar, go to the Keys section of the Thum.io and click on Generate new key.
Select the Type of the key to be HTTP Referrer Domain and fill the other fields according to your requirements.
Copy the API Key ID in Admin Settings Advanced Thum.io.
