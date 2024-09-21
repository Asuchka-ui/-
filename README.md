* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 20px;
    text-align: center;
}

.container {
    width: 80%;
    margin: 0 auto;
    padding: 20px;
}

h1, h2 {
    color: #333;
}

.gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.gallery-item {
    text-align: center;
    margin: 10px;
}

.gallery-item img {
    width: 45%;
    border-radius: 8px;
    transition: transform 0.3s ease;
    cursor: pointer;
}

.gallery-item img:hover {
    transform: scale(1.05);
}

footer {
    text-align: center;
    padding: 10px;
    background-color: #4CAF50;
    color: white;
}

.modal {
    display: none;
    position: fixed;
    z-index: 1000;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
}

.modal-content {
    margin: auto;
    display: block;
    max-width: 90%;
    max-height: 90%;
}

.close {
    position: absolute;
    top: 20px;
    right: 35px;
    color: #fff;
    font-size: 40px;
    cursor: pointer;
}

.close:hover {
    color: #999;
}
// Modal functionality for enlarging images
const modal = document.getElementById('modal');
const modalImg = document.getElementById('modalImage');
const closeBtn = document.getElementsByClassName('close')[0];
const images = document.getElementsByClassName('gallery-item');

Array.from(images).forEach(image => {
    image.onclick = function() {
        modal.style.display = 'block';
        modalImg.src = this.getElementsByTagName('img')[0].src;
    }
});

closeBtn.onclick = function() {
    modal.style.display = 'none';
}

window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = 'none';
    }
}
