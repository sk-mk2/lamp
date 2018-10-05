# 元となるイメージ
FROM python:latest
# そのまま
WORKDIR /app
# arg1: コピー元 arg2: コピー先 
COPY . /app
# コマンド
RUN pip install --trusted-host pypi.python.org -r requirements.txt
# このコンテナーが開放するポート？
EXPOSE 80
# 環境変数
ENV NAME World
# コンテナーが立ち上がったらコマンドを実行
CMD ["python", "app.py"]
