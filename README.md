# SecureChat
Simple end-to-end encryption/decryption widget for securing SMS text messages.

This is a stand-alone HTML form with embedded Javascript utilizing the Web Crypto API and AES-256-CTR encryption, which allows you to encrypt sensitive information before you send it to a recipient.  All encryption and decryption takes place on your mobile device.  No passwords or keys are transmitted to a server or stored within a messaging app; it is completely self-contained.

After the message is encrypted it is then encoded using Base64 which can easily be sent over SMS text messaging.  The recipient will need to use this same HTML form to decrypt the message.  The sender and recipient will need to use the same password to encrypt and decrypt messages.  You should agree on a shared strong password ahead of time by some other means, and not transmit the password in plaintext to the other party through a text message.

**Example screenshots of how to use the SecureChat widget**

Sender encrypts the message then copies the output and sends it as a text message to the recipient.

:warning: Be sure to verify that the cipher text you paste into your text message is correct.  Some mobile device auto-correct settings will try to capitalize the first letter or convert math symbols to equations.

![alt text](https://raw.githubusercontent.com/billchaison/SecureChat/main/e.png)

Recipient decrypts the message by copying it then pasting it into the input field using the same password.

![alt text](https://raw.githubusercontent.com/billchaison/SecureChat/main/d.png)

**Installing the SecureChat widget**

[Here is a link to the raw HTML](https://raw.githubusercontent.com/billchaison/SecureChat/refs/heads/main/secure_chat.html)

iPhone users have a couple of options:

* Download the raw HTML from the link above and save it to your Files then open it using Edge browser.
* Install the [JS Anywhere](https://apps.apple.com/us/app/javascript-anywhere-jsanywhere/id363452277) app from the App Store then create a new project named Secure Chat.  In the new project delete the default JS, HTML and CSS content, then download the raw HTML from the above link into the HTML section.  Press the play button in the JS Anywhere app to execute the web form.

For Android users:

* Save the HTML file from the above link and open in Chrome browser.
