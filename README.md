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
    <br><br><br>
    <h1 style="text-align: center; margin-top: 20px; color: #fff;">Interactive Photo Gallery</h1>
    <h3 style="text-align: center; margin-top: 20px; color: #fff;">M.Suryakumar 212224040340</h3>
    <br><br><br><br><br>

    <div class="gallery">
        <div class="gallery-item">
            <img src="https://uploads.sarvgyan.com/2014/06/cse-image.jpg" alt="Photo 1" onclick="openModal(this)">
        </div>
        <div class="gallery-item">
            <img src="https://images.pexels.com/photos/614117/pexels-photo-614117.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Photo 2" onclick="openModal(this)">
        </div>
        <div class="gallery-item">
            <img src="https://images.pexels.com/photos/6755078/pexels-photo-6755078.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Photo 3" onclick="openModal(this)">
        </div>
        <div class="gallery-item">
            <img src="https://images.pexels.com/photos/18069696/pexels-photo-18069696/free-photo-of-an-artist-s-illustration-of-artificial-intelligence-ai-this-illustration-depicts-language-models-which-generate-text-it-was-created-by-wes-cockx-as-part-of-the-visualising-ai-project-l.png?auto=compress&cs=tinysrgb&w=600" alt="Photo 4" onclick="openModal(this)">
        </div>
        <div class="gallery-item">
            <img src="https://media.istockphoto.com/id/1846545372/photo/chat-with-ai-artificial-intelligence-innovation-applying-ai-and-supporting-operations-data.jpg?s=612x612&w=0&k=20&c=sOI63Ml1a64Z9DpxkEaOE1h08gXIhnCP_wl1wyO5ZLY=" alt="Photo 5" onclick="openModal(this)">
        </div>
        <div class="gallery-item">
            <img src="https://media.istockphoto.com/id/940442486/photo/hacker-programing-in-technology-enviroment-with-cyber-icons.jpg?s=612x612&w=0&k=20&c=BOLumv_Hzf1eHuzL3RwkgVgbqRVBnvwOsWl_ko_4o8g=" alt="Photo 6" onclick="openModal(this)">
        </div>
    </div>

    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>

</body>
</html>
https://uploads.sarvgyan.com/2014/06/cse-image.jpg
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/c9d53f3c-2b78-4428-b714-4f0d8caf9d06)

![image](https://github.com/user-attachments/assets/b6b6a402-6608-4878-b1bf-0c14af16eac0)

![image](https://github.com/user-attachments/assets/5fa4e574-99a0-47fd-9f5e-ff3a22d49c53)

![image](https://github.com/user-attachments/assets/5c550f60-b30d-42ad-aad3-b59db407e259)

![image](https://github.com/user-attachments/assets/058d7634-3caf-4475-bf69-e68ab3363fba)


![image](https://github.com/user-attachments/assets/a6ba40a6-37f1-4f66-b2e1-4a0e669b2c50)

![image](https://github.com/user-attachments/assets/5069aa02-fbb4-4114-b8bf-5ee8fdc24fc8)



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
