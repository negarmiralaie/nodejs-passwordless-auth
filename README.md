# nodejs-passwordless-auth
# What is passwordless-authentication?
## It's like a 2 factor authentication without its first factor. Normal login is done using a username and a password, but this way you only need to know your username. Its somehow as safe as 2 factor authentication. e.x: in medium.com -> For loggin in, you just enter your email, they sent and email containing a link, by clicking on that link you will be signed in -> And that's it, you will be logged in without having a password. 
### Benefits:
- There is no password to steal -> If data gets breached, password of user won't be stolen -> You even have not typed any password in your phone/laptop to be licked to others -> There will be no password reuse, if any other site gets breached and your password is stolen, attackers can not use your password to access your data at this site.
- Phishing attacks also won't work(they try to trick you into typing your password) bc there is no password to type. => A lot of attacks will be stopped only by stop using passwords. 
- You do not need to change or reset your password. 
- all above, makes it much easier for developers.
- User also does not need to remember his password.
### Downsides:
- Sending an email or etc to get loggedin, might take seconds or minutes so user might need to wait in this case.
- This way if you lose access to your email/phoneNumber you get access to your account


## passport-magic-login package:
    https://www.passportjs.org/packages/passport-magic-login/
    
    We are going to use this package, it sends a magic link to user to authenticate him...

    Install it using below command: 
    ```bash
    npm install passport-magic-login
    ```

    Link to frontend setup guideline:
    https://www.passportjs.org/packages/passport-magic-login/#:~:text=%2Dmagic%2Dlogin-,Frontend%20usage,-This%20is%20what

    Link to backend setup guideline:
    https://www.passportjs.org/packages/passport-magic-login/#:~:text=json.code%0A%20%20%20%20%7D%0A%20%20%7D)-,Backend%20setup,-To%20make%20this