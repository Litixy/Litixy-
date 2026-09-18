Litixy PWA版

GitHub Pagesへアップロードするときは、このフォルダの中身をリポジトリの公開ルートへ置いてください。

構成:
index.html
manifest.webmanifest
sw.js
images/litixy-logo.webp
icons/apple-touch-icon.png
icons/icon-192.png
icons/icon-512.png
icons/icon-512-maskable.png

プロジェクト画像:
1. GitHubで images フォルダへ画像を追加
2. index.html の LITIXY_MAIN_PROJECTS / LITIXY_PROJECTS に image のパスを書く
例:
{
  name: "LX Typing",
  category: "Typing Game",
  description: "Litixyのタイピングゲーム。",
  url: "https://example.com",
  image: "images/lx-typing.webp",
  imageFit: "cover",
  imagePosition: "center"
}

PWAはGitHub PagesなどHTTPS環境で動作します。ローカルの file:// で開いただけではService Workerは登録されません。
