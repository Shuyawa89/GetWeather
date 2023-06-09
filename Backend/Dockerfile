# Python 3.9のベースイメージを使用
FROM python:3.9

# /appを作業ディレクトリに設定
WORKDIR /app

# requirements.txtをコンテナにコピー
COPY requirements.txt requirements.txt

# 必要なPythonパッケージをインストール
RUN pip install -r requirements.txt

# 残りのファイルをコンテナにコピー
COPY . .

# コンテナが起動したときにFastAPIアプリケーションを起動
#CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]