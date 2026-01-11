<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Special Moments</title>
<style>
  body {
    margin: 0;
    background-color: #111;
    color: white;
    font-family: Arial, sans-serif;
    text-align: center;
    overflow-x: hidden;
  }
  #message {
    font-size: 2em;
    margin: 20px 0 10px 0;
    color: #ff69b4;
  }
  #slideshow {
    max-width: 90vw;
    max-height: 70vh;
    border-radius: 15px;
    box-shadow: 0 0 20px #ff69b4;
    margin-bottom: 20px;
    object-fit: contain;
  }
  iframe {
    border: none;
    width: 90vw;
    max-width: 560px;
    height: 315px;
    border-radius: 15px;
    box-shadow: 0 0 20px #ff69b4;
  }
</style>
</head>
<body>

<div id="message">❤️Special moments 💞</div>
<img id="slideshow" src="" alt="Slideshow" />
<!-- Embedded YouTube player -->
<iframe src="https://www.youtube.com/embed/NVmXJ6KtO3o?autoplay=1&loop=1&playlist=NVmXJ6KtO3o" allow="autoplay" allowfullscreen></iframe>

<script>
  const images = [
    "https://drive.google.com/uc?export=view&id=1ujxtYiM64a2exCoKO_xAalJORzXwqSIN",
    "https://drive.google.com/uc?export=view&id=1BZwQgd94KfLsx7c_Svu-r_EpcFuKlirG",
    "https://drive.google.com/uc?export=view&id=1HrwnXgNtQl2iFSnoOlQu3VHtiUF94CV4",
    "https://drive.google.com/uc?export=view&id=1oiWAc5a2hTZpu88jSjTdAEsDCihnSn8E",
    "https://drive.google.com/uc?export=view&id=1Oxgs1U_XCjJn0RCicyNtbUwpMwdpLhHY"
  ];

  let currentIndex = 0;
  const slideshow = document.getElementById('slideshow');

  function showNextImage() {
    slideshow.src = images[currentIndex];
    currentIndex = (currentIndex + 1) % images.length;
  }

  showNextImage();
  setInterval(showNextImage, 5000);
</script>

</body>
</html>
