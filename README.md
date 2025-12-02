
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Flexbox 4x4 Image Grid</title>
<style>
* {
box-sizing: border-box;
margin: 0;
padding: 0;
}
body {
font-family: sans-serif;
}
.grid-container {
display: flex;
flex-wrap: wrap; 
justify-content: space-between; 
gap: 10px; 
padding: 10px;
max-width: 800px; 
margin: 20px auto; 
}
.grid-item {
flex-basis: calc(25% - 8px); 
flex-grow: 1; 
position: relative;
overflow: hidden;
padding-top: 25%; 
height: 0;
border: 1px solid #ccc;
}
.grid-item img {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
object-fit: cover; 
display: block;
}
</style>
</head>
<body>
<div class="grid-container">
<div class="grid-item"><img src="puzzle1_Q.jpg" alt="Image 1"></div>
<div class="grid-item"><img src="puzzle1_M.jpg" alt="Image 2"></div>
<div class="grid-item"><img src="puzzle1_J.jpg" alt="Image 3"></div>
<div class="grid-item"><img src="puzzle1_G.jpg" alt="Image 4"></div>
<div class="grid-item"><img src="puzzle1_A.jpg" alt="Image 5"></div>
<div class="grid-item"><img src="puzzle1_B.jpg" alt="Image 6"></div>
<div class="grid-item"><img src="puzzle1_H.jpg" alt="Image 7"></div>
<div class="grid-item"><img src="puzzle1_P.jpg" alt="Image 8"></div>
<div class="grid-item"><img src="puzzle1_E.jpg" alt="Image 9"></div>
<div class="grid-item"><img src="puzzle1_N.jpg" alt="Image 10"></div>
<div class="grid-item"><img src="puzzle1_C.jpg" alt="Image 11"></div>
<div class="grid-item"><img src="puzzle1_O.jpg" alt="Image 12"></div>
<div class="grid-item"><img src="puzzle1_F.jpg" alt="Image 13"></div>
<div class="grid-item"><img src="puzzle1_L.jpg" alt="Image 14"></div>
<div class="grid-item"><img src="puzzle1_K.jpg" alt="Image 15"></div>
<div class="grid-item"><img src="puzzle1_I.jpg" alt="Image 16"></div>
<img src="puzzle1_D.jpg" alt="Hidden Image" hidden>
</div>
