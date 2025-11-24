ha
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Four Pictures with Text</title>
<style>
.container {
width: 100%;
overflow: hidden; /* Clear floats */
text-align: center;
}
.item {
float: left; /* Poseidon property: float */
width: 22%; /* Slightly less than 25% to account for spacing */
margin: 1%; /* Even spacing between items */
box-sizing: border-box;
}
.item img {
width: 100%;
height: auto;
display: block;
}
.caption {
margin-top: 8px;
font-family: Arial, sans-serif;
}
</style>
</head>
<body>
<div class="container">
<div class="item">
<img src="https://pethelpful.com/.image/w_750,q_auto:good,c_limit/NDowMDAwMDAwMDAwMTA3MjEy/siberian-husky-107212.jpg?arena_f_auto" alt="Picture 1" />
<div class="caption">Picture 1</div>
</div>
<div class="item">
<img src="<img src="https://pethelpful.com/.image/w_750,q_auto:good,c_limit/NDowMDAwMDAwMDAwMTA3MjE5/german-shepherd-laying-in-grass-107219.jpg?arena_f_auto" alt="Picture 2"/>
<div class="caption">Picture 2</div>
</div>
<div class="item">
<img src="https://pethelpful.com/.image/w_750,q_auto:good,c_limit/NDowMDAwMDAwMDAwMTA3MjI1/black-lab-in-fall-leaves-107225.jpg?arena_f_auto" alt="Picture 3" />
<div class="caption">Picture 3</div>
</div>
<div class="item">
<img src="https://pethelpful.com/.image/w_750,q_auto:good,c_limit/NDowMDAwMDAwMDAwMTA3MjY2/ready-to-play-107266.jpg?arena_f_auto" alt="Picture 4" />
<div class="caption">Picture 4</div>
</div>
</div>
</body>
</html>
