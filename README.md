# MONITOR-MODE-for-Samsung-Galaxy-A03-Core-SM-A032F-S9-BINARY
So no one did enabled monitor mode for this phone soo I have modules that I compiled it took me months to make them work on my phone trial and error here is it also I am using MT7601U adapter also I provided only it's module if you want to compile more adapters use the S8 binary you can find it in Samsung OpenSource it worked use the correct vermagic of your phone 
make sure your phone boatloader is unlocked and rooted
to execute them enter any root shell termux or adb type
su
insmod /sdcard/Download/cfg80211.ko
insmod /sdcard/Download/mac80211.ko
change the path based on your path destination
if you have another Antennas that it support monitor you can just conpile them just feel the pain as me i felt it
for the antenna MT7601U here is the command:
su
insmod /sdcard/Download/mt7601u.ko
