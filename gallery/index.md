<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        body {
            background: linear-gradient(to bottom right, #ff7e5f, #feb47b); /* Warm gradient background */
            overflow: hidden;
            margin: 0;
            padding: 0;
        }
        .bg-circle-1, .bg-circle-2 {
            position: absolute;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.3);
            z-index: -1;
        }
        .bg-circle-1 {
            width: 300px;
            height: 300px;
            top: -100px;
            left: -100px;
        }
        .bg-circle-2 {
            width: 600px;
            height: 600px;
            bottom: -200px;
            right: -200px;
        }
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            padding: 20px;
        }
        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s;
        }
        .card:hover {
            transform: scale(1.05);
        }
        img {
            width: 100%;
            display: block;
        }
        .caption {
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="bg-circle-1"></div>
    <div class="bg-circle-2"></div>
    <div class="card-grid">
        <div class="card">
            <img src="img/img1.png" alt="Image 1">
            <div class="caption">🌟 Image 1 Caption</div>
        </div>
        <div class="card">
            <img src="img/img2.png" alt="Image 2">
            <div class="caption">🌈 Image 2 Caption</div>
        </div>
        <div class="card">
            <img src="img/img3.png" alt="Image 3">
            <div class="caption">🌻 Image 3 Caption</div>
        </div>
        <div class="card">
            <img src="img/img4.png" alt="Image 4">
            <div class="caption">✨ Image 4 Caption</div>
        </div>
    </div>
</body>
</html>