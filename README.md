# Web Management System
簡易後台員工管理系統

基於SpringBoot及MyBatisPlus框架完成的簡易後台員工管理系統


技術使用:

1.配置專案開發所需Maven文件

2.基於MVC架構完成程式撰寫

3.使用Thymeleaf模擬前端回傳資料

4.調用API功能如:VerifyCodeUtils 完成圖形碼驗證碼功能,Jayspt對重要資訊進行加密,DigestUtils完成MD5加密

5.配置Cors同源跨域資源共享

6.使用MyBatisPlus對資料庫進行增刪改查操作

7.撰寫Test類進行單元測試


功能介紹:

1.註冊帳號密碼，會檢查是否與資料庫中已存在的帳號衝突，如衝突則跳轉到指定頁面

2.判斷驗證碼是否與圖形相等

3.登入輸入密碼後進行MD5加密，與資料庫中的MD5密碼進行比對

4.可上傳員工照片，刪除員工照片會自動連帶路徑內儲存的照片一同刪除

5.可對員工資料進行基礎的增刪改查

6.安全登出後會自動清除Session內的資訊

7.攔截未登入帳號的Session請求

8.利用Advice攔截未知異常，進行頁面跳轉
