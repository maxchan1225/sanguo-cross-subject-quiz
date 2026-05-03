# 三國跨學科測驗

Firebase Hosting + Firestore 單頁測驗網頁。

- 5 道三國選擇題
- 每題 ABCD 單選
- 填寫組別名稱
- 提交後寫入 Firestore `sanguo_quiz_submissions`
- Firestore rules 僅允許建立合法測驗提交，不開放前端讀取提交資料

部署：

```powershell
npx.cmd -y firebase-tools@latest deploy --only firestore:rules,hosting
```
