# Magento 2 Admin Panel Two Factor Authentication
Two Factor Authentication to the Magento 2 admin panel using Google Authenticator

#### Server Time
It's extremely important that you keep your server time in sync with some NTP server.

## Installation
In your Magento 2 base directory run:  
`composer require pmclain/magento2-tfa`  
`bin/magento setup:upgrade`

* TFA must be enabled by the individual user by clicking 'Account Setting(user)' in the Magento 2 admin panel.
* Once there, the user is able to enable the two factor authentication and view the QR code for a Google Authenticator compatible application.
* Users with TFA enabled will not be able to log into the admin panel without a valid authentication code input on the Magento 2 admin login page.
* Users with TFA disabled can leave the 'Authenticator Code' field blank during login.

## Google Authenticator Apps:

To use the two factor authentication, your user will have to install a Google Authenticator compatible app, below are some currently available:

* [Authy for iOS, Android, Chrome, OS X](https://www.authy.com/)
* [FreeOTP for iOS, Android and Peeble](https://fedorahosted.org/freeotp/)
* [FreeOTP for iOS, Android and Peeble](https://www.toopher.com/)
* [Google Authenticator for iOS](http://itunes.apple.com/us/app/google-authenticator/id388497605?mt=8")
* [Google Authenticator for Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2")
* [Google Authenticator for Blackberry](https://m.google.com/authenticator")
* [Google Authenticator (port) on Windows app store](http://apps.microsoft.com/windows/en-us/app/google-authenticator/7ea6de74-dddb-47df-92cb-40afac4d38bb")
* [Microsoft Authenticator for Windows Phone](https://www.microsoft.com/en-us/store/apps/authenticator/9wzdncrfj3rj)
* [1Password for iOS, Android, OSX, Windows](https://1password.com)

## License
GNU GENERAL PUBLIC LICENSE Version 3
