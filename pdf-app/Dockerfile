# ベースイメージを指定
FROM node:16

# 作業ディレクトリを作成
WORKDIR /app

# パッケージファイルをコピー
COPY package.json ./
COPY package-lock.json ./

# 依存関係をインストール
RUN npm install

# ソースコードをコピー
COPY . .

# 開発サーバーを起動
CMD ["npm", "start"]