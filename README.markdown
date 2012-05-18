# reCAPTCHA

## Installation
1. Get reCAPTCHA API keys from http://recaptcha.net/whyrecaptcha.html
2. Upload the 'recaptcha' folder in this archive to your Symphony 'extensions' folder.
3. Enable it at System > Extensions.
4. Go to System > Preferences and enter your reCAPTCHA private/public API key pair.
5. Add the "reCAPTCHA Verification" filter rule to your Event via Blueprints > Events
6. Save the Event.
7. Add "reCAPTCHA: Public Key" Data Source to your page.
8. Add the following line to your form: 

    
    <script type="text/javascript" src="http://api.recaptcha.net/challenge?k={/data/recaptcha}"></script>

See http://recaptcha.net/apidocs/captcha/client.html for information about customisation of the reCAPTCHA box.