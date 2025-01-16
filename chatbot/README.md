### 実行するための準備

#### 1. 必要なライブラリをインストール

```
pip install streamlit beautifulsoup4 python-dotenv langchain_google_genai langchain 
```

#### 2. Gemini API Keyを発行

[https://aistudio.google.com/app/apikey?hl=ja](https://aistudio.google.com/app/apikey?hl=ja)

#### 3. Google API Keyの発行, Custom Search APIの有効化, Custom Search Engine（CSE）の取得

[https://qiita.com/zak_y/items/42ca0f1ea14f7046108c](https://qiita.com/zak_y/items/42ca0f1ea14f7046108c) を参照

#### 4. 環境変数の設定

.envファイルを作成し、発行したGemini API Keyを以下のように追記

```
GEMINI_API_KEY = 'あなたのGEMINI_API_KEY'
GOOGLE_API_KEY = 'あなたのGOOGLE_API_KEY'
CUSTOM_SEARCH_ENGINE_ID = 'あなたの検索エンジンID'
```

### 実行

```
streamlit run app.py
```