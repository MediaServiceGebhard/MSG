# MSG
Media Service Gebhard - Ihr Partner für Audio- Video- und Eventtechnik

<!DOCTYPE html>
<html lang="de">
    <head>
        <title>ESG</title>
        <link rel="stylesheet" href="style.css">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta charset="UTF-8">
        <meta name="description" content="Ihr Partner für Audio- Video- und Veranstaltungstechnik">
        <meta name="keywords" content="Audio, Video, Veranstaltungstechnik, Bearbeitung">
        <meta name="author" content="Julian Gebhard">
        <meta http-equiv="refresh" content="30">     
        <base href="https://ESG.com/index.html" target="_blank">   
    </head>
    <body>
        <header>
            <h1>ESG</h1>
        </header>

        <!-- Menü -->
        <div class="topnav" id="myTopnav">
            <a href="#home" class="active1">Home</a>
            <a href="#news">News</a>
            <a href="#contact">Contact</a>
            <a href="#about">About</a>
            <a href="javascript:void(0);" class="icon" onclick="myFunction()">&#9776;</a>
        </div>

        <!-- Slideshow -->
        <div class="slideshow-container">

        <!-- Full-width images with number and caption text -->
        <div class="mySlides fade">
        <div class="numbertext">1 / 3</div>
            <img src="img1.jpg" style="width:100%">
        <div class="text">Caption Text</div>
        </div>
      
        <div class="mySlides fade">
        <div class="numbertext">2 / 3</div>
            <img src="img2.jpg" style="width:100%">
        <div class="text">Caption Two</div>
        </div>
      
        <div class="mySlides fade">
        <div class="numbertext">3 / 3</div>
            <img src="img3.jpg" style="width:100%">
        <div class="text">Caption Three</div>
        </div>

        <!-- Next and previous buttons -->
        <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
        <a class="next" onclick="plusSlides(1)">&#10095;</a>
        </div>
        <br>
      
        <!-- The dots/circles -->
        <div style="text-align:center">
            <span class="dot" onclick="currentSlide(1)"></span> 
            <span class="dot" onclick="currentSlide(2)"></span> 
            <span class="dot" onclick="currentSlide(3)"></span> 
        </div>
    </body>
</html>


<!-- JavaScripte -->

<script>
    // ändert Menü 
function myFunction() {
    var x = document.getElementById("myTopnav");
    if (x.className === "topnav") {
        x.className += " responsive";
    } else {
        x.className = "topnav";
    }
}
</script>

<script>
    var slideIndex = 0;
showSlides();

function showSlides() {
    var i;
    var slides = document.getElementsByClassName("mySlides");
    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none"; 
    }
    slideIndex++;
    if (slideIndex > slides.length) {slideIndex = 1} 
    slides[slideIndex-1].style.display = "block"; 
    setTimeout(showSlides, 5000); // Bild wechselt alle 5 Sekunden
}
</script>
