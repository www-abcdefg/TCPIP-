### TCP/IP CH08 IP協定
# IPv4位置
# DHCP
# DNS
# IP協定
# IPv6

* IPv4
    * IPv4位置:32位元(bits)所構成
    * 位址由ICANN管理
    * IP位址區
    ![IP位址區](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/IP%E4%BD%8D%E5%9D%80%E5%8D%80.png)
    * 各類IP位址格式
    ![各類IP位址格式](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/%E5%90%84%E9%A1%9EIP%E4%BD%8D%E7%BD%AE%E6%A0%BC%E5%BC%8F.png)
    * A類
        * 最左邊位元值設為0
        * 具有7個網路位元，24個主機位元
    * B類
        * 最左邊兩個位元設為10
        * 最左第一個位元介於128~191
        * 具有14網路位元，16個主機位元
    * C類
        * 最左邊三個位元設為110
        * 最左第一個位元介於192~223
        * 具有21個網路位元
    * D類
        * 多點群播
        * 最左邊第四個位元設為1110
        * 左邊第一個位元介於224~239
        * 沒有網路位元和主機位元的區分
        * 多點群播的群組皆需要一個D類位址
        * 一對多的方式進行資料傳送
        * 有效降低網路的資料傳送
    * E類
        * 最左邊四個位元設為1111
        * 左邊第一個位元介於240~255
    * 網路遮罩
        * 遮罩值由左到右
        * 網路位元:1，主機位元:0
    * 子網路規劃
        * 向主機借未進行子網路規劃以及網域位址與廣播位址的訂定
        ![子網路規劃](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/%E5%AD%90%E7%B6%B2%E8%B7%AF%E8%A6%8F%E5%8A%83.png)
* DHCP
    * 網路必須配置DHCP伺服器
    * 節點連線後以廣播方式與DHCP server聯繫
    * 節點IP由伺服器分配
    * 設定使用期限來避免長時間占用IP
* DNS
    * 網路藉由IP位置對節點進行定址
    * 根據節點特性，以名稱對節點進行表示
    * 名稱容易記憶，但真正的定址還是IP位址
    * 正向名稱查詢(由網域名稱查出IP位址)
    * 反向名稱查詢(由IP位置查得網域位址)
    * 網域名稱
        * 最多五個層級
        * 每一級名稱至少2個字元以上，最多不超過63個字元
        * 名稱總長度不超過253字元
* IP協定
    * 標頭以32個位元為單位
    * IP標頭欄位的定義
    ![IP標頭](https://github.com/www-abcdefg/TCPIP-/blob/main/TCPIP/picture/IP%E6%A8%99%E9%A0%AD.png)
* IPv6
    * IPv6位置:128位元(bits)所構成
    * 每秒分配出一萬個IP位址
    * 三種傳播形式
        * 單點
        * 多點
        * 任點
    * 移除廣播傳播
    * IPv6標頭
        * 主標頭+延伸標頭
        * 主標頭固定8個
        * IPv6主標頭格式