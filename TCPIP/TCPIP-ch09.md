### TCP/IP CH08 傳輸層協定(TCP)
# 簡介
# 埠編號
# UDP
# TCP
* 簡介
    * 傳輸層架構
        * 傳輸層介於網路層和會議層之間
        * 傳輸層協定標頭位於網路層協定標頭後
        * 傳輸層協定標頭位置
        ![傳輸層協定標頭位置](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/%E5%82%B3%E8%BC%B8%E5%B1%A4%E5%8D%94%E5%AE%9A%E6%A8%99%E9%A0%AD%E4%BD%8D%E7%BD%AE.png)
        * TCP UDP 處理時間及可靠性的關係
            * 可靠度: TCP>UDP
            * 處理速度UDP>TCP
        ![處理時間及可靠性的關係](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/TCP%20UDP%20%E8%99%95%E7%90%86%E6%99%82%E9%96%93%E5%8F%8A%E5%8F%AF%E9%9D%A0%E6%80%A7%E7%9A%84%E9%97%9C%E4%BF%82.png)
        * TCP資料傳送程序
        ![TCP資料傳送程序](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/TCP%E8%B3%87%E6%96%99%E5%82%B3%E9%80%81%E7%A8%8B%E5%BA%8F.png) 
* 埠編號
    * 佔有16位元
    * 由ICANN的IANA管轄
    * 具有三種類別
        * 公認埠:公共以及常用服務應用程式
        * 註冊埠:一班應用服務程式(須向IANA註冊後才能使用)
        * 動態埠:不被註冊佔有，能夠自由運用
    * 各類別埠型號
    ![各類別埠型號](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/%E5%90%84%E9%A1%9E%E5%88%A5%E5%9F%A0%E5%9E%8B%E8%99%9F.png)
    * 兩機台運用埠編號進行連線
    ![進行連線](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/%E9%80%B2%E8%A1%8C%E9%80%A3%E7%B7%9A.png)
* UDP
    * 非可靠性傳輸模式
    * 不會檢驗是否成功將資料傳送給對方
    * 訊息長度單位:位元組(紀錄UDP標頭及其他所屬資料的總合長度)
    * UDP標頭
    ![UDP](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/UDP.png)
* TCP
    * TCP協定
        * 高可靠性傳輸模式
        * 比UDP複雜的標頭格式和定義
        * 三向交握
        * TCP標頭
        ![TCP](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/TCP.png)