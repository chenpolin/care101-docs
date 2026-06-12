---
description: 注意：此功能尚未完全開放。等待Google認證中，預期2025-12-30啟用。
---

# C1-3 Google Calendar 同步

{% embed url="https://youtu.be/wsuPa_knOLc" %}

<mark style="color:red;">**注意：此功能尚未完全開放。等待Google認證中，預期2025-12-30啟用。**</mark>

#### Google Calendar 同步功能說明

**什麼是 Google Calendar 同步？**

* 系統會自動將預約同步到治療師的 Google Calendar
* 治療師可以在 Google Calendar 中查看和管理預約
* 支援單向同步（系統 → Google Calendar）

**為什麼要使用？**

* ✅ 方便治療師在 Google Calendar 中查看預約
* ✅ 可以與其他行事曆整合
* ✅ 支援手機 Google Calendar App 查看

***

#### 設定 Google Calendar 連線

**使用情境**：

* 治療師想要將預約同步到自己的 Google Calendar
* 僅適用於 治療師帳號 。

**操作步驟（治療師）**：

1. **登入系統**
   * 使用治療師帳號登入
2. **進入「我的設定」頁面**
   * 左側選單 → 「我的設定」
3. **連線 Google Calendar**&#x20;
   * 找到「Google Calendar 連線」區塊
   * 點擊「連線 Google Calendar」或「授權」按鈕
   * 系統會跳轉到 Google 授權頁面
4. **授權系統存取**
   * 使用 Google 帳號登入
   * 確認授權系統存取您的 Google Calendar
   * 點擊「允許」或「同意」
5. **完成連線**
   * 系統會自動返回
   * 顯示「已連線」狀態

**注意事項**：

* 需要有效的 Google 帳號
* 需要授權系統存取 Google Calendar
* 連線後，新的預約會自動同步到 Google Calendar

***

#### 確認預約是否已同步

**使用情境**：

* 想確認預約是否已成功同步到 Google Calendar

**操作步驟**：

1. **開啟 Google Calendar**
   * 在瀏覽器中開啟 [Google Calendar](https://calendar.google.com)
   * 或開啟手機的 Google Calendar App
2. **查看預約**
   * 預約會顯示在 Google Calendar 中
   * 預約標題會顯示個案名稱
   * 預約時間會正確顯示
3. **檢查同步狀態**
   * 如果預約沒有出現，可能是：
     * Google Calendar 連線未完成
     * 同步尚未完成（可能需要幾分鐘）
     * 同步失敗（查看系統日誌）

***

#### 處理同步失敗的情況

**使用情境**：

* 預約建立成功，但 Google Calendar 沒有顯示
* 同步狀態顯示失敗

**可能原因**：

* Google Calendar 連線已中斷
* Google 授權已過期
* 網路連線問題
* 系統同步服務異常

**處理方式**：

1. **檢查 Google Calendar 連線狀態**
   * 進入「我的設定」頁面
   * 查看「Google Calendar 連線」狀態
   * 如果顯示「未連線」，重新連線
2. **重新連線 Google Calendar**
   * 點擊「重新連線」或「授權」按鈕
   * 重新完成授權流程
3. **檢查預約時間**
   * 確認預約是否在最近建立
   * 同步可能需要幾分鐘時間
4. **聯繫系統管理員**
   * 如果問題持續，聯繫系統管理員
   * 提供預約 ID 和時間，方便排查

***

#### 取消 Google Calendar 連線

**使用情境**：

* 不再需要同步到 Google Calendar
* 想要更換 Google 帳號

**操作步驟**：

1. **進入「我的設定」頁面**
   * 左側選單 → 「我的設定」
2. **取消連線**
   * 找到「Google Calendar 連線」區塊
   * 點擊「取消連線」或「移除授權」按鈕
   * 確認取消連線
3. **完成取消**
   * 系統會移除 Google Calendar 連線
   * 之後的預約不會再同步到 Google Calendar
   * 已同步的預約不會自動刪除（需手動在 Google Calendar 中刪除）
