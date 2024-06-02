---
{"dg-publish":true,"permalink":"/homepage/","tags":["gardenEntry"]}
---

hi

| Left Align | Center Align | Right Align |
|:-----------|:------------:|------------:|
| Row 1 Col 1 | Row 1 Col 2  | Row 1 Col 3 |
| Row 2 Col 1 | Row 2 Col 2  | Row 2 Col 3 |
Modal:

| Button       | Modal Content  |
|--------------|----------------|
| [Open Modal](#modal1) | Lorem ipsum dolor sit amet, consectetur adipiscing elit. |

<details id="modal1">
<summary>Modal Content</summary>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

</details>

Card:
 <!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
}
</style>
</head>
<body>

<div class="card">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG" alt="Avatar" style="width:100%">
  <div class="container">
    <h4><b>Title</b></h4> 
    <h6>Sub Title</h6> 
	 <p>Purpose</p>
  </div>
</div>

</body>
</html> 

Flip Card

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial, Helvetica, sans-serif;
}

.flip-card {
  background-color: transparent;
  width: 300px;
  height: 300px;
  perspective: 1000px;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color: #bbb;
  color: black;
}

.flip-card-back {
  background-color: #2980b9;
  color: white;
  transform: rotateY(180deg);
}
</style>
</head>
<body>

<h1>Card Flip with Text</h1>
<h3>Hover over the image below:</h3>

<div class="flip-card">
  <div class="flip-card-inner">
    <div class="flip-card-front">
      <img src="https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG" alt="Avatar" style="width:300px;height:300px;">
    </div>
    <div class="flip-card-back">
      <h4><b>Title</b></h4> 
    <h6>Sub Title</h6> 
	 <p>Purpose</p>
    </div>
  </div>
</div>

</body>
</html>
