# tcc-git-django-sample
這是給 Taipei Creative Coders Meetup #8 的一個範例 repository。在這邊簡易的示範了 commit log 以及 README 的整合。

## 環境建置
如果你真的想要跑這個範例的話，它僅僅是一個 Django 全空的 demo site。請先安裝 Pipenv。

### 安裝相依性套件

使用 pipenv 安裝相依性套件

```
$ pipenv install
```


### 產生 SECRET_KEY 與設定檔案

請至 https://djecrety.ir/ 產生一個 SECRET_KEY，並且將它複製下來。

接著請複製設定檔案的樣板 [django/tcc/local.env.sample](django/tcc/local.env.sample) 到真正的設定檔位置 `django/tcc/local.env`

```
$ cp django/tcc/local.env.sample django/tcc/local.env
```

編輯 `local.env` 並將剛剛複製下來的 SECRET_KEY 貼在檔案內 `SECRET_KEY=` 等號的後面


### 執行

接著就可以執行了

```
$ pipenv run ./manage.py runserver
```
