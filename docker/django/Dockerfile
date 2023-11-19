#FROM registry.access.redhat.com/ubi8/python-39

#ADD ./app . 
#RUN pip install -r requirements.txt

#ENTRYPOINT /bin/bash docker-entrypoint.sh

# ベースイメージの設定
FROM registry.access.redhat.com/ubi8/python-39

# アプリケーションファイルをコンテナに追加
ADD ./app .

# root権限を必要としないコマンドの実行
# 例：Pythonパッケージのインストール
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# エントリーポイントの設定
ENTRYPOINT /bin/bash docker-entrypoint.sh

