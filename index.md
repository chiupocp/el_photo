<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>我的摄影集</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/lightgallery.js/dist/css/lightgallery.min.css">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { background: #fafafa; font-family: -apple-system, BlinkMacSystemFont, sans-serif; }
    .gallery {
      columns: 3;
      column-gap: 12px;
      max-width: 1200px;
      margin: 40px auto;
      padding: 0 20px;
    }
    .gallery-item {
      break-inside: avoid;
      margin-bottom: 12px;
      cursor: pointer;
      border-radius: 6px;
      overflow: hidden;
    }
    .gallery-item img {
      width: 100%;
      display: block;
      transition: transform 0.3s ease;
    }
    .gallery-item:hover img { transform: scale(1.02); }
    @media (max-width: 768px) { .gallery { columns: 2; } }
    @media (max-width: 480px) { .gallery { columns: 1; } }
  </style>
</head>
<body>
  <div class="gallery" id="gallery">
    <a href="https://pub-725f084f4f9e40dd9cf5c2aed5a4cc84.r2.dev/5D4_3275-%E7%BC%96%E8%BE%91-Exposure_NIK.jpg" class="gallery-item">
      <img src="https://pub-725f084f4f9e40dd9cf5c2aed5a4cc84.r2.dev/5D4_3275-%E7%BC%96%E8%BE%91-Exposure_NIK.jpg" alt="作品1">
    </a>
    <a href="你的第2张R2图片链接" class="gallery-item">
      <img src="你的第2张R2图片链接" alt="作品2">
    </a>
    <a href="你的第3张R2图片链接" class="gallery-item">
      <img src="你的第3张R2图片链接" alt="作品3">
    </a>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/lightgallery.js/dist/js/lightgallery.min.js"></script>
  <script>
    lightGallery(document.getElementById('gallery'), {
      selector: 'a',
      download: false,
      counter: false,
      bgColor: '#000'
    });
  </script>
</body>
</html>
