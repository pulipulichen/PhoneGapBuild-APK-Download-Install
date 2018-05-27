# PhoneGapBuild-APK-Download-Install
An Android APP to create shortcuts for download an APK and installing it.

# TODO
- 偵測網頁要開啟的檔案類型或網址是否是APK...還是算了


- GitHub: https://github.com/pulipulichen/PhoneGap-ShareToEvent
- PhoneGap Build: https://build.phonegap.com/apps/3176725/builds

- Install: https://bit.ly/2IKsRrk
![Install](https://chart.googleapis.com/chart?chs=116x116&cht=qr&chl=https://build.phonegap.com/apps/3176725/install/DNZBQy-QDMDQZAi-AzzK&chld=L|1&choe=UTF-8)


# Reference
- Icon: http://www.iconninja.com/green-share-sharethis-sharing-icon-288495


https://dotblogs.com.tw/hanry/archive/2012/07/05/73239.aspx
安裝 APK 檔
Uri uri = Uri.parse("url_of_apk_file"); 
Intent it = new Intent(Intent.ACTION_VIEW, uri); 
it.setData(uri); 
it.addFlags(Intent.FLAG_GRANT_READ_URI_PERMISSION); 
it.setClassName("com.android.packageinstaller", 
                "com.android.packageinstaller.PackageInstallerActivity"); 
startActivity(it);  
//make sure the url_of_apk_file is readable for all users  