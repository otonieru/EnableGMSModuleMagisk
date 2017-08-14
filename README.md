## Brief Explanation
I always find that Google Play Services is way too aggresive in doing its activities in the background. And its no secret that this main services from google is oftenly one of the main culprit for the sub par battery performance on most stock or even custom ROM across devices.

## The Idea & The Barrier
Starting in Android 6.0, Google has introduced one of my favorite features in battery saving : DOZE (quick read about this Here), it help us to make apps go into a "shallow" hibernation state. Where it use less energy but retain it's functionality.

Thing is, this feature is NOT applicable for Google Play Services. Thus, it cant help you to save the battery from being eaten by Google Play Services. And this is not for no reason of course (read SIDE EFFECT/NOTE section bellow for further explanation)

## THE SOLUTION
Quick study reveal that Google put simple configuration is /system/etc/sysconfig/google.xml that WHITELISTING Google Play Services from the DOZE Mechanism.

So to make DOZE able to work on it, we simply need to remove the whitelisting.

This is WHAT THIS MODULE DO - SYSTEMLESSLY (obviously)

By installing this module, you can move Google Play Services from the "App Not Optimised" list to "App Optimised" which mean DOZE mechanism will work its magic on Google Play Services, thus should saving you more juices/batt throughout the day.

## The Side Effect/ Note
Saving energy never come without side effect. Same goes with this method.

By enabling Doze on Google Play Services, it will theoritically delay/pause some it's services. Most noticeable might be the GCM (cloud messaging) services.

App that use this services might experience delay in notification when Doze already kick in.

Although, in my experience (i use this mod on all of my three devices) my notif for LINE, WhatsApp and Telegram (my main comm app) is never been delayed. ( I put all these apps in my whitelist btw)

The one i noticed had slight delay is GMail. But i check my mail regularly throughout the day, so i need no real time notif for that.

As for all other main services like Accounts, Alarm, Location and elses, i never have any issue with them when i got this module active. GPS work fine, Alarm ringing, Account Syncing normally.

## CHANGELOG
v1. Initial Release
v2. Template Update
v3. Code Cleaning
v4. Template Update for Magisk 13.3

## Support
Find support on my thread @XDA : https://forum.xda-developers.com/apps/magisk/module-enable-doze-google-play-services-t3608783/post72344542#post72344542

## Copyright
otonieru@xda-developers may 2017
If you wish to implement the modification into your ROM, please mention me :)
