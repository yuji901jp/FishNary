# FishNary
Fish Dictionary based on Deep Learning  
魚の画像ファイルを読み込むことで魚種を判定する。内部にはTensorFlow/Kerasを中心に使っている。  

使い方
-------------
0. Anaconda Navigatorを起動し、関連モジュールをインストール  
  
1. trainフォルダへ学習用画像ファイルを配置。  
   フォルダ毎にラベルが付与されるので魚種毎にフォルダを配置すること。  
   現在は3魚種(ブリ、ヒラマサ、マダイ)に対応済み。  
  
2. FishNary-3.ipynbをjupyter notebookで開き、順次実行。  
   実行結果はmodel-outフォルダへ出力される。  
   logs_FishNary-3にはTensorBoard表示用のファイルが出力されるため、  
   以下コマンドによってTensorBoardにて学習結果を確認できる。  
   
   >tensorboard --logdir=logs_FishNary-3  
  
3. imagesフォルダに判別したい画像ファイルを配置する。  
   画像の解像度は指定なし。ただし形式はJPEGとすること。

4. FishNary-checker.ipynbをjupyter notebookで開き、  
   img_pathに手順3で配置した画像ファイルへのパスを指定後、順次実行。

5. FishNary-checker.ipynbの中で判別結果が表示される。  

注意点
-------------
勉強用ファイルのためJupyter Notebook環境での動作を前提としている。  
なお、MacOS(Sierra)、Anaconda Navigator(1.9.6)にて開発を実施している。  

関連モジュールのバージョン情報
-------------
Anaconda Navigator = 1.9.6  
Python = 3.6.7  
Keras  = 2.1.2-tf (backend: tensorflow1.5.0)  
Numpy  = 1.14.2
