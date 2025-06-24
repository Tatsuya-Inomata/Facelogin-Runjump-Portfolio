# Unity × AI顔認証ログインゲーム（Run & Jump Game）

## 概要

本プロジェクトは、**Unity製2D Run & Jumpゲーム** に **Python + Flask による顔認証ログイン機能** を組み合わせたものです。ユーザーがゲームをプレイする前にカメラで撮影された顔画像を用いて、データベース内の画像と認証を行い、成功すればゲームが開始されます。

顔認証処理は Python の `face_recognition` ライブラリで実装され、Unity からは HTTP API を通じて Flask サーバに画像データを送信します。

---

## デモ動画

[YouTubeでデモを見る] 
※顔認証からゲームプレイまでを紹介しています。

## 使用技術
| 分野         | 使用技術                              |
|--------------|----------------------------------------|
| ゲーム        | Unity, C#                              |
| 顔認証        | Python, face_recognition, OpenCV       |
| APIサーバ     | Flask                                  |
| 通信         | UnityWebRequest（Unity → Flask）       |
| その他       | Pillow, NumPy, base64, WebCamTexture   |

### ゲーム部分（Unity）
- Unity 2021.3
- C#

### 顔認証アプリ部分（Python）
- Python 3.10
- face_recognition（顔画像認識）
- OpenCV（カメラ入力処理）

###　通信
- Flask（APIサーバー）
- UnityWebRequest (Unity → Flask)
