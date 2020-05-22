# 前言
這次題目是借用了網路知名人物「胡立」所製作的小遊戲：http-challenge ，它當初也是為了讓他的學生了解 http 與串接 api 而設計了這些題目。我自己玩過，認為非常適合新手了解 http 的運作原理，所以我想讓大家玩玩這個遊戲。

雖然網路上滿好找到正確解答的，但我希望大家能夠不找解答，自己慢慢摸索來完成關卡。但希望大家不要只想著突破關卡，看到陌生的字句 or 功能，都要能自己發散學習，為了讓大家有一致的發散目標，我一樣會出幾個簡答題，請大家破關之後，也回答下方問題。

# 推薦遊玩工具
1. [curl](https://ec.haxx.se/) ：command line 使用 URLs 傳送資料的工具，當然也支援 http 協議。
2. [Postman](https://www.postman.com/) ：web api 測試工具。

不推薦純粹使用瀏覽器，原因自己去摸索

# 開始遊戲
## [Challenge](https://lidemy-http-challenge.herokuapp.com/start)

# 問題
強烈建議:等遊戲至少破完 LV10 再回答！

給大家強調一個觀念：

好想工作室不是一個補習班，我們不主動提供課程，也不限定學習範圍，大家在學習的時候要自己學習怎麼學習，從一個問題中如何看到(找到)自己不懂的東西，自己發散、收斂學習的內容也是自學最重要的課題。

大家可以先完成遊戲，再來看我的問題(題目要往下捲)，看看這段過程你有沒有自己發現這些問題。
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
準備好了嗎？
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
1. URI 中何為 Query String？如何使用?<br/>
    URI後面的參數。URI後面加上"?參數1=XX&參數2=XX"。

2. URI 與 URL 的差異？<br/>
    URL 是路徑，URI 是資源實際位置。

3. URI 的完整格式包含哪些東西？<br/>
    包含server name、路徑、檔案名稱。

4. content type：application/x-www-form-urlencoded 是什麼意思？<br/>
    是一種POST的傳送方式，在header中可設定content type，然後在BODY的部份設定傳送POST內容

5. http 的 request method 有哪些？分別是做什麼用的？<br/>
    *  GET：請求展示指定資源，在header中傳送，會顯示在URI上。
    *  HEAD：跟GET一樣，差別為response沒有body。
    *  POST：用於提交指定資源的實體，傳送量比GET更大，是在body中傳送所以較具保密性。
    *  PUT：以請求的 酬載 (payload)，替換目標資源，（就是修改、更新）。
    *  DELETE：移除目標資源。
    *  CONNECT：會和指定資源標明的伺服器之間，建立隧道（tunnel）
    *  OPTIONS：描述 目標資源 的 通訊選項
    *  TRACE：沿著目標資源的路徑執行訊息 loop-back 測試。
    *  PATCH：指定資源的部份修改，跟PUT的不同點在PUT是全部修改，PATCH是部份修改。


6. 何謂 endpoint？<br/>
    endpoint代表終點，URI最後的目錄。
