# node-weather-website2
* Node.jsによる簡単な天気予報Webサイト
* Dark Sky API のサポートは 2023 年 3 月 31 日に終了したので、現在動きません。
* 以下はHerokuにデプロイしたときのものですが、現在はrender.comにデプロイしています。
![天気予報](https://user-images.githubusercontent.com/47315420/93012424-44416200-f5db-11ea-992b-49cf9e40a948.gif)

# Features
Node.js 及び下記パッケージ/モジュールを使用しています。
* [env-cmd](https://www.npmjs.com/package/env-cmd)
* [Express](http://expressjs.com/)
* [hbs](https://www.npmjs.com/package/hbs)
* [request](https://www.npmjs.com/package/request)
 
# Requirement
以下のAPIアカウントを取得する必要があります。
* [Dark Sky API](https://darksky.net/dev)
* [mapbox](https://www.mapbox.com/)
 
# Installation
ローカルで実行する場合は、.envファイルを作成し、以下を記述してください。
```
PORT=3000
DARKSKY_NET_API_KEY=https://api.darksky.net/forecast/********************************/
MAPBOX_ACCESS_TOKEN=pk.*******************************************************************.**********************
MAPBOX_GEOCODING_URL=https://api.mapbox.com/geocoding/v5/mapbox.places/
```

# Usage
テキストボックスに「横浜市」などと入力して[検索]ボタンをクリックしてください。
 
# Note
render.comでの設定は次のようにしました。別途、Environment Variablesも設定する必要があります。

```
Branch: main
Root Directory: ./
Build Command: $ npm install
Start Comand: $ node src/app.js
```
 
# Author
pitang1965
 
* 作成者
pitang1965

* Website
https://software.pitang1965.com/
 
# License
"node-weather-website" is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
