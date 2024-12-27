# Ex.08 Design of Interactive Image Gallery
# Date:16/11/2024
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
gallery.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="gallery styles.css">
</head>
<body>
    <div class="full-img" id="fullImgBox">
        <img src="C:\Users\admin\Downloads\img gallery-1.jpg" id="fullImg">
        <span onclick="closeFullImg()">X</span>
    </div>
    <div class="img-gallery">
        <img src="C:\Users\admin\Downloads\img gallery-1.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery2.jpeg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img gallery3.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery4.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery5.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery6.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery7.jpg" onclick="openFullImg(this.src)">
        <img src="c:\Users\admin\Downloads\img-gallery8.jpg" onclick="openFullImg(this.src)">
    </div>


<script>

    var fullImgBox = document.getElementById("fullImgBox");
    var fullImg = document.getElementById("fullImg");

    function openFullImg(pic){
        fullImgBox.style.display = "flex";
        fullImg.src = pic;
    }

    function closeFullImg(){
        fullImgBox.style.display = "none";
    }
</script>   
</body>
</html>

gallery styles.css
* {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}
body{
    background: #ecf4fb;
}
.img-gallery{
    width: 80%;
    margin: 100px auto 50px;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 30px;
}
.img-gallery img{
    width: 300px;
    height: 300px;
    cursor: pointer;
}

.img-gallery img:hover{
    transform: scale(0.8) rotate(-15deg);
    border-radius: 20px;
    box-shadow: 0 32px 75px rgba(68,77,136, 0.2)
}

.full-img{
    width: 100%;
    height: 100vh;
    background: rgba(0,0,0,0.9);
    position: fixed;
    top: 0;
    left: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 100;
}
.full-img img{
    width: 90%;
    max-width: 500px;
}
.full-img span{
    
    position: absolute;
    top: 5%;
    right: 5%;
    font-size: 30px;
    color: #fff;
    cursor: pointer;
}
```

# OUTPUT:

![Screenshot (84)](https://github.com/user-attachments/assets/1c9cc13e-b14f-4ab3-8d7e-332ca17b1ad5)

![Screenshot (85)](https://github.com/user-attachments/assets/7dddf23b-bf12-4455-862b-4a30229a4884)

![Screenshot (86)](https://github.com/user-attachments/assets/61efc5d9-2f3e-4171-b934-b3e6289ea5ab)

![Screenshot (87)](https://github.com/user-attachments/assets/07860a87-0156-4241-8ca2-516a6838905d)

![Screenshot (88)](https://github.com/user-attachments/assets/103d0c7c-3b90-4139-8c6c-ddc893cb3d76)

![Screenshot (89)](https://github.com/user-attachments/assets/2e420f6f-7f3f-4f64-a801-efb32d78ec00)

![Screenshot (90)](https://github.com/user-attachments/assets/fef758b7-3489-4877-b6b9-b8320cbc59b7)

![Screenshot (91)](https://github.com/user-attachments/assets/e0d3e5fc-5f3a-4479-814e-1e03ab000416)

![Screenshot (92)](https://github.com/user-attachments/assets/38a477c2-995a-45cc-a06f-17834539017a)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
