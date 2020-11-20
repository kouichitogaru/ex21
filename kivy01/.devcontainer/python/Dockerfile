FROM python:3.7-slim

#作業ディレクトリを変更
WORKDIR /tmp/mydir

#ファイルのコピー
COPY requirements.txt ${PWD}

#pythonパッケージをインストール
RUN pip install -r requirements.txt