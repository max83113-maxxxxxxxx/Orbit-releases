# Orbit 下載

Orbit 是 Windows 11 x64 桌面資訊工具，提供日期時鐘、Codex 額度、Google 今日行程與 Gmail 新信提醒。

此版本庫只提供下載與版本說明；Orbit 原始碼維持私人。

目前公開測試版：**1.1.0**。

精簡小時鐘本體維持約 108×64，時間固定在上方。新增「設定 → 基本 → 精簡資訊輪播」：開啟後每 6 秒輪播日期、Codex 額度、今日行程與 Gmail 本機新信摘要；滑鼠或鍵盤焦點停留會暫停，點擊進入對應頁。輪播預設關閉，未連接或資料過期會明確標示，不補假數值；Gmail 數量不是整個信箱未讀總數。

鈴鐺與待處理數量移到小時鐘框外，不再擠壓內容。有提醒時整體視窗約 108×96，全部關閉後縮回。「設定 → 提醒」可選提醒在上方／下方，預設下方；新增「新提醒自動展開」，預設開啟，關閉後維持精簡，只更新框外提醒，鈴聲仍依獨立設定。不搶焦點、不改置頂、不叫出使用者已隱藏的視窗。

完整面板與精簡小時鐘各自記住位置，移動小時鐘不會覆寫大面板的位置。第一次收合靠原面板右下角，之後切換與重開各自回原位；各放到喜歡的位置一次便會自動保存。螢幕配置改變時仍會救回可操作範圍。

修正設定調整後捲回頂端：同一分頁保留捲動位置與焦點，快速連續調整也不會互相覆蓋。等待時間保留 10 秒、30 秒、1 分鐘、3 分鐘、5 分鐘，預設 5 分鐘；操作 Orbit、停留、設定、登入與前景查詢期間不收合。

使用者已授權本批直接發布，未另提供定位修正後逐項真人驗收結果。開發驗證：TypeScript 10 項、Rust 45 項（1 ignored）、桌面回歸 55 項與定位專項兩組通過；實際等待約 10.77 秒收合。隔離模擬不替代真實 Google、其他電腦、混合 DPI、睡眠喚醒或長時間驗收。

## 下載與開啟

[下載 Orbit 1.1.0 免安裝 ZIP](https://github.com/max83113-maxxxxxxxx/Orbit-releases/releases/download/v1.1.0/Orbit_1.1.0_windows-x64-portable.zip) · [版本說明與 SHA-256](https://github.com/max83113-maxxxxxxxx/Orbit-releases/releases/tag/v1.1.0)

下載 Releases 中名稱包含 `windows-x64-portable.zip` 的檔案，完整解壓縮至你有寫入權限的資料夾，開啟 `Orbit.exe`。請保留同一資料夾中的 `binaries` 與 `orbit-portable.json`。GitHub 自動顯示的 Source code 壓縮檔只包含下載說明，請使用版本附件中的 Orbit ZIP。

之後可在「設定 → 更新」檢查新版、下載，再按「更新並重新開啟」。下載不會直接套用；更新會驗證簽章與版本，保留本機設定與登入資料。

## 測試版使用條件

- Windows 11 x64，需具備 Microsoft Edge WebView2；不需要另外安裝 Node.js 或 Codex CLI。
- 時鐘可獨立使用。Codex 額度以自己的 ChatGPT 帳號在官方網頁登入，依方案與介面支援情況提供，不為查詢額度發出模型推論。
- Google 功能目前限已加入應用程式測試名單的帳號；尚未完成 Google 公開驗證。採官方登入與唯讀權限，不讀郵件內文、不寄信或修改郵件。
- 此測試版尚無 Windows Authenticode 發行者憑證。更新包的驗證簽章與 Windows 發行者簽章是不同項目；遇到系統提示時，請核對本站來源與版本提供的 SHA-256，無需關閉防毒。
- 請將程式放在可寫入的位置，保留更新與備份空間。更新時若斷電或磁碟損壞，必要時可重新下載完整 ZIP，或從程式資料夾內更新備份的 `previous` 回復。

操作說明：https://orbit.masaju.com/guide

官網：https://orbit.masaju.com/  
隱私權：https://orbit.masaju.com/privacy  
服務條款：https://orbit.masaju.com/terms

隨附 Codex 元件的授權與 NOTICE 位於 ZIP 的 `binaries`。安裝包不含維護者的個人登入、設定、郵件或行程。
