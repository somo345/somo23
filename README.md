<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sumerta x Akon</title>
    <style>
        /* Background dengan gradasi */
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #1e1e2f, #3a3a55);
            color: white;
            text-align: center;
            padding: 20px;
        }

        /* Animasi judul berwarna-warni & berkedip */
        @keyframes rainbow {
            0% { color: red; }
            20% { color: orange; }
            40% { color: yellow; }
            60% { color: green; }
            80% { color: blue; }
            100% { color: purple; }
        }

        @keyframes blink {
            0%, 50%, 100% { opacity: 1; }
            25%, 75% { opacity: 0.5; }
        }

        .title {
            font-size: 3rem;
            font-weight: bold;
            text-transform: uppercase;
            animation: rainbow 2s infinite linear, blink 1s infinite;
        }

        /* Tombol YouTube dengan animasi hover */
        .youtube-button {
            display: inline-block;
            background: red;
            color: white;
            padding: 12px 24px;
            font-size: 1.2rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(255, 0, 0, 0.5);
            transition: transform 0.2s, background 0.3s;
        }

        .youtube-button:hover {
            background: darkred;
            transform: scale(1.1);
        }

        /* Membuat video responsif */
        .video-container {
            position: relative;
            padding-bottom: 56.25%; /* Rasio aspek 16:9 */
            height: 0;
            overflow: hidden;
            max-width: 100%;
            background: black;
            margin-top: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(255, 255, 255, 0.3);
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
    </style>
</head>
<body>

    <!-- Judul dengan efek animasi warna-warni & berkedip -->
    <h1 class="title">Sumerta x Akon</h1>

    <!-- Tombol ke YouTube -->
    <h2>Tonton di YouTube:</h2>
    <a href="https://youtu.be/7ixTSPHMqaQ?si=GsYI2SfERMOC6wzU" target="_blank" class="youtube-button">
        Klik di sini untuk menonton
    </a>

    <!-- Video YouTube Responsif -->
    <h2>Video YouTube Tertanam:</h2>
    <div class="video-container">
        <iframe src="https://www.youtube.com/embed/7ixTSPHMqaQ" 
            title="Sumerta x Akon" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
            allowfullscreen>
        </iframe>
    </div>

</body>
</html>
