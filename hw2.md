## 1.PERT/CPM 圖

![PERT/CPM 圖](PERT.png "PERT/CPM 圖")

---
## 2.甘特圖

```mermaid
gantt
    title 工作分解結構清單
    dateFormat  YYYY-MM-DD
    section 項目與說明
    研擬計畫         :a1, 2025-09-30, 1d
    任務分配         :a2, after a1, 4d
    取得硬體         :a3, after a1, 17d
    程式開發         :a4, after a2, 70d
    安裝硬體         :a5, after a3, 10d
    程式測試         :a6, after a4, 30d
    撰寫使用手冊     :a7, after a5, 25d
    轉換檔案         :a8, after a5, 20d
    系統測試         :a9, after a6, 25d
    使用者訓練       :a10, after a7 a8, 20d
    使用者測試       :a11, after a9 a10, 25d
```

---
## 3.關鍵路徑

![PERT/CPM 圖](PERT.png "PERT/CPM 圖")
> 「紅色方框」 → 關鍵路徑  

- 關鍵路徑： 研擬計畫 → 任務分配 → 程式開發 → 程式測試 → 系統測試 → 使用者測試

- 各段工期：1d + 4d + 70d + 30d + 25d + 25d

- 總工期：155 天
