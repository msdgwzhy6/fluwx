## WeChat Not Installed on iOS?
if you have installed WeChat on your iPhone but you still catch an exception that "wechat not installed",just add the following
code to your *info.plist*:
```xml
<key>LSApplicationQueriesSchemes</key>
<array>
<string>weixin</string>
</array>
<key>NSAppTransportSecurity</key>
<dict>
<key>NSAllowsArbitraryLoads</key>
<true/>
</dict>
```
