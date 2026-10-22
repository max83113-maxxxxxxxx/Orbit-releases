# Orbit 下載

Orbit 是 Windows 11 x64 桌面資訊工具，提供日期時鐘、Codex 額度、Google 今日行程與 Gmail 新信提醒。

此版本庫只提供下載與版本說明；Orbit 原始碼維持私人。

## 下載與開啟

[下載 Orbit 1.0.0-rc.3 免安裝 ZIP](https://github.com/max83113-maxxxxxxxx/Orbit-releases/releases/download/v1.0.0-rc.3/Orbit_1.0.0-rc.3_windows-x64-portable.zip) · [版本說明與 SHA-256](https://github.com/max83113-maxxxxxxxx/Orbit-releases/releases/tag/v1.0.0-rc.3)

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
