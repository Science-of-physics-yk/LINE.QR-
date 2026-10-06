# LINE.QR-

<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LINE 公式アカウント / 連絡先</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts Inter & Noto Sans JP -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Noto Sans JP', 'Inter', sans-serif;
        }
        /* カスタムLINEカラー定義 */
        .bg-line {
            background-color: #06C755;
        }
        .bg-line-hover:hover {
            background-color: #05b34c;
        }
        .text-line {
            color: #06C755;
        }
    </style>
</head>
<body class="bg-gradient-to-br from-slate-900 via-indigo-950 to-slate-900 min-h-screen flex flex-col justify-between items-center p-4 sm:p-6 text-slate-100">

    <!-- 
    ====================================================================
    【GitHub Pages 公開手順 & 画像差し替えガイド】
    ====================================================================
    1. このファイルを 「index.html」 という名前で保存します。
    2. QRコード画像（例: line-qr.png）を準備し、index.html と同じフォルダに置きます。
       - 下記の <img> タグの src を "line-qr.png" に書き換えてください。
    3. LINE追加用の直接リンクURL（https://line.me/ti/p/... や https://lin.ee/...）を取得し、
       「友だち追加」ボタンの href="" の中に貼り付けてください。
    4. GitHubにリポジトリを新規作成（Publicで作成）し、index.html と画像ファイルをアップロードします。
    5. GitHubの Settings > Pages を開き、
       Branch を "main" (または master) に設定して "Save" をクリックします。
    6. 数分後、発行されたURLにアクセスするとWebサイトが公開されます！
    ====================================================================
    -->

    <main class="w-full max-w-md my-auto">
        <!-- カードコンテナ -->
        <div class="bg-slate-800/80 backdrop-blur-md border border-slate-700/60 rounded-3xl shadow-2xl p-6 sm:p-8 text-center flex flex-col items-center">
            
            <!-- プロフィールアイコン / ロゴ Placeholder -->
            <div class="relative mb-4">
                <div class="w-20 h-20 sm:w-24 sm:h-24 rounded-full bg-gradient-to-tr from-emerald-500 to-teal-400 p-1 shadow-lg">
                    <!-- 画像を使う場合は下の <img> のコメントアウトを解除し、srcを指定してください -->
                    <!-- <img src="profile.jpg" alt="Profile" class="w-full h-full object-cover rounded-full"> -->
                    <div class="w-full h-full bg-slate-800 rounded-full flex items-center justify-center text-emerald-400 text-3xl font-bold">
                        <i class="fa-solid font-bold fa-user"></i>
                    </div>
                </div>
                <!-- LINEバッジ -->
                <div class="absolute bottom-0 right-0 bg-line text-white p-1.5 rounded-full shadow-md flex items-center justify-center">
                    <i class="fa-brands fa-line text-lg"></i>
                </div>
            </div>

            <!-- タイトル & 説明文 -->
            <h1 class="text-2xl sm:text-3xl font-bold tracking-tight text-white mb-2">
                公式アカウント名
            </h1>
            <p class="text-slate-300 text-sm sm:text-base mb-6 font-normal leading-relaxed">
                お問い合わせ・ご相談はLINE公式アカウントよりお気軽にご連絡ください。
            </p>

            <!-- QRコード表示エリア -->
            <div class="bg-white p-4 rounded-2xl shadow-inner border border-slate-200 mb-6 w-full max-w-[240px] aspect-square flex flex-col items-center justify-center">
                <!-- 
                  【QRコード画像の設定】
                  自分のLINE QRコード画像のファイル名に変更してください（例: src="line-qr.png"）
                -->
                <img 
                    src="https://placehold.co/300x300/06C755/white?text=LINE+QR+Code" 
                    alt="LINE QR Code" 
                    class="w-full h-full object-contain rounded-lg"
                    onerror="this.src='https://placehold.co/300x300/e2e8f0/475569?text=QR+Image+Error'"
                >
            </div>

            <!-- LINE追加ボタン (モバイルで直接LINEアプリを開くリンク) -->
            <a 
                href="https://line.me" 
                target="_blank" 
                rel="noopener noreferrer"
                class="w-full bg-line bg-line-hover text-white font-bold py-3.5 px-6 rounded-xl shadow-lg transition-all transform active:scale-95 flex items-center justify-center gap-3 text-base sm:text-lg mb-3"
            >
                <i class="fa-brands fa-line text-2xl"></i>
                <span>LINEで友だち追加</span>
            </a>

            <p class="text-xs text-slate-400">
                ※ スマホの方はボタンタップでLINEが開きます
            </p>
        </div>
    </main>

    <!-- フッター -->
    <footer class="text-center text-xs text-slate-500 py-4">
        <p>&copy; <span id="year"></span> Your Name / Business. All rights reserved.</p>
    </footer>

    <script>
        // 今日の年を自動取得
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>