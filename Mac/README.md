## English

### Summary of ES_R-DevelopmentKit-Mac 
* "ES_R" means JINS MEME ES_R (previouslly called JINS MEME Academic pack)
* sample code included  
* Checked runnning on MacOS 11.5.2 and Xcode 12.5.1
* Dongle(BLE receiver) in NOT needed for Mac
* To record the data, you need to write codes as needed.

### STEP1 Download and Build the xcode project
* Download ES_R-Development-kit at https://github.com/jins-meme/ES_R-Development-Kit
* go to /ES_R-Development-Kit-master/Mac/ES_R_DevKit_Mac/
* launch "MEME_Academic.xcodeproj"
* Then, build the project

When, successfully build, sample UI shows up.
* ![successbuild](https://cloud.githubusercontent.com/assets/18042520/26821411/48e4c6ce-4ae1-11e7-844b-b424ae910582.png)

### STEP2 Connect JINS MEME ES_R
* Turn JINS MEME ES_R on. Then, press "Scan MEME" then connect your JINS MEME
* NOTICE that device Number shown in UI (e.g) 1C1-1047 in the image) is not equivalent to Bluetooth ID of JINS MEME  
![screen shot 2017-06-06 at 18 01 45](https://cloud.githubusercontent.com/assets/18042520/26821738/6faa99d6-4ae2-11e7-9e48-d62387ad4bf9.png)

* When your JINS MEME ES_R is connected, "Start Measurement" button shows up.
* Press "Start Measurement" button to start working JINS MEME
![screen shot 2017-06-06 at 18 02 08](https://cloud.githubusercontent.com/assets/18042520/26821755/7ef5c136-4ae2-11e7-9913-27c6ee52397d.png)

### STEP3 Enjoy making your original application

## Japanese(準備中です）

### ES_R_DevKit_Mac
最新版

#### ビルド方法について
* Hardened Runtimeがない場合
develop版としてビルド可能です。
（Hardened Runtimeがある状態でXcodeからMacにビルドするとエラーになります。
'/System/Library/Frameworks/CocoaAsyncSocket.framework/Versions/A/CocoaAsyncSocket' (no such file)
というエラーが出ている場合はSigning & CapabilitiesのHardened Runtimeを削除してください）

* Hardened Runtimeがある場合
配布アプリ版としてビルド可能です。

#### 配布アプリのビルド方法

* 1.Hardened Runtimeを追加する。
TARGETS > Signing & Capabilities > Hardened Runtime
* 2.アーカイブを作成する
Product > Archive
* 3.公証を得る
Archive > Distribute App > Deceloper ID > Upload
* 4.エクスポート（公証を得た後）
Archive > Distribute App > Deceloper ID > Export

### ES_R_DevKit_Mac_Simple
2022/9/1までの古いバージョン
