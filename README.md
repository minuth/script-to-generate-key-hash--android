# script to generate key-hash android
# debug mode
keytool -exportcert -alias androiddebugkey -keystore debug.keystore | openssl sha1 -binary | openssl base64
# password for debug mode
android
# release mode
keytool -exportcert -alias [0aliasName] -keystore [keystoreFilePath] | openssl sha1 -binary | openssl base64
