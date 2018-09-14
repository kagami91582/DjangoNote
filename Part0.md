# Part0 在那之前先準備好環境

## 安裝 Python



值得注意的是，Django每個版本都有相對應的Python版本，看來是越新越好了(X)。

|Django Ver.|Python 2.x|Python 3.x|
|:---:|:---:|:---:|
|1.8|2.7|3.2 / 3.3 / 3.4 / 3.5|
|1.9|2.7|3.4 / 3.5|
|1.10|2.7|3.4 / 3.5|
|1.11|2.7|3.4 / 3.5 / 3.6|
|2.0||3.4 / 3.5 / 3.6|
|2.1||3.5 / 3.6 / 3.7|

## 安裝 virtualenv

主要常見有兩種

1. 安裝現有虛擬環境套件，例如anaconda
2. 手動安裝Virtualenv

當然是純手工打造最純了(?)，啟動你的終端機，在裡面輸入

```
@Windows cmd
C:\Python3_\python.exe -m venv venv名稱
```
```
@Linux/mac
python -m venv venv名稱
```

那假如要進去的話就
```
@Windows cmd
C:\Users\....\proj位置 > venv名稱\Scripts\activate
```
```
@Linux/mac
source venv名稱\bin\activate
```

只要看到下面長這個樣子就對了

```
(venv名稱) ~/
(venv名稱) C:\Users\....\ >
```

要退出虛擬環境就可以使用`deactivate`退出。

那麼進去之後的程式碼就沒有差別了。

## 安裝Django

```
pip install django
pip install django==指定的版本
```

## 創建project

```
django-admin startproject project名稱
```

## 新增app

```
python manage.py startapp app名稱
```

## 有沒有程式可以一次打包做好

旁邊有個懶癌患者，直接推薦服用PyCharm，一個add按下去，選擇Django就能venv、project、app通通傳扁邊。
![](img/001.png)
