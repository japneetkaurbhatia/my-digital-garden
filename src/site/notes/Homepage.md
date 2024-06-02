---
{"dg-publish":true,"permalink":"/homepage/","tags":["gardenEntry"]}
---

# Index - now

- [Table](#table)
- [Modal](#modal)
- [Static Card](#static-card)
- [Card with Flip](#card-with-flip)
- [Card with Flip Images](#card-with-flip-images)
- [Card with Flip Text](#card-with-flip-text)

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
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG" alt="Avatar" style="width:100%">
  <div class="container">
    <h4><b>Title</b></h4> 
    <h6>Sub Title</h6> 
	 <p>Purpose</p>
  </div>
</div>

</body>
</html> 

---
## card-with-flip

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
---
## card-with-flip-images

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flip Card</title>
  <style>
    .flip-card {
      width: 300px;
      height: 300px;
      perspective: 1000px;
    }

    .flip-card-inner {
      width: 100%;
      height: 100%;
      text-align: center;
      transition: transform 0.6s;
      transform-style: preserve-3d;
    }

    .flip-card:hover .flip-card-inner {
      transform: rotateY(180deg);
    }

    .flip-card-front, .flip-card-back {
      width: 100%;
      height: 100%;
      backface-visibility: hidden;
      position: absolute;
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

<div class="flip-card">
  <div class="flip-card-inner">
    <div class="flip-card-front">
      <img src="https://upload.wikimedia.org/wikipedia/commons/5/58/AcetoFive.JPG" alt="Front Image">
    </div>
    <div class="flip-card-back">
      <img src="https://images.unsplash.com/photo-1587474260584-136574528ed5?q=80&w=1000&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8ZGVsaGl8ZW58MHx8MHx8fDA%3D" alt="Back Image">
    </div>
  </div>
</div>

</body>
</html>

---
## card-with-flip-text
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flip Card with Text</title>
<style>
  .flip-card-container {
    background-color: #f0f0f0; /* Background color for the flip card container */
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .flip-card {
    background-color: transparent;
    width: 300px;
    height: 200px; /* Adjust height as needed */
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

  .flip-card-front, .flip-card-back {
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
        <p>Front side content goes here.</p>
      </div>
      <div class="flip-card-back">
        <h2>Back Side Title</h2>
        <p>Back side content goes here.</p>
      </div>
    </div>
  </div>
</div>

</body>
</html>


