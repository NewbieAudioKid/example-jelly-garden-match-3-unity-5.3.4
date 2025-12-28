# 🍬 Jelly Garden マッチ3ゲーム

<div align="center">

**言語 / Language:** [English](README.md) | [中文](README_zh.md) | [日本語](README_ja.md)

![Unity](https://img.shields.io/badge/Unity-2019.4+-black?style=flat-square&logo=unity)
![C#](https://img.shields.io/badge/C%23-8.0-blue?style=flat-square&logo=c-sharp)
![License](https://img.shields.io/badge/License-Proprietary-red?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20Android-lightgrey?style=flat-square)

モダンな機能、ソーシャル統合、収益化機能を備えた完全なマッチ3パズルゲームテンプレート。

[機能](#-機能) • [はじめに](#-はじめに) • [プロジェクト構造](#-プロジェクト構造) • [ドキュメント](#-ドキュメント) • [サポート](#-サポート)

</div>

---

## 📋 目次

- [概要](#-概要)
- [機能](#-機能)
- [はじめに](#-はじめに)
- [プロジェクト構造](#-プロジェクト構造)
- [コアシステム](#-コアシステム)
- [統合とサービス](#-統合とサービス)
- [ドキュメント](#-ドキュメント)
- [システム要件](#-システム要件)
- [ビルドとデプロイ](#-ビルドとデプロイ)
- [貢献](#-貢献)
- [サポート](#-サポート)
- [ライセンス](#-ライセンス)

---

## 🎮 概要

**Jelly Garden マッチ3**は、モバイルプラットフォーム向けに設計された機能豊富なUnityパズルゲームテンプレートです。スケーラビリティとカスタマイズ性を重視して構築され、レベルデザインツールから収益化システムまで、商用マッチ3ゲームのローンチに必要なすべてを含んでいます。

### 主要なハイライト

- 🎯 **完全なマッチ3メカニクス**：特殊アイテムとブースターを備えたクラシックなスワップ＆マッチゲームプレイ
- 🗺️ **スマートレベルシステム**：100以上のプリビルトレベルを持つ高度なレベルエディター
- 💰 **収益化対応**：アプリ内課金、広告統合、仮想通貨システム
- 🌐 **ソーシャル機能**：Facebook統合、リーダーボード、フレンドシステム
- 📱 **クロスプラットフォーム**：最適化されたパフォーマンスでiOSとAndroidをサポート
- 🎨 **洗練されたUI/UX**：美しいアニメーション、パーティクルエフェクト、レスポンシブデザイン

---

## ✨ 機能

### コアゲームプレイ

- **マッチ3メカニクス**

  - クラシックなスワップ＆マッチゲームプレイ
  - 特殊アイテム：ボム、横/縦ストライプ、レインボーアイテム
  - ビジュアルエフェクト付きコンボシステム
  - 複数のゲームモードと目標

- **レベルシステム**

  - 100以上のユニークなプリデザインレベル
  - 段階的な難易度カーブ
  - 星評価システム（1-3星）
  - 複数のレベル目標（スコア、食材、ブロックなど）

- **ブースターとパワーアップ**
  - プレイ前ブースター
  - ゲーム内ブースター
  - デイリー報酬システム
  - 自動回復付きライフシステム

### 技術的機能

- **レベルエディター**

  - ビジュアルレベルデザイナー
  - ドラッグ＆ドロップインターフェース
  - リアルタイムプレビュー
  - インポート/エクスポート機能

- **スマートマップシステム**

  - スクロール可能なレベルマップ
  - アンロック進行
  - ビジュアルレベルステータス表示
  - エピソードシステム

- **アニメーションシステム**
  - スムーズなアイテム遷移
  - マッチのパーティクルエフェクト
  - 画面シェイクエフェクト
  - 報酬アニメーション

### 収益化

- **アプリ内課金**

  - コインパッケージ
  - ブースターバンドル
  - ライフ購入
  - 広告削除オプション

- **広告統合**

  - リワード動画広告
  - インタースティシャル広告
  - バナー広告
  - 広告イベントシステム

- **仮想経済**
  - ソフト通貨（コイン）
  - 購入追跡
  - 報酬配布

### ソーシャルとネットワーク

- **Facebook統合**

  - ログインシステム
  - フレンドリスト
  - アバター読み込み
  - スコア共有

- **リーダーボード**

  - グローバルランキング
  - フレンドランキング
  - オフラインサポート
  - スコア同期

- **クラウドサービス**
  - GameSparks統合
  - PlayFab統合
  - データ永続化
  - クロスデバイス同期

---

## 🚀 はじめに

### 前提条件

- **Unity**：2019.4 LTS以上（2020.3+推奨）
- **オペレーティングシステム**：Windows 10/11またはmacOS 10.14+
- **IDE**：Visual Studio 2019+またはJetBrains Rider
- **モバイルSDK**：
  - Android：SDK API Level 19+
  - iOS：Xcode 12+

### インストール

1. **リポジトリをクローン**

   ```bash
   git clone https://github.com/NewbieAudioKid/example-jelly-garden-match-3-unity-5.3.4.git
   cd example-jelly-garden-match-3-unity-5.3.4
   ```

2. **Unityで開く**

   - Unity Hubを起動
   - 「追加」をクリックしてプロジェクトフォルダーを選択
   - Unity 2019.4以上で開く
   - プロジェクトの初期化とパッケージのインポートを待つ

3. **初期設定**

   - `Assets/JellyGarden/Scenes/`に移動
   - ゲームプレイには`game.unity`シーンを開く
   - レベル選択には`map.unity`シーンを開く

4. **ゲームをテスト**
   - Unityエディターで再生ボタンをクリック
   - またはターゲットプラットフォーム向けにビルド

### クイック設定

**基本設定** (`InitScript.cs`)：

```csharp
// ゲーム設定
public int startLife = 5;           // 開始ライフ数
public int startCoins = 100;        // 開始コイン数
public int levelToOpenEditor = 10;  // エディターを開くレベル
```

**レベル設定**：

- レベル保存場所：`Assets/JellyGarden/Resources/Levels/`
- 組み込みレベルエディターを使用してレベルを編集
- アクセス方法：Unity メニュー → Window → Level Editor

---

## 📁 プロジェクト構造

```
Jelly Garden Match 3/
│
├── Assets/
│   └── JellyGarden/
│       ├── Animation/          # アニメーションクリップとコントローラー
│       │   ├── Item animations
│       │   ├── UI animations
│       │   └── Effect animations
│       │
│       ├── Audio/              # 効果音と音楽
│       │   ├── BGM/
│       │   └── SFX/
│       │
│       ├── Fonts/              # カスタムフォントとマテリアル
│       │
│       ├── Materials/          # パーティクルとシェーダーマテリアル
│       │
│       ├── Prefabs/            # 再利用可能なゲームオブジェクト
│       │
│       ├── Resources/          # ランタイムで読み込み可能なアセット
│       │   ├── Levels/        # レベルデータファイル (.txt)
│       │   ├── Items/         # マッチ3アイテム
│       │   └── UI/            # UIプレハブ
│       │
│       ├── Scenes/             # Unityシーン
│       │   ├── game.unity     # メインゲームシーン
│       │   └── map.unity      # レベル選択シーン
│       │
│       ├── Scripts/            # C#ソースコード
│       │   ├── System/        # コアゲームシステム
│       │   ├── GUI/           # UIコントローラー
│       │   ├── Integrations/  # サードパーティサービス
│       │   ├── Leadboard/     # リーダーボードシステム
│       │   └── Editor/        # Unityエディター拡張
│       │
│       ├── SmartLevelsMap/     # レベルマップシステム
│       │
│       ├── Textures/           # スプライトと画像
│       │   ├── Items/
│       │   ├── UI/
│       │   └── Backgrounds/
│       │
│       └── Documentation/       # PDFとガイド
│
├── ProjectSettings/            # Unityプロジェクト設定
├── Packages/                   # パッケージ依存関係
└── README.md                   # このファイル
```

---

## 🔧 コアシステム

### ゲームマネージャー (`InitScript.cs`)

ゲーム状態、初期化、コアゲームループを管理する中央ハブ。

**主な責任：**

- ゲームの初期化と設定
- レベルの読み込みと管理
- プレイヤーデータの永続化
- スコアと目標の追跡
- ゲーム状態管理（プレイ中、一時停止、完了）

**重要なメソッド：**

```csharp
InitGame()              // ゲームシステムを初期化
LoadLevel(int num)      // 特定のレベルを読み込む
CheckWinLose()         // ゲーム完了条件をチェック
SaveMapPlayerPrefs()   // プレイヤーの進行状況を保存
```

### マッチシステム (`CombineManager.cs`)

すべてのマッチ検出、アイテム組み合わせ、特殊アイテム生成を処理。

**機能：**

- マッチ3以上の検出
- 特殊アイテム作成ルール
- コンボチェーンリアクション
- マッチスコアリングシステム

### レベルマネージャー (`LevelManager.cs`)

レベルデータ、目標、進行を管理。

**コンポーネント：**

- レベルデータパーサー
- 目標追跡
- 星計算
- レベル完了ロジック

### アイテムシステム (`Item.cs`, `Square.cs`)

個々のゲームピースとボードマスを制御。

**アイテムタイプ：**

- シンプルアイテム（6色）
- ストライプ（横/縦）
- ボム
- レインボーアイテム
- パッケージアイテム

---

## 🌐 統合とサービス

### Facebook統合

**セットアップ：**

1. [developers.facebook.com](https://developers.facebook.com)でFacebookアプリを作成
2. `FacebookManager.cs`にApp IDを追加
3. Android/iOSプラットフォーム設定を構成
4. 必要な権限を有効化（public_profile、user_friends）

**機能：**

- ユーザー認証
- フレンドリスト取得
- アバター読み込み
- スコア投稿

### 広告サービス

**サポートされているネットワーク：**

- Unity Ads
- AdMob
- カスタム広告ネットワーク統合

**設定：**

- 広告配置のために`AdsEvents.cs`を編集
- 各プラットフォームの広告ユニットIDを設定
- 報酬値を構成

### クラウドバックエンド

**GameSparks統合：**

- 場所：`Assets/JellyGarden/Scripts/Integrations/Network/Gamesparks/`
- 機能：プレイヤーデータ、リーダーボード、実績

**PlayFab統合：**

- 場所：`Assets/JellyGarden/Scripts/Integrations/Network/PlayFab/`
- 機能：プレイヤーアカウント、仮想経済、統計

---

## 📖 ドキュメント

プロジェクトには包括的なドキュメントが含まれています：

- **メインドキュメント**：`Assets/JellyGarden/JellyGardenDocumentation1.6.pdf`
- **オンラインガイド**：`Assets/JellyGarden/JellyGarden online doc.pdf`

### ドキュメントトピック：

1. **はじめに**

   - プロジェクト概要
   - Unity設定
   - シーン構造

2. **レベルデザイン**

   - レベルエディターの使用
   - 新しいレベルの作成
   - レベルバランス調整のヒント

3. **カスタマイズ**

   - ビジュアルの変更
   - ゲームプレイパラメータの変更
   - 新しいアイテムタイプの追加

4. **統合ガイド**

   - Facebook設定
   - 広告ネットワーク統合
   - バックエンドサービス構成

5. **ビルドと公開**
   - iOSビルドプロセス
   - Androidビルドプロセス
   - アプリストア提出

---

## 💻 システム要件

### Unity要件

| コンポーネント         | 最小要件   | 推奨      |
| ---------------------- | ---------- | --------- |
| Unityバージョン        | 2019.4 LTS | 2020.3以上 |
| .NETバージョン         | 4.x        | 4.x       |
| スクリプティングバックエンド | IL2CPP     | IL2CPP    |

### プラットフォーム要件

**iOS：**

- iOS 10.0以上
- Xcode 12以上
- CocoaPods（依存関係用）

**Android：**

- Android 4.4以上（API Level 19）
- Android SDK
- Gradle 6.1.1以上

### ハードウェア要件（開発環境）

- **プロセッサー**：Intel Core i5 / AMD Ryzen 5以上
- **RAM**：最小8GB、推奨16GB
- **ストレージ**：10GB以上の空き容量
- **グラフィックス**：DirectX 11/12対応GPU

---

## 🏗️ ビルドとデプロイ

### Androidビルド

1. **プレイヤー設定を構成**

   ```
   File → Build Settings → Android → Player Settings
   - 会社名を設定
   - 製品名を設定
   - パッケージ名を設定（com.yourcompany.jellygarden）
   - バージョンとBundle Version Codeを設定
   ```

2. **キーストアを構成**

   ```
   Publishing Settings
   - キーストアを作成または選択
   - キーストアパスワードを入力
   - エイリアスとパスワードを選択
   ```

3. **APK/AABをビルド**
   ```
   File → Build Settings → Android
   - 「Build App Bundle (Google Play)」または「Build APK」を選択
   - 出力場所を選択
   - Buildをクリック
   ```

### iOSビルド

1. **プレイヤー設定を構成**

   ```
   File → Build Settings → iOS → Player Settings
   - Bundle Identifierを設定
   - バージョンを設定
   - ターゲットSDKを設定
   - 署名を構成
   ```

2. **Xcodeプロジェクトをビルド**

   ```
   File → Build Settings → iOS
   - Buildをクリック
   - 出力フォルダーを選択
   - Xcodeプロジェクト生成を待つ
   ```

3. **Xcodeで開く**
   - 生成された.xcodeprojを開く
   - 署名証明書を構成
   - App Store用にビルドとアーカイブ

### 最適化のヒント

- **ビルドサイズの削減**：

  - コードストリッピングを有効化
  - アセット圧縮を使用
  - 未使用のリソースを削除

- **パフォーマンス**：
  - GPUインスタンシングを有効化
  - テクスチャアトラスを使用
  - パーティクルエフェクトを最適化
  - Unity Profilerでプロファイル

---

## 🤝 貢献

貢献を歓迎します！以下のガイドラインに従ってください：

### 開発ワークフロー

1. **リポジトリをフォーク**
2. **機能ブランチを作成**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **変更を加える**

   - C#コーディング規約に従う
   - 複雑なロジックにコメントを追加
   - 必要に応じてドキュメントを更新

4. **変更をコミット**

   ```bash
   git commit -m "素晴らしい機能を追加"
   ```

5. **ブランチにプッシュ**

   ```bash
   git push origin feature/amazing-feature
   ```

6. **プルリクエストを開く**

### コード標準

- [Microsoft C#コーディング規約](https://docs.microsoft.com/ja-jp/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)に従う
- 意味のある変数名とメソッド名を使用
- パブリックAPIにXMLドキュメントコメントを追加
- メソッドは焦点を絞り、可能な限り50行以内に保つ

### テスト

- PRを提出する前にiOSとAndroidでテスト
- 既存機能の退行がないことを確認
- 異なる画面解像度でテスト

---

## 💬 サポート

### ヘルプの取得

- **ドキュメント**：`Assets/JellyGarden/`のPDFガイドを確認
- **Issues**：GitHubで詳細な説明付きのissueを開く
- **メール**：support@yourcompany.com

### バグ報告

バグを報告する際は、以下を含めてください：

- Unityバージョン
- プラットフォーム（iOS/Android/エディター）
- 再現手順
- 期待される動作と実際の動作
- スクリーンショット/ログ（該当する場合）

### 機能リクエスト

機能提案を歓迎します！以下をお願いします：

- まず既存のissueを確認
- 明確なユースケースを提供
- 期待される動作を説明
- 実装の複雑さを考慮

---

## 📄 ライセンス

このプロジェクトは独占的ソフトウェアです。すべての権利を留保します。

**利用規約：**

- 教育目的と個人利用は許可
- 商用利用にはライセンスが必要
- 許可なしの再配布は禁止
- 保証は提供されません

ライセンスに関するお問い合わせ：license@yourcompany.com

---

## 🎯 ロードマップ

### 今後の機能

- [ ] 新しいゲームモード（タイムアタック、パズルモード）
- [ ] 追加の特殊アイテム
- [ ] シーズナルイベントシステム
- [ ] ギルド/チームシステム
- [ ] チャット機能
- [ ] ライブオペレーションダッシュボード

### バージョン履歴

- **v1.6**（現在）

  - 強化されたレベルエディター
  - パフォーマンス改善
  - バグ修正と安定性

- **v1.5**

  - PlayFab統合を追加
  - 新しいブースタータイプ
  - UI改善

- **v1.0**
  - 初回リリース
  - 100レベル
  - 基本的なソーシャル機能

---

## 🌟 クレジット

### 開発チーム

- **リード開発者**：[あなたの名前]
- **ゲームデザイン**：[デザイナー名]
- **アートとアニメーション**：[アーティスト名]
- **サウンドデザイン**：[サウンドデザイナー]

### サードパーティアセット

- **UIフレームワーク**：Unity UI
- **パーティクルエフェクト**：カスタムエフェクト
- **オーディオ**：ライセンス音楽と効果音
- **フォント**：Boris Black Bloxx、Candy Script

### 特別な感謝

すべての貢献者とUnityコミュニティのサポートとフィードバックに感謝します！

---

## 📞 連絡先

**プロジェクトメンテナー**：[あなたの名前]

- GitHub：[@NewbieAudioKid](https://github.com/NewbieAudioKid)
- メール：contact@yourcompany.com
- ウェブサイト：[yourcompany.com](https://yourcompany.com)

---

<div align="center">

**Unityで心を込めて作成**

[⬆ トップに戻る](#-jelly-garden-マッチ3ゲーム)

</div>

