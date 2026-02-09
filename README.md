# mobile-app-testing

Do you skip Android apps during bug hunting? You might be missing out on hidden bugs! 🐛

I’ve had conversations with several hunters who lack confidence or overlook mobile apps, but Android apps often have hidden endpoints or API calls not visible in the web interface. This could mean missing out on valuable findings.

🔍 To discover these, try dynamic analysis: run the app on your device/Genymotion, intercept traffic using tools like Charles Proxy or mitmproxy. Inpsect all API calls and unusual behavior and perform further testing on these to look for IDORs, RBAC, CSRFS, etc.

📂 For static analysis, tools like MobSF allow you to review Java classes for discovering hidden endpoints, or you can extract URLs directly from APKs using apkurlgrep or apk2url.

I’ve often found High/Critical bugs in Android apps when the web version had no issues. The takeaway? Always check mobile apps during bug bounties!
