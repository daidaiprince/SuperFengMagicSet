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
&emsp;
&emsp;
&emsp;
***

移除軟體 
 
透過控制台的 [ 新增或移除程式 ] ，我們可以對系統進行新增或移除程式的動作，如果你不希望別人透過這個程式，任意新增程式到電腦中，或者把你所安裝的程式移除，可藉此來禁止或停用功能。 

![移除軟體](https://github.com/daidaiprince/image-database/blob/main/SUPERFENG03.png?raw=true "移除軟體")
&emsp;
&emsp;











