# STM32作業
## 📁 專案目錄與結構細節

```text
STM32/
├── LAB1/                       # 實驗一：(例如：GPIO 控制 LED 閃爍)
│   ├── Core/
│   │   ├── Src/
│   │   │   └── main.c          # 核心主程式碼 (實作 LED 控制邏輯)
│   │   └── Inc/
│   │       └── main.h          # 相關標頭檔
│   └── LAB1.ioc                # STM32CubeMX 腳位與時脈設定檔
│
├── LAB2/                       # 實驗二：(例如：按鈕中斷控制 EXTI)
│   ├── Core/Src/main.c         # 實作按鈕中斷服務常式
│   └── LAB2.ioc                # 包含中斷腳位設定
│
├── LAB2_challange/             # 實驗二挑戰題：(填寫挑戰題的目標)
│   └── Core/Src/main.c         # 挑戰題進階邏輯實作
│
├── LAB3/                       # 實驗三：(例如：Timer 計時器應用)
│   └── (依此類推，列出重要檔案)
│
├── README.md                   # 專案總說明檔
└── TEST.txt                    # 測試用檔案
