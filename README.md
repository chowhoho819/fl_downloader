# fl_downloader

A plugin to download files using the native capabilities.

On Android it uses the DownloadManager system service to download files to user's **Download** folder and, on iOS, it uses the URLSession to download files to the **App Documents** folder.

## iOS Configuration

If you don`t want to show downloaded files to the user on the Files app, there is no need for special configuration.

If you want to show downloaded files to the user on the Files app, add the following lines to your **info.plist** file:

``` xml
<key>LSSupportsOpeningDocumentsInPlace</key>
<true/>
<key>UIFileSharingEnabled</key>
<true/>
```

## Android Configuration

There is no need for special configuration
