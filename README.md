# yc_0913
gzip
  ○壓縮：gzip FileName
  ○解壓縮：
    ■gunzip FileName.gz
    ■gzip -d FileName.gz8
xz
  ○壓縮：xz -z FileName
  ○解壓縮：xz -d FileName.xz
tar.gz
  ○壓縮：tar -zcvf FileName.tar.gz DirName
  ○解壓縮：tar -zxvf FileName.tar.gz9
檔案搜尋
○option
  ■-size EX：找出大於500M的檔案→ -size +500M
  ■-name EX：找出為照片的檔案→ -name "*.jpg"
  ■-type EX：-type f→ 一般檔案;  -type d→ 一般目錄
  ■-user EX：同時找兩個擁有者的檔案→-user user1 -o -user user2
○action -exec
  ■ls
  ■print10
檔案內容查閱
cat從第一行  顯示檔案內容、形成新檔案○cat -n file1 > file2→把file1的檔案內容加上行號後 輸入file2檔案
  ■-n  → 由1開始對  所有輸出的行數編號
  ■>    → 將多個文件覆蓋 到目 標文件中
  ■>>  → 將多個文件追加到目 標文件中，不覆蓋
tac從最後一行開始顯示
    ○tac -r -s 'x\|[^x] ' test.log→一個 接著一個字符的反轉一個文件
        ■-r→將分 隔符作為基  礎正規表達是處理
        ■-s→使用String作為分隔符代替默認的換行符12
more一頁一頁的顯示 檔案內容
    ○more +20 testfile→從第20行開始顯示testfile的文檔內容
        ■EN TER：向下n行(default為1行)
        ■Ctrl+F   /S PACE：向下滾動一屏
        ■Ctrl+B：返回 上一 屏
     ●less與more 類似 ，顯示 檔案 室允許  用戶既可以 向前又可以 向後翻頁   閱讀檔案
        ○ps -ef    |less→ps查看進程 信息並通過less分頁顯示
              ■j→下一行
              ■k→上一行
              ■G→移動 到最 後一行
              ■g→移動 到第一行13
當瀏覽器輸入網址，發出一個 GE T請求時， 過程中發生了哪些事情？
1.TCP三向交握在瀏覽器送出請求之後，瀏覽器和伺服器就會開始初步溝通，確定雙方的溝通管道順暢，以便後續請求的執行
2.瀏覽器請求、資料傳輸、渲染畫面如同前面所提，當三項交握結束後，瀏覽器和伺服器便會開始執行請求、資料傳輸與渲染畫面的過程
3.TCP四次揮手，結束連線在網頁成功渲染之後，瀏覽器就會和伺服器進行最後的溝通，確認傳輸過程已完成，準備結束連線
Linux指令-網路相關
  1.add:新增一條路由規則
  2.del:刪除一條路由規則
  3.-net:目的地址是一個網路
  4.-host:目的地址是一個主機
  5.target:目的網路或主機
  6.netmask:目的地址的網路掩碼
  7.gw:路由資料包通過的閘道器
  8.dev:為路由指定的網路介面



