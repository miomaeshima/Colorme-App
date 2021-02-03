# Colorme
<body style="background:linear-gradient(#fcfcfc, #95cdf5)">

####  _このアプリケーションはコードクリサリス在学中に作成されました。_  <br><br>

「この色はなんという名前だったろう。  
赤とか、青とか、ではなく、もっと細やかな名前があったはず。」　　

色の名前は単なる記号ではなく、それ自体、繊細で色彩にあふれています。
わずかな違いを表す名前を、もう一度味わうためにこのアプリを作りました。  

ふと、この写真の色はなんというのだろう、と思ったとき、懐かしい響きの名前が調べられます。  

---
## ローカルでのインストール

### バックエンド  
pythonがインストールされている前提で、[バックエンドレポジトリ](https://github.com/miomaeshima/Colorme-backend)をクローンしたのち、コマンドラインで以下のように入力。
```
$ pip install flask flask_cors openpyxl
$ virtualenv 
$ env\Scrips\activate 
$ python app.py
```

### フロントエンド
[フロントエンドレポジトリ](https://github.com/miomaeshima/Colorme-frontend)をクローンしたら、コマンドラインで以下の通り入力。
```
$ npm install または　yarn 
$ npm http-server または yarn http-server
```
http://localhost:8080を開いてください。  

___

## 使い方　　
今はイメージファイルにある画像のみが対象です。  

アプリには712色を含む日本の伝統色パレットが入っおり、それぞれの色にはRGB値と伝統的色名が含まれています。  

<p align="center"><img src="./img/cherry.png" width="100%"></p>

例えば上の画像をクリックすると、この画像中、一番使われている色がパレットから探され、同じ色か、まったく同じRGB値の色がない場合はその色に一番近い色が求められて、その伝統的名称が、色彩とともに表示されます。

<p align="center"><img src="./img/cherry-name.png" width="100%"></p>

色の近さはRGBを3次元の座標ととらえ、写真のメインカラーとパレット中の色の距離を見て、この距離が一番近い色を表示します。


<p align="center"><img src="./img/rgb3d.png" width="300px"></p>


写真のメインカラーをaとしたとき、色cより、色bのほうが近い。

___
## テクノロジー

フロントエンド　HTML, CSS, HTML, CSS, JavaScript, [color-thief](https://github.com/lokesh/color-thief)   
バックエンド　Python
___
## 今後の機能拡張

1．デモページの作成。  
2．デバイス内の画像ファイルを選択できるようにする。  
3．画像をアップロードして色名を調べられるにする。  
4．英語の色名パレットにも切り替えられるようにする。
 
</body>



