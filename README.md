# project
The intention of the project is to detect the proxy given by students in colleges or schools. The app will take audio as an input.
Then the input data will be matched with each other to identify whether there is any similarity between the data. If similarity is found, then the proxy is detected.

First we need to take permissions like record audio, wake lock etc in android menifest

<?xml version="1.0" encoding="utf-8"?>
<manifest
    xmlns:android="http://schemas.android.com/apk/res/android"
    package="cafe.adriel.androidaudiorecorder.example">

    <uses-permission android:name="android.permission.RECORD_AUDIO"/>
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
    <uses-permission android:name="android.permission.WAKE_LOCK" />

    <application
        android:label="@string/app_name"
        android:theme="@style/AppTheme"
        android:icon="@mipmap/ic_launcher"
        android:allowBackup="true">
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>

Now we will be taking audio input and on users concern the audio data will be forwarded for processing.

You can refer the java files used in the project in the same repository.

