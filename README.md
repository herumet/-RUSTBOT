# -RUSTBOT
### 導入手順

1. **必要なソフトウェアのインストール**:
   - Rust をインストール: [Rust公式サイト](https://www.rust-lang.org/) を参照。
   - ChromeDriver をインストール: [ChromeDriver公式サイト](https://chromedriver.chromium.org/downloads) からダウンロードし、実行可能なパスに配置。

3. **Selenium WebDriver のセットアップ**:
   Selenium Server を実行する。以下をインストールして実行。

   ```bash
   java -jar selenium-server-standalone.jar
   ```

4. **コードの実行**:
   ターミナルで以下を実行。

   ```bash
   cargo run
   ```

5. **実行中の挙動**:
   - ログインページにアクセスし、SBI証券にログイン。
   - 指定した銘柄の在庫状況を監視。
   - 在庫が検知された場合、取引を実行。

6. **トラブルシューティング**:
   - WebDriverの起動に失敗する場合は、ChromeDriverとブラウザのバージョンが一致していることを確認。
   - ログイン失敗時には `.env` ファイルの内容が正しいか確認。

この手順でコードを運用できるはずです。
