```markdown
# WorldModel2024Group28
松尾研世界モデル講義の最終課題用リポジトリ

最終課題は、Google Colab の Notebook で実装しています。

---

## 成果物
- **webAgent試作.ipynb**  
  WebAgentの実行環境  
- **miniwob.zip**  
  MiniWoBの環境  
- **frame_mark_elements2.js**  
  HTML加工用のライブラリ  

---

## セットアップ

### ① Gemini の API-KEY の準備
- Gemini 1.5 - Flash を使用するため、事前に `gemini-1.5-flash` の API_KEY を準備してください。

### ② 環境構築
- 以下のファイルをダウンロードし、zipファイルを解凍後、Colab 環境へアップロードしてください。
  - `miniwob.zip`
  - `frame_mark_elements2.js`

### ③ webAgent試作.ipynb への API と環境パスの設定
1. **API-KEY の登録**  
   - Colab の左端にある鍵アイコンから `GOOGLE_API_KEY` を設定してください。
   - 以下のようにコードを修正します:
     ```python
     genai.configure(api_key=userdata.get('GOOGLE_API_KEY'))
     ```

2. **環境パスの設定**  
   - 以下の部分を、アップロード先のパスに合わせて修正してください。
     ```python
     # miniwob の HTML を配置しているフォルダパス（例）
     miniwob_path = '/content/drive/MyDrive/miniwob/html/miniwob/'
     
     # JavaScript ファイルの配置パス（例）
     js_path = '/content/drive/MyDrive/miniwob/frame_mark_elements2.js'
     ```

### ④ タスクの設定
- **webAgent試作.ipynb** の一番下のセルにて、実行したいタスクを切り替えてください。
- 以下のように `task_name` に実行したいタスクを設定します。
  
  ![タスク設定例](https://github.com/user-attachments/assets/cba12621-05c2-46e8-acec-2f00926bde67)

---

## 実行
- Colab を上から順番にセルを実行することで、処理を行えます。
- 一度全てのセルを実行済であれば、**最終セルのタスクを書き換えることで別タスクを実行可能**です。

---

## 実験結果
![実験結果](https://github.com/user-attachments/assets/0777011a-c69f-4ed0-a72e-2d92c99bf882)
```
