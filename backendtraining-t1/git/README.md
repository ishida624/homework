# 前言
版本控制系統大概是最基礎的工具，不管你是在前端、後端還是 APP。熟悉 Git 是基本技能。假設你現在是一個人開發 Web 專案，你至少需要熟悉以下流程。

# 推薦學習資源
中文書：[為你自己學Git](https://gitbook.tw/)

# 問題
- Q1: 請說明
    1. 什麼是版本控制系統？

        利用將每次修改過的檔案備份並且紀錄其修改的內容，若是新的版本有問題可以回到之前的版本，
        也可以紀錄修改的日期、修改人、修改的內容，方便一個團隊做開發。

    2. Git 版本控制中有哪幾種檔案狀態？

        分為未追蹤Unstracked
        有修改、還沒準備要被遞交 Changes not staged for commit
        有修改、準備要被遞交的檔案(在Staging Area) Changes to be committed
        已經被遞交的檔案 Committed

![](https://i.imgur.com/hZoDAPf.png)
- Q2: 上圖 A-J 是 Git 中檔案狀態切換得流程，請查出 A-J 執行的指令。(重點是確保自己真的學到在什麼情況下使用該指令。)
    - A: 將一般目錄變成 git working folder     ： git init
	- B: 將 working folder 的異動狀態登錄到 stage ：git add
	- C: 將 stage 的狀態放到 local repository  ：git commit
    - D: 將 local repository 的狀態放到 remote repository：git push
    - E: 將 remote repository 的狀態取回到 local repository：git fetch，git pull
    - F: 將 local repository 的狀態退回到 stage 階段（是 C 的逆向)：git reset HEAD^ --soft
    - G: 將 stage 的狀態退回到 working folder 階段（是 B 的逆向）git reset HEAD
    - H: 將 local repository 的狀態一口氣退回到 working folder 階段（是 B+C 的逆向) ：git rm  --cached
    - I: 從 remote repository 取回建立成新的 working folder  ：git clone
    - J: 將 git working folder 變回一般目錄 ：rm .git

- Q3. 做這個題目，你事前評估做了什麼、利用了哪些資源、排程為何、事後怎麼驗收、得到什麼經驗？

    事前評估：初步了解git是在做什麼後，了解到他是程式開發上必須的工具

    資源：中文書：[為你自己學Git](https://gitbook.tw/)、youtube相關影片

    排程：安裝git、了解git運作結構、學習git指令、申請github帳號，練習GitHub pull、push

    驗收：嘗試將檔案按照結構圖跑一次

    得到什麼經驗：了解到git版本控制對程式開發上的好處，以及以後在團隊作業上式必須的工具
