# C# + OpenCVSharp 画像処理アプリ開発計画

## 目的
OpenCVSharp を使った画像処理アプリを C# + Windows Forms/WPF でまず1本開発し、その後 Electron を用いたクロスプラットフォーム化を目指します。

---

## ステップ1：C# + OpenCVSharp によるプロトタイプ

### 1. NuGetパッケージ導入
- [ ] OpenCvSharp4.Windows をプロジェクトに追加
- [ ] OpenCvSharp4.runtime.win を併用

### 2. 最初のアプリ作成
- [ ] ファイル選択 → 画像読込 → グレースケール変換 → 保存
- [ ] GUIはWindows FormsまたはWPFを使用
- [ ] 実行確認と例外処理の検証

### 3. テスト
- [ ] ユニットテスト (xUnit or NUnit)
- [ ] 処理結果の画像比較テスト（差分検出）

---

## ステップ2：Electronとの統合

### 4. フロントエンドをElectronで作成
- [ ] Node.js + Electronプロジェクトの準備
- [ ] C#との通信方法の選定（例：WebSocket, Named Pipe, gRPC）

### 5. C#のバックエンドをラップ
- [ ] C#の画像処理をCLI化またはサービス化
- [ ] Electronから実行・結果取得

### 6. サンプルアプリの完成
- [ ] UIで画像選択 → C#で処理 → UIに結果表示
- [ ] macOS互換性の確認（.NET Core使用）

---

## ステップ3：本格展開に向けた構想（将来計画）

- [ ] モジュール分割（UI/処理/データ層）
- [ ] GitHubで公開・共有
- [ ] ユーザー設定や履歴保存機能の追加
