# data-course-sample


這個是Alpha camp的推薦模型系統的課程演練題目

題目目的:
建立一個推薦系統，希望透過系統找到適合的商品，呈現到曾經在Amazon網站上購買過美妝商品的客戶的瀏覽頁面上增加其興趣

所應用的資料時間範圍:
Training Data:日期在2018-09-01之前的用戶評分資料
Testing Data: 日期介於2018-09-01及2018-09-30的用戶評分資料

資料介紹:
此資料集為2014 年 Amazon 發布的資料集，這個資料集中包含：
1.評論資訊 (評價星級、文字評價、投票等)
高達 2 億 3310 萬條評論資訊 (其中在 2014 年就新增了 1 億 4280 萬條)，包含 1996.05 - 2018.10 的資訊內容

2.商品後設資料 (商品描述、類別、價格、品牌、圖片資訊等)
我們在每一條評論資訊中能同時看到商品後設資料的功能，包含：
  商品資訊 - 顏色、尺寸、包裝版本(禮盒或電子產品) 等等 & 買家收貨後的實品照片
在商品頁呈現細節資訊，例如：
  以列點呈現品名以外的其他細項描述、以表格呈現技術屬性的細節、以表格比較其他相似產品
3.連結 (觀看資料、購買資料等)



使用的工具及平台
1.Colab
2.Python (package- gzip, json, pandas, numpy, datetime)


評估方式以及結果
用過往2014~2018-09-01前的商品資料及評論資料來Train推薦模型，並以2018-09-01及2018-09-30間的用戶購買行為作為模型的判別標準，以平均用戶評分當作最後的推薦衡量值(評分加總/總共test用戶數)
最後的分數為0.001694915254237288


反思
因為對於python工具的熟系度還不夠強烈，僅使用類似的人還買了什麼來作為推薦，評分結果對比於其他同學來說還有很大的進度空間，最近會好好找資料看看到底要怎麼寫模型，後續希望能做熱門推薦、其他人看過、協同式過濾、還有網路上一直交的Matrix & SVD得做法，


