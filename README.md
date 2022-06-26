#  z690 台式機 intel i7-12700k

用於我的工作站 hackintosh 的 OpenCore 引導加載程序配置文件。

## 系統信息

| 姓名 | 型號 |
| :------- | ------------------------------------: |
| 中央處理器 | intel i7-12700k |
| 顯卡 | AMD RX 5700xt |
| 固態硬盤 | 美光mx550-500gb |
| 無線網絡 | ax201(無法使用) |
| 主機板| ROG STRIX Z690-A GAMING WIFI D4  |
| 以太網 | Intel(R) Ethernet Controller I225-V |

- OpenCore：v0.8.1
- MacOS：v12.4 Monterey
- 
- (未來實現)
- OpenCanopy 主題：<https://github.com/tekteq/opencanopy-minimal-theme>

## 指南

<https://dortania.github.io/OpenCore-Install-Guide/prerequisites.html>

###  SMBIOS

已選擇：`MacPro7,1`

不要忘記更改設備uuid，板序列號和網絡mac地址
轉到 <https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#platforminfo> 有關設置 SMBIOS 平台信息的信息

## 使用的 Kext
| 包裝 | 版本 |
| :------------------------ | ------: |
| 蘋果ALC | 1.5.9 |
| 麗露 | 1.5.2 |
| VirtualSMC | 1.2.2 |
| 機場BcrmFixup | 2.1.2 |
| 瑞昱RTL8111 | 2.4.0 |
| NVMeFix | 1.0.7 |
| AppleMCEReporterDisabler | 1.2.0 |
| 限制事件 | 1.0.0 |

## 什麼有效

- [x] 圖形
- [x] 網絡服務
- [x] USB
- [x] 無線網絡
- [x] 藍牙
- [x] 睡眠
- [x] 音頻
- [x] iOS 模擬器

## 什麼不工作

-然而發現，一切似乎都運行良好。以太網未經測試。


## 預安裝

-更新 SMBIOS 和 MAC 地址
-開啟 4G 以上編碼，關閉 Resizable bar 支持
  
## 安裝後

-升級 OpenCore 版本
