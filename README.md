# Amazon_App
React-Native ile amazon uygulaması hazırlanmıştır.
Yapı dinamik hazırlanmııştır.
Veriler Data klasörü içerisinden alınmıştır.
Proje oluşturulmadan önce hataları en aza indirmek için kütüphaneleri ilk olarak import edip daha sonra pod install yapmayı unutmayalım.
# Uyarı
   /*! importların doğru yerden alındığına dikkat ediniz. */


# kütüphaneler
- npm install @react-navigation/native
- npm install react-native-screens react-native-safe-area-context
- npm install @react-navigation/stack 
index.js içerisine import et
      import 'react-native-gesture-handler';
      
- npm install react-native-gesture-handler
- npm install @react-native-masked-view/masked-view
- npm i react-native-linear-gradient
- npm i react-native-swiper
- npm install --save react-native-vector-icons
 ios/amazon/info.plist sonuna yapıştır.
 <key>UIAppFonts</key>
<array>
  <string>AntDesign.ttf</string>
  <string>Entypo.ttf</string>
  <string>EvilIcons.ttf</string>
  <string>Feather.ttf</string>
  <string>FontAwesome.ttf</string>
  <string>FontAwesome5_Brands.ttf</string>
  <string>FontAwesome5_Regular.ttf</string>
  <string>FontAwesome5_Solid.ttf</string>
  <string>FontAwesome6_Brands.ttf</string>
  <string>FontAwesome6_Regular.ttf</string>
  <string>FontAwesome6_Solid.ttf</string>
  <string>Foundation.ttf</string>
  <string>Ionicons.ttf</string>
  <string>MaterialIcons.ttf</string>
  <string>MaterialCommunityIcons.ttf</string>
  <string>SimpleLineIcons.ttf</string>
  <string>Octicons.ttf</string>
  <string>Zocial.ttf</string>
  <string>Fontisto.ttf</string>
</array>

- android/app/build.gradle (NOT android/build.gradle) and add:

apply from: file("../../node_modules/react-native-vector-icons/fonts.gradle")

- rootProject.name = 'MyApp'

include ':app'

+ include ':react-native-vector-icons'
+ project(':react-native-vector-icons').projectDir = new File(rootProject.projectDir, '../node_modules/react-native-vector-icons/android')

- Edit the android/app/build.gradle (located in the app folder) as shown below:
implementation project(':react-native-vector-icons')# Amazon_Clone_Mb
