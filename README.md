楔子：初始化环境
npm install
npm start

一、生成资源
android：
react-native bundle --platform android --entry-file index.android.js --bundle-output ./bundles/index.android.bundle --assets-dest ./bundles/ --dev false

ios：
react-native bundle --platform ios --entry-file index.ios.js --bundle-output ./bundles/index.ios.bundle --assets-dest ./bundles/ --dev false

二、注册CodePush
code-push register

三、注册App（android和iOS分开）
code-push app add testIOS
code-push app add testAndroid

四、集成CodePushSDK
npm install --save react-native-code-push
react-native link react-native-code-push



