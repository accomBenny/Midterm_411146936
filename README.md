# Mideterm Content

## 環境設定

下載並解壓縮玩課雲教材區中，Midterm下的3個檔案(.py, .md, .db)
下載並安裝Git
(非必要)下載並安裝DB browser for sqlite

## 專案起始

在桌面建立專案資料夾，名稱為Midterm_你的學號 (eg. Midterm_0583404)
將(.py, .md, .db)等3個檔案存於專案資料夾中
在GitHub上建立新的repository，名稱為Midterm_你的學號
利用git指令將該專案資料夾的內容push至GitHub上

## 常用之git指令提示

下列指令內容為簡要版，均在VS code提供之terminal中操作，<>中內容為指令說明
git init <初始化>
git config --global user.name <建立編輯者姓名>
git config --global user.email <建立編輯者電子郵件>
git add . <將資料夾內所有檔案加入追蹤>
git commit -m 'message(此處message須簡單交代此版本做了哪些修正)' <版本修改說明>
git remote add origin https://github.com/your_account/your_repository.git <連線至GitHub>
git branch -M main <更改目前branch名稱>
git push -u origin main <將資料夾內容推送至GitHub>


## 新增button_delete按鈕

修改視窗大小，由root.geometry('300x350') > root.geometry('300x400')
其餘程式碼，如投影幕所示
其功能是「從資料庫中刪除db_student_id為studend_id(從畫面輸入)之該筆資料」
注意，此處"僅須"確認程式碼可以正常執行即可，不要commit、不要push


## 專案管理工具: Jira (建立模板及待辦事項)

建立Software Development > Scrum模板
建立backlog/待辦事項，名稱為SCRUM build button_delete(你的學號)，類別為Story
將上述待辦事項拉入新的sprint，並點擊start sprint

## 專案管理工具: Jira (連結待辦事項與GitHub)

進到Board裡，將該待辦事項連結至特定GitHub repository中
須在Code頁籤完成Jira與GitHub連線的動作

(參考指令01，在VS code輸入) git checkout -b YourScrumIDandStory (請參考待辦事項設定中的Development > create new branch所提供的指令，形式應如上所示)<br><br>
(參考指令02，在VS code輸入) git commit -m "WTDL-8 <add a new delete button>" (請參考待辦事項設定中的Development > create new commit所提示的指令，形式應如上所示)<br><br>
(參考指令03，在VS code輸入) git push --set-upstream origin YourScrumIDandStory (或可直接輸入git push，其error message會提示要輸入什麼指令，形式應如上所示)<br>
<br>
前往GitHub，進到Midterm_你的學號之repository，完成branch的Merge
不要刪除任何Branch。即便Merge成功，也不要刪除Branch
(請截圖)連結成功後，畫面將顯示該待辦事項已連結至特定repository，如下圖1所示(紅框內容請務必呈現)。