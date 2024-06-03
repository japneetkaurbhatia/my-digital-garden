---
{"dg-publish":true,"permalink":"/homepage/","tags":["gardenEntry"]}
---

# Index

- [Table](#table)
- [Modal](#modal)
- [Static Card](#static-card)
- [Flip Card](#flip-card)
- [Multi Card](#multi-card)

## table

| Left Align  | Center Align | Right Align |
| :---------- | :----------: | ----------: |
| Row 1 Col 1 | Row 1 Col 2  | Row 1 Col 3 |
| Row 2 Col 1 | Row 2 Col 2  | Row 2 Col 3 |

---
## modal:

<details id="modal1">
<summary>Modal Content</summary>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

</details>

---
## static-card:

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
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG" alt="card-image" style="width:100%">
  <div class="container">
    <h4><b>Title</b></h4> 
    <h6>Sub Title</h6> 
	 <p>Purpose</p>
  </div>
</div>

</body>
</html> 

---

## flip-card:

<html lang="en">

<head>

<meta charset="UTF-8" />

<meta name="viewport" content="width=device-width, initial-scale=1.0" />

<title>Flip Card with Text</title>

<style>

.flip-card-container {

background-color: #f0f0f0;

}

  

.flip-card {

background-color: #292cd1;

width: 300px;

height: 200px;

perspective: 1000px;

}

  

.flip-card-inner {

position: relative;

width: 100%;

height: 100%;

text-align: center;

transition: transform 0.6s;

transform-style: preserve-3d;

}

  

.flip-card:hover .flip-card-inner {

transform: rotateY(180deg);

}

  

.flip-card-front,

.flip-card-back {

position: absolute;

width: 100%;

height: 100%;

backface-visibility: hidden;

}

  

.flip-card-front {

background-color: #bbb;

color: black;

display: flex;

flex-direction: column;

justify-content: center;

align-items: center;

}

  

.flip-card-back {

background-color: #2980b9;

color: white;

transform: rotateY(180deg);

display: flex;

flex-direction: column;

justify-content: center;

align-items: center;

}

</style>

</head>

<body>

<div class="flip-card-container">

<div class="flip-card">

<div class="flip-card-inner">

<div class="flip-card-front">

<h2>Front Side Title</h2>

<p>Front side content</p>

</div>

<div class="flip-card-back">

<h2>Back Side Title</h2>

<p>Back side content</p>

</div>

</div>

</div>

</div>

</body>

</html>


## multiple-card:

<html>

<head>

<meta name="viewport" content="width=device-width, initial-scale=1">

<style>

.custom-card {

box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);

transition: 0.3s;

width: 40%;

margin: 10px;

background-color: blueviolet;

}

  

.custom-card:hover {

box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);

}

  

.custom-container {

padding: 2px 16px;

}

  

.custom-card-container {

display: flex;

flex-wrap: wrap;

justify-content: space-around;

}

</style>

</head>

<body>

  

<div class="custom-card-container" id="custom-card-container">

</div>

  

<script>

const cardData = [

{

image: "https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG",

title: "Title 1",

subtitle: "Sub Title 1",

purpose: "Purpose 1"

},

{

image: "https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG",

title: "Title 2",

subtitle: "Sub Title 2",

purpose: "Purpose 2"

},

{

image: "https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG",

title: "Title 3",

subtitle: "Sub Title 3",

purpose: "Purpose 3"

}

];

  

const cardContainer = document.getElementById('custom-card-container');

  

cardData.forEach(data => {

const card = document.createElement('div');

card.className = 'custom-card';

card.innerHTML = `

<img src="${data.image}" alt="card-image" style="width:100%">

<div class="custom-container">

<h4><b>${data.title}</b></h4>

<h6>${data.subtitle}</h6>

<p>${data.purpose}</p>

</div>

`;

cardContainer.appendChild(card);

});

</script>

  

</body>

</html>