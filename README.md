<a href="https://github.com/tocoteron">
  <img align="left" height="170px" src="https://github-readme-stats.vercel.app/api?username=f-nakahara&count_private=true&show_icons=true&theme=dracula" />
</a>
<a href="https://github.com/tocoteron">
  <img align="left" height="170px" src="https://github-readme-stats.vercel.app/api/top-langs/?username=f-nakahara&layout=compact&theme=dracula" />
</a>

```
src/
├── features/                       // 機能単位でまとめる（UI・ロジック・状態）
│   ├── user/
│   │   ├── components.tsx          // ユーザー機能専用の UI コンポーネント
│   │   ├── hooks.ts                // カスタムフック
│   │   ├── usecases.ts             // ユースケース（UIから呼び出す操作単位）
│   │   ├── repository.ts           // データ取得処理（API, localStorageなど）
│   │   └── store.ts                // Zustand, Redux などの状態管理
│   ├── product/
│   └── order/
│
├── pages/                          // 複数 feature を組み合わせて画面を構築
│   ├── dashboard.tsx
│   └── user.tsx
│
├── shared/                         // 再利用可能な UI / ユーティリティ群
│   ├── components.tsx              // 共通UI（Button, Modalなど）
│   ├── utils.ts                    // 汎用関数（純関数）
│   ├── constants.ts                // 定数
│   └── types.ts                    // 共通型
│
├── core/                           // アプリ全体の基盤機能
│   ├── api.ts                      // API クライアント設定（axios等）
│   ├── auth.ts                     // 認証関連処理
│   ├── config.ts                   // 環境設定
│   └── store.ts                    // グローバルストアの初期化
│
└── main.tsx                        // エントリーポイント
```
