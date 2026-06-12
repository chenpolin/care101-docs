# Care101 Docs 開發指南與指令

本文件記錄了此文件的維護指引以及專案中定義的輔助工具（Skills）。

## 常用指令

### 執行 WordPress 文章同步與發布 (post-wp Skill)
將指定的 Markdown 文章同步至 WordPress 網站。此工具會自動進行：
1. 解析 Markdown 內容、提取標題並轉換為 HTML。
2. 根據檔名產生縮短且乾淨的 URL 別名 (Slug)。
3. 自動從 `blog-plan.md` 檢索該文章所屬的主題分類，並於 WordPress 後台建立/對應分類。
4. 尋找 `img` 資料夾內同名的圖片，若非 JPG 格式（如 PNG），將調用轉檔工具轉換為 JPG 後上傳為文章封面（精選圖片）。
5. 自動產生 AI 繪圖 Prompt 並更新至發布紀錄表格。

```bash
uv run C:\Users\定淵\.agents\skills\post-wp\scripts\post_wp.py <Markdown檔案路徑>
# 範例
uv run C:\Users\定淵\.agents\skills\post-wp\scripts\post_wp.py blog_posts/01-periodic-reservation.md
```

### 圖片轉 JPG 工具 (img-to-jpg Skill)
將 PNG, WEBP 等格式的圖片轉換為符合 WordPress 標準的 JPG 格式。
```bash
uv run C:\Users\定淵\.agents\skills\post-wp\scripts\img_to_jpg.py <圖片路徑>
# 範例
uv run C:\Users\定淵\.agents\skills\post-wp\scripts\img_to_jpg.py blog_posts/img/01-periodic-reservation.png
```

## 專案結構
* [wordpress-publish-report.md](file:///c:/app/care101-docs/wordpress-publish-report.md) - 自動更新的文章發布狀態與 AI 配圖 Prompt 表格。
