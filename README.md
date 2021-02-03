# Colorme

## How to install

backend
git clone  

pip install flask flask_cors openpyxl
python app.py

virtualenv 
env\Scrips\activate 

frontend
git clone
npm install または　yarn 
npm http-server または yarn http-server
http://localhost:8080
を開いてください。

## How to use
今はimg fileにある画像のみが対象です。
アプリには712色を含む日本の伝統色パレットが入っています。
パレットはRGB値と伝統的な名前が含まれています。

画像をクリックするとその画像で一番使われている色とその名前が表示されます。
まったく同じRGB値の色がない場合はその色に一番近い色を計算します。
近さはRGBを3次元ととらえ、写真のメインカラーとパレット中の各色のRGB値の差をそれぞれ二乗したものの合計の平方根に基づいています。





