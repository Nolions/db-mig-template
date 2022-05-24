# db-mig-template

資料料庫Schema管理Migrate Template

## Installation

```shell
compposer install` && cp `.env.example .env
```

### Usage

Create database kyogre on local first

```shell
// 撤銷所有 migration
make rollback

// 跑還沒跑過的 migration
make migrate

// 塞入預設的必要與測試資料
make seed

// 重設整個資料庫，等同於：rollback + migration + seed
make reset

// 建立migration文件
make create Class=<class_name>
```
