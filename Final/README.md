# 網頁設計期末專案-留言板製作

前言
---
本專案程式碼並非全部原創!
- HTML
留言板頁面互相切換及一些JS的function模仿自[此](https://codepen.io/rosewang0303/pen/mXrEwQ)
- CSS
註冊及登入頁面的美化模仿自[此](https://codepen.io/rosewang0303/pen/mXrEwQ)
- JavaScript
帳號密碼的儲存(localstorage)學習自[五倍紅寶石，專業程式教育機構](https://5xruby.tw/posts/localstorage)
留言內容的儲存(Web SQL)參考自[CSDN](https://blog.csdn.net/qq_42285889/article/details/106669330)

## 內容新增
HTML
---
- 留言板發布頁面
從原本合併的發文頁面更改成兩頁獨立頁面
新增登出及刪除按鈕
          
CSS
---
- 註冊及登入頁面的美化
- 留言板發文頁面的美化

javascript
---
- 登入及註冊帳號時的會員資料儲存

        利用localStorage.setItem(key,value)的方式將使用者帳號及密碼儲存在
        localstorage裡面，並用localStorage.getItem(key)的方式將指定的"key"
        所對應的"value"取出來
- 留言內容的儲存
        
        留言板內容的部分則是用web db的方式將留言的內容儲存起來
- 刪除按鈕的function撰寫

        利用prompt得到使用者輸入的內容，並將其值傳入web db，如果有找
        到對應的數值，便刪除留言。

心得感想
---
畢竟將使用者的帳號密碼儲存在網路上實在太危險，且因為是將帳號儲存在local，因此沒辦法取得所有使用者的資料，只能簡單用作個人使用的用途，未來應該會朝學習php語法的方式，學習更加適合的儲存方法。
