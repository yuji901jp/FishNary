このフォルダには以下のファイルが自動作成されます。

１. FishNary-3_model_setting.json
   学習時に使った各関数、各層の次元数がJSON形式で保存される。
   学習後に判別を行う際には以下によって読み込み、利用可能。
   "model = model_from_json(open('./model-out/FishNary-3_model_setting.json', 'r').read())"
   また具体的にどのような関数、次元で学習したのかが記載されているため、後にチューニングを行う際に参照すると便利。

2. FishNary-3_model_weights.h5
   学習された結果、最終的なパラメーター（重み）セットがHDF形式で保存される。
   学習後に判別を行う際には以下によって読み込み、利用可能。
   "model.load_weights('./model-out/FishNary-3_model.h5')"
   
3. FishNary-3_model_flow.png
   学習時に使ったモデルのフローの画像ファイルがPNG形式で保存される。
   
