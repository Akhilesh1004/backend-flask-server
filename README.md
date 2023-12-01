# backend-flask-server

## Architecture

```
.
├── config.py
├── config.py.sample
├── controllers
│   ├── auth.py
│   ├── ddns.py
│   ├── domains.py
│   ├── glue.py
│   └── __init__.py
├── launch_thread.py
├── main.py
├── models
│   ├── db.py
│   ├── ddns.py
│   ├── domains.py
│   ├── elastic.py
│   ├── glues.py
│   ├── __init__.py
│   ├── records.py
│   └── users.py
├── README.md
├── services
│   ├── auth_service.py
│   ├── dns_service.py
│   ├── __init__.py
│   └── nctu_oauth
│       ├── __init__.py
│       ├── oauth.py
│       └── README.md
└── tests
    ├── __init__.py
    ├── test_attacker.py
    ├── test_common.py
    ├── test_controllers.py
    ├── test_ddns.py
    ├── test_domain_expired.py
    ├── test_domain_register.py
    └── test_issue_token.py
```

### config.py 和 config.py.sample:
config.py 包含應用程序的配置信息，如資料庫連接設置、API金鑰等。
config.py.sample 是 config.py 的範本，用來展示配置文件的格式和示例值。

### controllers:
這個目錄包含了應用程序的控制器或路由層，用於處理HTTP請求和路由它們到適當的功能模組。

### launch_thread.py:
這個文件包含一個用於啟動回收 domain 的 process。

### main.py:
這個文件是應用程序的入口點，它可能包含主要的程式邏輯，如應用程序的初始化和啟動。

### models:
這個目錄包含應用程序的模型層，用於定義資料模型、資料庫表結構以及與資料庫的互動。

### services:
這個目錄包含應用程序的服務層，用於實現不同的業務邏輯，如身份驗證服務、DNS服務等。

### tests:
這個目錄包含測試用例，用於測試應用程序的各個部分，確保它們按照預期工作。
