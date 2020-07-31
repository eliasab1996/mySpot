<activity android:name=".ProfileActivity"></activity>
        <activity
            android:name=".LabelHomePageActivity"
            android:parentActivityName=".MainActivity" /> <!-- Note: we updated the parent activity -->
        <activity
            android:name=".LogInActivity"
            android:parentActivityName=".MainActivity" />
        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
<uses-permission android:name="android.permission.INTERNET" />
