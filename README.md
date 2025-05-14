# Ex.08 Design of Interactive Image Gallery
## Date:14.05.2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>

<head>
    <title>Image Gallery</title>
    <link rel="stylesheet" href="style.css">
    <script src="script.js" defer></script>
</head>

<body class="back">

    <h1 align="center" style="font-family: Georgia, 'Times New Roman', Times, serif;color: rgb(255, 60, 0);">
        CHENNAI</h1>

    <div class="gallery">
        <br><br><br>
        <img src="images/img 2.jpg" alt="Image 1" class="gallery-item" onclick="openModal(this)">
        <img src="images/img 6.jpg" alt="Image 2" class="gallery-item" onclick="openModal(this)">
        <img src="images/img 3.jpg" alt="Image 3" class="gallery-item" onclick="openModal(this)">
        <img src="images/img 1.jpg" alt="Image 4" class="gallery-item" onclick="openModal(this)">
        <img src="images/img 5.jpg" alt="Image 5" class="gallery-item" onclick="openModal(this)">
        <img src="images/img 4.jpg" alt="Image 5" class="gallery-item" onclick="openModal(this)">
         <div style="margin-top: 30px;">
        <span>Normal</span>
        <span style="margin-left: 50px;">Spaced 50px</span>
    </div>
    </div>

    <div id="imageModal" class="modal">
        <span class="close" onclick="closeModal()">&times;</span>
        <img class="modal-content" id="modalImage">
    </div>

</body>

</html>

body {
    background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
}

.gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 30px; /* Increased from 10px to 30px */
    padding: 20px;
    justify-content: center;
}

.gallery-item {
    margin: 15px; /* Increased margin for more spacing */
    width: 300px;
    height: auto;
    cursor: pointer;
    border-radius: 15px;
    border: 2px solid #4bc8c8;
    transition: transform 0.3s; /* Smoother hover animation */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Optional: adds depth */
}

.gallery-item:hover {
    transform: scale(1.05); /* More subtle hover effect */
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3); /* Enhanced shadow on hover */
}
.modal {
    display: none;
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    justify-content: center;
    align-items: center;
}

.modal-content {
    max-width: 80%;
    max-height: 80%;
}

.close {
    position: absolute;
    top: 20px;
    right: 30px;
    font-size: 30px;
    color: rgb(167, 61, 61);
    cursor: pointer;
}

.back {
    background-color: rgb(22, 21, 20);
}

function openModal(image) {
    const modal = document.getElementById('imageModal');
    const modalImg = document.getElementById('modalImage');

    modal.style.display = "flex";
    modalImg.src = image.src;
}

function closeModal() {
    const modal = document.getElementById('imageModal');
    modal.style.display = "none";
}

```
## OUTPUT:
![alt text](<Screenshot 2025-05-14 192653.png>)
![alt text](<Screenshot 2025-05-14 192709.png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
