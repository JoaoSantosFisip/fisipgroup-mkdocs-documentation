# How to publish for the Android Platform
## About
Here's the documentation on how to publish an apk to the Google's Play Store. 

[Google Play Console Dashboard](https://play.google.com/console/u/2/developers/)

## Requirements
- Google developer account<p style = "font-size:10px;">(Should be created with the fisipgroup email)</p>
- Be on FisipGroup's google organization.
- Have the right permissions.

## Build the APK/AAB
1. Go to `File -> Build Settings`.
2. Make sure the `Build App Bundle (Google Play)` checkmark is on, and the `Development Build` is off.
![Player Settings](images/base/publish/android/publish_android_1.png)
3. Go to `Player Settings... -> Other Settings`.
4. Increment the `Bundle Version Code` value.
    - Make sure it's one value above the last published build.
    - If the `FisipGroup Addressables` custom package is *NOT* integrated, change the `Version` to the same value, otherwise it will update automatically.
    ![Player Settings](images/base/publish/android/publish_android_6.png)
    - You can find the last published build on the overview page `Home -> App -> Releases Overview`: [Google Play Console Dashboard](https://play.google.com/console/u/2/developers/)
    <figure markdown="span">
    ![Releases Overview](images/base/publish/android/publish_android_7.png)
        <figcaption>The highest one on all tracks</figcaption>
    </figure>
5. Set keystore's password on `Publishing Settings`. The password should be on a text file inside the project on `Assets -> Help -> SigningKeyPassword`. 
    <p style = "font-size:12px;">If not contact a developer that worked on the specific game.</p>
![Keystore Password](images/base/publish/android/publish_android_10.png)
6. Go back to `Build Settings` and press `Build` or `Build and Run` to build an `.abb` file.
7. Save the `.abb` file on a location of preference.
8. If the `FisipGroup Addressables` custom package is integrated, select if you want some of the game files to be loaded from the `Cloud` or be added to the `.abb` file.
![Keystore Password](images/base/publish/android/publish_android_3.png)

## Publish on Google Play Console
1. Go to the [Google Play Console Dashboard](https://play.google.com/console/u/2/developers/).
2. Select the game app you are working on.
![App select](images/base/publish/android/publish_android_4.png)
3. Go to the `Release` section and select the type of release.
4. Select `Create new release`. If the button is greyed out there is a draft of a release already and instead go to `Releases -> Edit Release`.
![release](images/base/publish/android/publish_android_5.png)
5. Drag the `.abb` file to the App Bundles box.
![App bundle](images/base/publish/android/publish_android_8.png)
6. Add the `Release name` and `Release notes`. 
For the release notes we usually go to gitkraken or trello and get a list of all the tasks done since last release. Only important on `production` releases.
![Release details](images/base/publish/android/publish_android_9.png)
7. Press `Next` once the `.abb` file as been uploaded and the notes added.
8. Select `Save and publish`.