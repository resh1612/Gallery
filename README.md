# Ex.08 Design of Interactive Image Gallery
# Date:16.12.2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
            background-image:url("exp08bg.jpg");
        }

        h1 {
            margin-top: 20px;
            color: #f4f4f4;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 200px;
            height: 150px;
            border: 2px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="C:\Users\balaj\.vscode\gal1.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="C:\Users\balaj\.vscode\gal2.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="C:\Users\balaj\.vscode\gal3.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="C:\Users\balaj\.vscode\gal4.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="C:\Users\balaj\.vscode\gal5.jpg" alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>

```

# OUTPUT:
![WhatsApp Image 2024-12-16 at 20 44 02_bb1d772e](https://github.com/user-attachments/assets/fbe5e9df-c241-48ac-89a1-b4c124dc06d5)
![WhatsApp Image 2024-12-16 at 20 37 47_c5b4cb17](https://github.com/user-attachments/assets/40952450-b3b4-4c92-ad99-24891e1289ca)
![WhatsApp Image 2024-12-16 at 21 23 42_8fdf2290](https://github.com/user-attachments/assets/5f2ac4d6-1a69-4d8f-b3eb-2d17e896cb82)
![WhatsApp Image 2024-12-16 at 20 44 53_ad5795dc](https://github.com/user-attachments/assets/38a18bf1-cdeb-41cb-b905-9c39c0326a9f)
![WhatsApp Image 2024-12-16 at 20 39 12_064d373f](https://github.com/user-attachments/assets/5adb1bd5-3a4b-4b9f-883d-3a52eb5daf17)
![WhatsApp Image 2024-12-16 at 20 39 41_3c4277e7](https://github.com/user-attachments/assets/219b7cc2-917d-4857-bb18-4d25be15c06e)
![WhatsApp Image 2024-12-16 at 20 40 14_2895cbfb](https://github.com/user-attachments/assets/09a22a60-2cf1-45ac-8a24-225854a94055)
![WhatsApp Image 2024-12-16 at 20 40 42_c4a3f2e8](https://github.com/user-attachments/assets/aa716f25-151b-4686-870c-c2ffd8341115)
![WhatsApp Image 2024-12-16 at 20 41 12_e89a0c68](https://github.com/user-attachments/assets/db9af037-c9e5-41e8-8ad0-b735a3e31c9f)
![WhatsApp Image 2024-12-16 at 20 42 05_466c0a7d](https://github.com/user-attachments/assets/a08c6fa8-8294-4578-b836-39ad23460286)
![WhatsApp Image 2024-12-16 at 20 42 27_c6786211](https://github.com/user-attachments/assets/1d173381-fed4-4a56-84d8-5951f70c7304)













# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
