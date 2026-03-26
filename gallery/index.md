<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        body {
            background: linear-gradient(135deg, #ff7e5f, #feb47b);
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            padding: 20px;
        }
        .card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            overflow: hidden;
            transition: transform 0.2s;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .image {
            width: 100%;
            height: 200px;
            background: url('path-to-image.jpg') no-repeat center center;
            background-size: cover;
        }
        .content {
            padding: 15px;
        }
        h3 {
            margin: 0 0 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="card">
            <div class="image" style="background-image: url('image1.jpg');"></div>
            <div class="content">
                <h3>Image Title 1</h3>
                <p>Description of image 1.</p>
            </div>
        </div>
        <div class="card">
            <div class="image" style="background-image: url('image2.jpg');"></div>
            <div class="content">
                <h3>Image Title 2</h3>
                <p>Description of image 2.</p>
            </div>
        </div>
        <div class="card">
            <div class="image" style="background-image: url('image3.jpg');"></div>
            <div class="content">
                <h3>Image Title 3</h3>
                <p>Description of image 3.</p>
            </div>
        </div>
        <!-- Add more cards as needed -->
    </div>
</body>
</html>
