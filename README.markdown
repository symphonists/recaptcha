# reCAPTCHA

## Installation
1. Get reCAPTCHA API keys from https://www.google.com/recaptcha/intro/index.html
2. Upload the 'recaptcha' folder in this archive to your Symphony 'extensions' folder.
3. Enable it at System > Extensions.
4. Go to System > Preferences and enter your reCAPTCHA private/public API key pair.
5. Add the "reCAPTCHA Verification" filter rule to your Event via Blueprints > Events
6. Save the Event.
7. Add "reCAPTCHA: Public Key" Data Source to your page.
8. Add the following script to your site: 

```HTML    
<script src="https://www.google.com/recaptcha/api.js" async defer></script>
```
8. Add the following html where you want your recaptcha to appear: 

```HTML    
<div class="g-recaptcha" data-sitekey="{/data/recaptcha}"></div>
```

See https://developers.google.com/recaptcha/intro for additional reCAPTCHA information / customization.
