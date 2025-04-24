# Ex.05 Design of Interactive Image Gallery
## Date:24.04.2025

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
            background-color: #000000;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            padding: 20px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.5);
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
    <br>
    <br>
    <br>

    <h1 style="text-align: center; margin-top: 20px; color: #fff;">Interactive Photo Gallery</h1>
    <h3 style="text-align: center; margin-top: 20px; color: #fff;">M.Suryakumar 212224040340</h3>
     <br>
     <br>
     <br>
     <br>
     <br>

    <div class="gallery">
        <div class="gallery-item" data-image="image1.jpg">
            <img src="image 2.png" alt="Photo 1" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image2.jpg">
            <img src="image 3.webp" alt="Photo 2" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
            <img src="image 4.jpg" alt="Photo 3" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
          <img src="image 5.avif" alt="Photo 3" onclick="openModal(this)">
      </div>
      <div class="gallery-item" data-image="image3.jpg">
        <img src="image 6.webp" alt="Photo 3" onclick="openModal(this)">
    </div>
    <div class="gallery-item" data-image="image3.jpg">
      <img src="image 7.png" alt="Photo 3" onclick="openModal(this)">
  </div>
        
    </div>

    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        function openModal(image) 
        {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() 
        {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>

</body>
</html>
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/6055e08c-6281-4598-9707-9b4ab7b90147)

![image](https://github.com/user-attachments/assets/b4246138-67c3-4d02-a7fd-49c89dda2c7b)

![image](https://github.com/user-attachments/assets/835b1df2-3a42-4fad-905c-0c8c7196c356)

![image](https://github.com/user-attachments/assets/b4b50d79-1c99-4f50-8974-367aeff43414)

![image](https://github.com/user-attachments/assets/51571ae7-b5a6-4b9d-99b8-1a8f3ff2a81b)

![image](https://github.com/user-attachments/assets/b2f49e43-d232-4ccb-b8bb-2cf35a802784)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
