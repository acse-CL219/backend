### 學生綜合素質可視化分析 後端代碼

## 項目配置安裝

### 前提:
- mysql數據庫
- 安裝Python3
- 安裝pip

下面命令在工程根目錄執行

### 1. 創建虛擬環境
使用PyCharm 或者 VSCode 等IDE ，就將工程的虛擬環境切換為剛才創建的虛擬環境(在工程根目錄下)

### 2. pip安裝依賴所需依賴

- 在終端裡進入虛擬環境

```
windows 環境
venv\Scripts\activate
Linux 環境
[root@zhsz zhsz_flask]# source venv/bin/activate
```

- 使用pip安裝依賴庫
```
pip install -r requirements.txt

```

## 初始化

### 1.配置數據庫
修改`settings.py`文件
設置 MySQL 的 地址 和 用戶名密碼

### 初始化數據庫

第一次運行執行下面命令創建對應的表

```
python manage.py db init
python manage.py db migrate
python manage.py db upgrade
```



## 啟動項目

使用命令
`python3 manage.py server`


### 修改維護

- 生成requirements.txt

`pip freeze > requirements.txt`
