# WorldModel2024Group28
松尾研世界モデル講義の最終課題用リポジトリ

最終課題は、google colab のnotebookで実装しています。

# 成果物
・webAgent試作.ipynb　　・・・WebAgentの実行環境
・miniwob.zip　　・・・miniwobの環境
・frame_mark_elements2.js 　・・・HTML加工用のライブラリ

# セットアップ

①geminiのAPI-KEYの準備
　gemini 1.5 -flash を使用するため、事前にgemini-1.5-flashのAPI_KEYを準備

②環境構築
　下記ファイルをダウンロードし zipファイルは解凍し、colab環境へアップロード
　・miniwob.zip
　・frame_mark_elements2.js

③webAgent試作.ipynbへの上記、API,環境PATHの設定
　１.　webAgent試作.ipynbに　API　－KEYの登録　※colabの左端の鍵アイコンでGOOGLE_API_KEYを設定
 　　genai.configure(api_key=userdata.get('GOOGLE_API_KEY'))

  ２．環境パスの設定
  　以下の部分を、アップロード先のパスに合わせて定義を修正してください.
   
   #miniwobのhtmlを配置しているフォルダパス（例）
　　miniwob_path = '/content/drive/MyDrive/miniwob/html/miniwob/'
  
   #javascriptファイルの配置パス（例）
　  js_path='/content/drive/MyDrive/miniwob/frame_mark_elements2.js'

④タスクの設定
webAgent試作.ipynbの一番下のセルにて、実行したいタスクの切り替え
task_nameに実行したいタスクを設定する。

![image](https://github.com/user-attachments/assets/cba12621-05c2-46e8-acec-2f00926bde67)

 # 実行
 colabを上から順次実行することで、処理が行える。
 １度でも全セルを実行済であれば、、最終セルのタスクを書き換えて別のタスクを実行することが可能。

# 実験結果
![image](https://github.com/user-attachments/assets/0777011a-c69f-4ed0-a72e-2d92c99bf882)
