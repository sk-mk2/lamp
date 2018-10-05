# 元となるイメージ
FROM nginx:latest
# そのまま
# 別にどうでもいい
WORKDIR /app
# arg1: コピー元 arg2: コピー先 
COPY ./www /usr/share/nginx/html
# コマンドpythonのだからいらない
# RUN pip install --trusted-host pypi.python.org -r requirements.txt
# このコンテナーが開放するポート
EXPOSE 80
# 環境変数
# ENV NAME World
# コンテナーが立ち上がったらコマンドを実行
# CMD ["python", "app.py"]

#コンテナ内と外部のディレクトリを使えるようにする?
#あんままだわかってない
#VOLUME
