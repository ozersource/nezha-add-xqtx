## nezha-add-xqtx
哪吒面板增加續期提醒
### 功能：
面板信息中的國旗增加中文提示，有的國旗不認識，鼠標懸停可以看到國家名稱
面板信息中的在綫增加續期提醒，點擊對應的主機，彈出信息框，輸入續期時間即可
 續期時間5天以上，字體黑色；續期時間3-5天，字體藍色；續期時間2-3天，字體橙色；續期時間0-2天，字體紅色；
### 前端代碼
* 修改代碼中的兩個地址：
```
 fetch('https://xxx/xxx.php') //json url 改成後端讀取數據地址（readexp.php)
  $.post('https://xxx/yyyy.php', JSON.stringify({ serid: id, expdate: expdate }))//json url 改成後端存儲數據地址(update.php)
```
* 放在面板設置裏（自定义代码(style、script 都可以)），***只適配了defalut主題***
### 後端代碼
提供PHP示例
 update.php是保存續期時間的示例
 readexp.php是讀取續期時間的示例
### 部署
直接部署在支持PHP的服務器上，注意前端的鏈接地址

##更多内容，請關注[博文](https://mocikate.eu.org "雨絲部落格")
