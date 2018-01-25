# SignAppToPlatform

Run the sign.sh to get platform.jks, use this to give app a platform sign.
Add the following code in your build.gradle to use:

signingConfigs {
        release {
            storeFile file("../../SignApk/platform.jks")
            storePassword '******'
            keyAlias 'platform'
            keyPassword '******'
        }

        debug {
            storeFile file("../../SignApk/platform.jks")
            storePassword '******'
            keyAlias 'platform'
            keyPassword '******'
        }
}
