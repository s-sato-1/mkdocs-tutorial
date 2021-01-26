
## バージョン確認

```
$ python -V
Python 3.8.5
$ pip -V
pip 20.0.2 from /usr/lib/python3/dist-packages/pip (python 3.8)
```

## 仮想環境を作成・読込

```
$ python -m venv venv
$ . ./venv/bin/activate
$ source ./venv/bin/activate
```

## mkdocsをインストール

```
$ pip install mkdocs
$ mkdocs -V
mkdocs, version 1.1.2
```

## my-siteを作成

```
$ mkdocs new my-site
```

## buildする

+ mkdocs.ymlがカレントにあることを確認
+ siteが作成される

```
$ cd my-site
$ mkdocs build
```

## 簡易サーバを立ち上げる

+ mkdocs.ymlがカレントにあることを確認

```
$ mkdocs serve
```

## ディレクトリ構造

```
.
├── README.md
├── my-site
│   ├── docs // markdownを入れる
│   │   └──index.md
│   ├── mkdocs.yml // 設定を書き込む
│   └── site // 生成される静的ファイル
│       ├── 404.html
│       ├── css
│       ├── fonts
│       ├── img
│       ├── index.html
│       ├── js
│       ├── search
│       ├── sitemap.xml
│       └── sitemap.xml.gz
│
├── venv
```

