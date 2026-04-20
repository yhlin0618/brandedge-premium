# 快速使用指南 - Sandbox Test 專案

**最後更新**: 2025-10-16

---

## 🚀 新手快速上手（5 分鐘）

### 第一步：了解專案結構

```
sandbox_test/
├── 📁 app_*.R                    主應用程式（3個app）
├── 📁 modules/                   模組檔案
├── 📁 config/                    配置檔案
├── 📁 documents/                 專案規格文件
├── 📁 work_log/                  ⭐ 開發記錄和學習筆記
├── 📁 tests/                     測試檔案
└── 📁 archive/                   歷史備份
```

### 第二步：從這裡開始學習

**🎯 如果你想...**

#### 快速了解整個專案
👉 閱讀：`work_log/00_MASTER_LEARNING_GUIDE.md`
- 5 條學習路徑
- 完整導航系統
- 問題快速索引

#### 學習 Shiny 模組開發
👉 閱讀：`work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md`
- Reactive Closure Error 完整解析
- 防禦性編程模式
- 模組最佳實踐

#### 學習多語言國際化
👉 閱讀：`work_log/vitalsigns/dna_module/LECTURE_NOTES.md`
- UI vs Server 作用域問題
- 51 處硬編碼文字修正記錄
- AI 語言參數傳遞鏈

#### 解決具體問題
👉 查看：`work_log/quick_reference/`
- 快速修復指南
- 常見問題解答
- 故障排除步驟

#### 了解整理成果
👉 閱讀：`FINAL_ORGANIZATION_REPORT_2025-10-16.md`
- 完整統計數據
- Top 10 學習點
- 後續工作建議

---

## 📚 按角色推薦閱讀

### 👨‍💻 前端開發者

**核心必讀** (2-3 小時):
1. `work_log/vitalsigns/dna_module/LECTURE_NOTES.md`
   - 第 2 節：UI vs Server 作用域
   - 第 4 節：硬編碼問題
2. `work_log/apps/language_switching/`
   - 多語言切換機制

**進階閱讀** (3-4 小時):
1. `work_log/features/ui_ux/`
   - UI/UX 最佳實踐
2. `work_log/framework/config/`
   - 動態配置 UI

### 👨‍💼 後端開發者

**核心必讀** (2-3 小時):
1. `work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md`
   - Reactive 編程
   - 模組架構
2. `work_log/framework/config/`
   - 配置驅動開發

**進階閱讀** (3-4 小時):
1. `work_log/vitalsigns/revenue_pulse/`
   - 數據處理流程
2. `work_log/framework/audits/`
   - 程式碼審計

### 🏗️ 架構師 / Tech Lead

**核心必讀** (4-5 小時):
1. `work_log/00_MASTER_LEARNING_GUIDE.md`
   - 整體架構理解
2. `work_log/framework/`
   - 框架設計原則
3. `FINAL_ORGANIZATION_REPORT_2025-10-16.md`
   - 專案狀態與規劃

**進階閱讀** (5-6 小時):
1. 所有 LECTURE_NOTES.md
   - 深入理解各模組
2. `work_log/sessions/`
   - 開發決策歷程

### 🧪 QA 測試人員

**核心必讀** (1-2 小時):
1. `work_log/quick_reference/`
   - 已知問題和解決方案
2. `tests/` 目錄結構
   - 測試案例組織

**進階閱讀** (2-3 小時):
1. `work_log/vitalsigns/*/LECTURE_NOTES.md`
   - 常見錯誤模式
2. `work_log/framework/audits/`
   - 審計檢查清單

### 📝 技術文件撰寫者

**核心必讀** (2-3 小時):
1. `documents/instruction/`
   - 現有文件結構
2. `work_log/00_MASTER_LEARNING_GUIDE.md`
   - 導航系統設計

**進階閱讀** (3-4 小時):
1. 所有 LECTURE_NOTES.md
   - 學習筆記格式範例
2. `FINAL_ORGANIZATION_REPORT_2025-10-16.md`
   - 完整專案文檔

---

## 🎯 按問題類型查找

### ⚠️ 遇到錯誤時

#### 1. Reactive Closure Error
```
Error: could not find function 'xxx'
Error: object 'xxx' not found in module
```
👉 **解決方案**: `work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md` → 第 4.1 節

#### 2. 語言切換不生效
```
部分文字無法切換語言
UI 顯示硬編碼中文
```
👉 **解決方案**: `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` → 第 4 節

#### 3. get_lang_text() 在 UI 中報錯
```
Error: get_lang_text not found
```
👉 **解決方案**: `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` → 第 4.2 節

#### 4. AI 回應語言不正確
```
AI 始終用中文回應
```
👉 **解決方案**: `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` → 第 4.5 節

#### 5. 配置載入失敗
```
Error: YAML key not found
Error: Config file not loaded
```
👉 **解決方案**: `work_log/framework/config/` + `work_log/framework/audits/`

### 🔧 想要實作功能時

#### 1. 新增 Shiny 模組
👉 **參考**: `work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md` → 第 6 節

#### 2. 實作多語言支援
👉 **參考**: `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` → 第 5 節

#### 3. 整合 AI 功能
👉 **參考**:
- `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` → 第 4.5 節
- `work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md` → 第 3.4 節

#### 4. 建立配置驅動的模組
👉 **參考**: `work_log/framework/config/` → CONFIGURATION_DRIVEN_DEVELOPMENT_GUIDE.md

#### 5. 實作數據視覺化
👉 **參考**:
- `work_log/features/ui_ux/`
- `work_log/vitalsigns/revenue_pulse/`

---

## 📖 學習路徑推薦

### 🟢 新手路徑（第 1-2 週）

**Day 1-2: 理解專案結構**
- [ ] 閱讀 `work_log/00_MASTER_LEARNING_GUIDE.md`
- [ ] 瀏覽 `documents/instruction/` 了解系統架構
- [ ] 執行 `work_log/generate_stats.sh` 了解檔案分布

**Day 3-5: Shiny 基礎**
- [ ] 閱讀 `work_log/vitalsigns/acquisition_retention/LECTURE_NOTES.md`
- [ ] 實際執行 `app_vitalsigns.R`
- [ ] 嘗試修改簡單的 UI 元素

**Day 6-7: 多語言系統**
- [ ] 閱讀 `work_log/vitalsigns/dna_module/LECTURE_NOTES.md` 第 4 節
- [ ] 檢查 `config/yaml/` 的 YAML 結構
- [ ] 嘗試新增一個翻譯鍵值

**Day 8-10: 實作小功能**
- [ ] 從 `work_log/quick_reference/` 選擇一個快速任務
- [ ] 參考 LECTURE_NOTES.md 的最佳實踐
- [ ] 提交你的第一個 PR

### 🟡 中級路徑（第 3-4 週）

**Week 3: 深入模組開發**
- [ ] 完整閱讀兩個 LECTURE_NOTES.md
- [ ] 理解 Reactive 編程的 4 大規則
- [ ] 嘗試建立一個簡單的 Shiny 模組

**Week 4: 配置驅動開發**
- [ ] 閱讀 `work_log/framework/config/`
- [ ] 閱讀 `work_log/framework/audits/CONFIGURATION_DRIVEN_DEVELOPMENT_GUIDE.md`
- [ ] 將一個硬編碼模組改為配置驅動

### 🔴 高級路徑（第 5-8 週）

**Week 5-6: 完整模組開發**
- [ ] 開發一個新的完整模組
- [ ] 實作多語言支援
- [ ] 整合 AI 功能
- [ ] 撰寫測試案例

**Week 7-8: 架構優化**
- [ ] 審計現有程式碼
- [ ] 提出架構改進建議
- [ ] 撰寫技術文件
- [ ] 貢獻學習筆記

---

## 🛠️ 常用命令

### 查看統計資訊
```bash
cd /Users/hauhungyang/Library/CloudStorage/Dropbox/ai_martech/l3_premium/sandbox_test
./work_log/generate_stats.sh
```

### 搜尋特定內容
```bash
# 搜尋所有提到 "Reactive Closure" 的文件
grep -r "Reactive Closure" work_log/

# 搜尋特定錯誤解決方案
grep -r "get_lang_text" work_log/vitalsigns/
```

### 查看模組結構
```bash
# 列出所有 R 模組
ls -lh modules/module_*.R

# 檢查特定模組的行數
wc -l modules/module_vitalsigns_dna.R
```

### 快速導航
```bash
# 開啟主學習指南
open work_log/00_MASTER_LEARNING_GUIDE.md

# 開啟 DNA 模組學習筆記
open work_log/vitalsigns/dna_module/LECTURE_NOTES.md
```

---

## 📞 需要幫助？

### 🔍 找不到想要的資訊？

1. **使用搜尋**: 在 `work_log/00_MASTER_LEARNING_GUIDE.md` 中搜尋關鍵字
2. **查看索引**: 檢查各個 LECTURE_NOTES.md 的 "🔗 相關文件索引" 章節
3. **瀏覽目錄**: 根據問題類型選擇對應的子目錄

### 📝 想貢獻內容？

1. **更新學習筆記**: 在對應的 LECTURE_NOTES.md 中新增你的發現
2. **記錄新錯誤**: 在 "⚠️ 遇到的錯誤與問題" 章節新增
3. **分享解決方案**: 在 "✅ 解決方案與改進" 章節補充
4. **提煉最佳實踐**: 在 "💡 最佳實踐" 章節總結

### 🎯 想了解後續規劃？

查看 `FINAL_ORGANIZATION_REPORT_2025-10-16.md` 的 "🚀 後續建議工作" 章節

---

## ⚡ 快速參考卡片

### 核心概念速查

| 概念 | 文件位置 | 關鍵字 |
|------|---------|--------|
| Reactive Closure Error | acquisition_retention/LECTURE_NOTES.md | ns, session$ns |
| UI vs Server 作用域 | dna_module/LECTURE_NOTES.md | get_lang_text, get_text |
| 硬編碼 Fallback | dna_module/LECTURE_NOTES.md | fallback, YAML |
| AI 語言參數 | dna_module/LECTURE_NOTES.md | language, current_language |
| 配置驅動開發 | framework/config/ | YAML, config |

### 檔案命名規範

| 類型 | 命名格式 | 範例 |
|------|---------|------|
| 模組檔案 | `module_[app]_[name].R` | `module_vitalsigns_dna.R` |
| 配置檔案 | `[app]_[module].yaml` | `vitalsigns_dna.yaml` |
| 學習筆記 | `LECTURE_NOTES.md` | (固定名稱) |
| 完成報告 | `*_COMPLETE.md` | `DNA_FIX_COMPLETE.md` |

---

## 🎉 開始你的學習之旅！

**推薦起點**:
1. 📖 `work_log/00_MASTER_LEARNING_GUIDE.md` - 了解全局
2. 📚 選擇一個 LECTURE_NOTES.md - 深入學習
3. 🔧 `work_log/quick_reference/` - 實戰練習

**記住**:
- 💡 遇到問題先搜尋 work_log/
- 📝 學到新知識記得更新 LECTURE_NOTES.md
- 🤝 分享你的經驗幫助他人

---

**最後更新**: 2025-10-16
**維護者**: Development Team
**狀態**: ✅ 持續更新中
