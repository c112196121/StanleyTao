graph TD
    subgraph "時程計算 (單位: 天)"
        A[<b>1. 研擬計畫</b><br>ES:0, EF:1<br>LS:0, LF:1<br>D:1, S:0] --> B[<b>2. 任務分配</b><br>ES:1, EF:5<br>LS:1, LF:5<br>D:4, S:0]
        A --> C[<b>3. 取得硬體</b><br>ES:1, EF:18<br>LS:58, LF:75<br>D:17, S:57]
        B --> D[<b>4. 程式開發</b><br>ES:5, EF:75<br>LS:5, LF:75<br>D:70, S:0]
        C --> E[<b>5. 安裝硬體</b><br>ES:18, EF:28<br>LS:75, LF:85<br>D:10, S:57]
        D --> F[<b>6. 程式測試</b><br>ES:75, EF:105<br>LS:75, LF:105<br>D:30, S:0]
        E --> G[<b>7. 撰寫使用手冊</b><br>ES:28, EF:53<br>LS:85, LF:110<br>D:25, S:57]
        E --> H[<b>8. 轉換檔案</b><br>ES:28, EF:48<br>LS:90, LF:110<br>D:20, S:62]
        F --> I[<b>9. 系統測試</b><br>ES:105, EF:130<br>LS:105, LF:130<br>D:25, S:0]
        G --> J[<b>10. 使用者訓練</b><br>ES:53, EF:73<br>LS:110, LF:130<br>D:20, S:57]
        H --> J
        I --> K[<b>11. 使用者測試</b><br>ES:130, EF:155<br>LS:130, LF:155<br>D:25, S:0]
        J --> K
    end

    linkStyle 0 stroke:red,stroke-width:2px;
    linkStyle 2 stroke:red,stroke-width:2px;
    linkStyle 4 stroke:red,stroke-width:2px;
    linkStyle 7 stroke:red,stroke-width:2px;
    linkStyle 10 stroke:red,stroke-width:2px;

    style A fill:#ffcccc
    style B fill:#ffcccc
    style D fill:#ffcccc
    style F fill:#ffcccc
    style I fill:#ffcccc
    style K fill:#ffcccc
