##cordova-plugin-get-referrer

A cordova plugin to receive the referrer string from the Play Store on Android when the app is installed
It then writes the string to app preferences 

##Test: 

`adb shell`
`am broadcast -a com.android.vending.INSTALL_REFERRER -n <package_name>/com.roostermoney.getreferrer.Receiver --es "referrer" "utm_source=test_source&utm_medium=test_medium&utm_term=utm_test&utm_content=test_content&utm_campaign=test_name"`