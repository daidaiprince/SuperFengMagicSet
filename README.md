# 超級小楓魔法設定

**功能 : Windows XP 系統調校工具**

**撰寫 : 吳彥楓**

![超級小楓魔法設定](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG01.png?raw=true "超級小楓魔法設定")
&emsp;
&emsp;
&emsp;
&emsp;

## 使用限制
目前測試可在 Windows XP 系統上執行,其他 windows 系統執行多數功能無效。

## 開發緣由
學習 VB 語言使用控制元件 ( OCX ) 的時候，無意間在網路上找到登錄機碼存取的 OCX ，搭配書籍--登錄檔大全，完成具系統調整的軟體。
&emsp;
&emsp;


## 開發環境
程式語言 : VisualBasic6.0 + ServicePack5




## 程式範例

建立機碼值
```
Reg1.hKey=HKEY_CURRENT_USER 
Reg1.Path="Software\Microsoft\Windows\CurrentVersion\Policies\Uninstall"
Reg1.CreateKey 
Reg1.ValueName="NoAddRemovePrograms" 
Reg1.Data=1 
Reg1.DataType=REG_DWORD 
Reg1.SetValue
```

修改機碼值
```
Reg1.hKey=HKEY_CURRENT_USER 
Reg1.Path="ControlPanel\Desktop" 
Reg1.ValueName="MenuShowDelay" 
Reg1.Data="1" 
Reg1.DataType=REG_SZ 
Reg1.SetValue
```

刪除機碼值
```
Reg16.hKey=HKEY_CURRENT_USER 
Reg16.Path="ControlPanel\Desktop" 
Reg16.ValueName="SmoothScroll" 
Reg16.DeleteValue
```



## 軟體畫面

自動執行

當 Windows 開機時會自動執行一些應用程式，一般的取消方式是在開始功能表中的[啟動]上刪除，可是有些程式並不會在這個資料夾中，便可藉此來取消開機時自動執行的程式。

![自動執行](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG02.png?raw=true "自動執行")
***
移除軟體 

透過控制台的 [ 新增或移除程式 ] ，我們可以對系統進行新增或移除程式的動作，如果你不希望別人透過這個程式，任意新增程式到電腦中，或者把你所安裝的程式移除，可藉此來禁止或停用功能。 

![移除軟體](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG03.png?raw=true "移除軟體")![移除軟體](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG04.png?raw=true "移除軟體")
***
開始選單

開始功能表和工作列，可以說是 Windows 中最常操作的地方，裡面幾乎提供了大半執行的功能，如果你不希望別人輕易地透過開始功能表，對系統進行各項操作，可透過此設定將一些項目隱藏起 來，避免透過開始功能表和工作列進行設定，以保護系統使用的安全性。

![開始選單](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG05.png?raw=true "開始選單")
![開始選單](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG06.png?raw=true "開始選單")
***
開機 

與開機相關的選項，除了可以自訂登入歡迎畫面的背景之外，還有開機固定開啟數字鍵、關閉自動 重新啟動…等功能可以設定。

![開機](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG07.png?raw=true "開機")
![開機](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG08.png?raw=true "開機")
***
網路加速

Windows 預設的網路參數較為保守，並沒有將速度發揮到最大的效能，你可以透過這個選項來調整設定，讓網路速度達到極限。

![網路加速](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG09.png?raw=true "網路加速")
***
IE 瀏覽器

如果你不想要被別人更改你的 IE 首頁或是禁止別人在你的電腦上下載檔案，或者是你想要自訂 IE 視窗的標題列…等，舉凡和 IE 相關的選項，都可藉此來設定。

![IE 瀏覽器](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG10.png?raw=true "IE 瀏覽器")![IE 瀏覽器](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG11.png?raw=true "IE 瀏覽器")
![IE 瀏覽器](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG12.png?raw=true "IE 瀏覽器")![IE 瀏覽器](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG13.png?raw=true "IE 瀏覽器")
***
硬碟與光碟機 
 
硬碟和光碟機是電腦中最常被使用的零組件，如果你不想讓別人任意瀏覽磁碟機的內容或者是光碟機的相關設定，要讓它們在使用上能更安全、更有效率，可藉此選項來調整其運行狀態。

![硬碟與光碟機](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG14.png?raw=true "硬碟與光碟機")![硬碟與光碟機](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG15.png?raw=true "硬碟與光碟機")
***
核心元件

主機中的微處理器和記憶體，可透過此設定達到最佳化的效能。

![核心元件](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG16.png?raw=true "核心元件")
***






