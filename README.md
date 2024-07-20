# Next.js Tutorial
勉強会用

## 技術スタック
| 項目| 名前 |　説明 |
| ---- | ---- |---- |
| 言語 | TypeScript ||
| フレームワーク(フロント) |  Next.js | |
| フレームワーク(CSS) | Tailwind ||

## 学んだこと
### 2章 CSS
- clsx
### 3章　Optimizing Fonts and Images
- fontモジュール
- Imgコンポーネント
### Creating Layouts and Pages
- layout.tsx
### 5章 
- Linkコンポーネント('next/link')
  - Next.jsはルートセグメントごとにコードを自動的に分割します
  - 旧来のReactに代表されるSPAの手法との違い
- usePathname
  - reactのhook
### 6章
- vercelへデプロイ
  - mainブランチにpushすると自動的に再デプロイされる
### 7章
- Data Fetch
- React Server Components
### 8章
- StaticRendering
### 9章
- loading.tsx
- ルートグループ
## 特徴
- ファイルシステムルーティング
  - 新しいページを作りたいときは、フォルダをきって配下にpage.tsxを書く。
  - Layout
    - 複数間にわたって同じUIを共有。再レンダリングも不要
    - パーシャルレンダリング
## 何が嬉しい？
- フォント最適化
  - レイアウトシフトを防ぐ
  - next/fontモジュールを使うことで、事前に静的アセットとしてビルドしておく。ユーザーがページを訪れた際にfontダウンロードのための通信が発生しないので、パフォーマンスに影響しない
  - サブセット化
- 画像最適化
  - よしなにしてくれる
- Linkコンポーネント('next/link')
  - Next.jsはルートセグメントごとにコードを自動的に分割します
  - 旧来のReactに代表されるSPAの手法との違い
- Server Component
## 後で調べる
- 5章
  - prefetch
  - client component
- 7章
  - server component
- 9章
  - streaming
    - ストリーミングによって、遅いデータ・リクエストがページ全体をブロックするのを防ぐことができます。 これにより、UIがユーザーに表示される前にすべてのデータがロードされるのを待つことなく、ユーザーはページの一部を見て操作することができます。
      - loading.tsx ファイル名で探しに行くっぽい
  - React Suspense