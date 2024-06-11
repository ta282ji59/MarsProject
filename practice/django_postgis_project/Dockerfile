# Python 3ベース
FROM python:3

# 環境変数を設定する
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# ワークディレクトリを設定
WORKDIR /code

# プロジェクトの依存パッケージをインストールする
COPY requirements.txt /code/
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# プロジェクトファイルをコピーする
COPY . /code/
