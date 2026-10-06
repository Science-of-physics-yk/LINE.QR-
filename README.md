<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LINE 公式アカウント</title>
    <style>
        /* 全体のスタイル設定 */
        body {
            font-family: sans-serif;
            background-color: #f4f5f7;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            box-sizing: border-box;
        }

        /* 中央の白いカード */
        .card {
            background-color: #ffffff;
            padding: 30px;
            border-radius: 16px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            text-align: center;
            max-width: 360px;
            width: 100%;
        }

        h1 {
            font-size: 20px;
            color: #333333;
            margin-top: 0;
            margin-bottom: 8px;
        }

        p {
            font-size: 14px;
            color: #666666;
            margin-top: 0;
            margin-bottom: 20px;
        }

        /* QRコード画像 */
        .qr-image {
            width: 200px;
            height: 200px;
            object-fit: contain;
            border: 1px solid #eeeeee;
            border-radius: 8px;
            margin-bottom: 20px;
        }

        /* LINEボタン */
        .line-button {
            display: block;
            background-color: #06C755; /* LINEの緑色 */
            color: #ffffff;
            text-decoration: none;
            font-weight: bold;
            font-size: 16px;
            padding: 12px 20px;
            border-radius: 8px;
            transition: background-color 0.2s;
        }

        .line-button:hover {
            background-color: #05b34c;
        }

        /* 初心者ガイド表示 */
        .guide {
            margin-top: 24px;
            padding-top: 16px;
            border-top: 1px dashed #dddddd;
            font-size: 12px;
            color: #888888;
            text-align: left;
            line-height: 1.6;
        }
    </style>
</head>
<body>

    <div class="card">
        <!-- タイトル -->
        <h1>公式LINEアカウント</h1>
        
        <!-- 説明文 -->
        <p>以下のQRコードを読み取るか、ボタンを押して友だち追加してください。</p>

        <!-- 
           【画像の設定】
           同じフォルダに「qr-code.png」という名前で画像を保存するか、
           以下の src="qr-code.png" の部分を画像ファイル名に変更してください。
        -->
        <img src="qr-code.png" alt="LINE QRコード" class="qr-image" onerror="this.src='https://placehold.co/200x200/06C755/white?text=QR+Image+Here'">

        <!-- 
           【LINEボタンの設定】
           href="https://line.me/ti/p/..." の部分にあなたのLINE追加URLを入れてください。
        -->
        <a href="https://line.me" target="_blank" class="line-button">LINEで友だち追加</a>

        <!-- 超かんたん解説 -->
        <div class="guide">
            <strong>【超かんたん使い方】</strong><br>
            1. QR画像を「<code>qr-code.png</code>」という名前でこのファイルと同じ場所に保存する。<br>
            2. ボタンの「<code>https://line.me</code>」を自分のLINE URLに変える。<br>
            3. このファイルを「<code>index.html</code>」の名前でGitHubにアップロードしてPages設定をONにするだけ！
        </div>
    </div>

</body>
</html>