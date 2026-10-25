```
STM32/
├── LAB1/                      # 實驗一：GPIO 狀態機與按鈕防彈跳控制
│   ├── Core/
│   │   ├── Src/
│   │   │   └── main.c         # 實作 PC13 軟體防彈跳，依序切換 PA11、PA12、PB12 三顆 LED 的四段亮滅狀態
│   │   └── Inc/
│   │       └── main.h         # 相關硬體定義與標頭檔
│   └── LAB1.ioc               # 腳位設定 (PC13 設為 Input，PA11, PA12, PB12 設為 Output)
│
├── LAB2/                      # 實驗二：按鈕中斷控制 EXTI (紅綠 LED 閃爍與切換)
│   ├── Core/Src/main.c        # 實作外部中斷回呼函式，處理 50ms 防彈跳與即時顏色切換邏輯
│   └── LAB2.ioc               # 將按鈕腳位設定為外部中斷下降緣觸發 (EXTI Falling)
│
├── LAB2_challange/            # 實驗二挑戰題：非對稱頻率閃爍與中斷即時切換
│   └── Core/Src/main.c        # 實作動態調整 Delay 時間 (綠燈慢閃、紅燈快閃) 及中斷狀態同步
│
├── LAB3/                      # 實驗三：狀態機 (State Machine) 控制與綜合按鈕事件
│   ├── Core/Src/main.c        # 實作 NORMAL/WARNING/EMERGENCY 三種狀態切換與計時器自動轉換
│   └── LAB3.ioc               # 設定 PC9 (Polling) 與 PC13 (EXTI) 按鈕，及三色 LED 腳位輸出
│
├── LAB4/                      # 實驗四：UART 序列通訊與字串指令控制
│   ├── Core/Src/main.c        # 實作 LPUART1 接收字元緩衝、strcmp 指令解析與對應 LED 控制
│   └── LAB4.ioc               # 設定 LPUART1 (115200 Baud) 通訊腳位與雙色 LED 腳位輸出
│
├── LAB5/                      # 實驗五：Timer PWM 控制與單顆 LED 呼吸燈挑戰
│   ├── Core/Src/main.c        # 使用 HAL_GetTick 非阻塞計時與 __HAL_TIM_SET_COMPARE 動態更新亮度
│   └── LAB5.ioc               # 設定 TIM3_CH3 (PC8) 為 PWM 輸出，PSC 設為 84，ARR 設為 19999
│
├── README.md                  # 專案總說明檔
└── TEST.txt                   # 測試用檔案
```
