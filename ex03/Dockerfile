FROM ubuntu:20.04

# Nginx の インストール 
RUN apt-get update && apt-get install -y \ 
    nginx \ 
    tzdata \ 
&& rm -rf /var/lib/apt/lists/* 

# タイム ゾーン を 設定 する 環境変数 
ENV TZ=Asia/Tokyo 

# ポート の 指定 
EXPOSE 80

## ファイル の コピー 
COPY src/index.html /var/www/html/ 

# Nginx の 起動 
CMD ["nginx", "-g", "daemon off;"]