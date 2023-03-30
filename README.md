Advance JavaScript
MODULE: 3
Name : Mohmad Mohasin

1. Create a program to hide/show the password

ANS.
<body>

<label for="password">Password:</label>
<input type="password" id="password" />
<button id="toggle-password">Show/Hide Password</button>
<script>
const passwordInput = document.getElementById('password');
const toggleButton = document.getElementById('toggle-password');
toggleButton.addEventListener('click', () => {
if (passwordInput.type === 'password') {
passwordInput.type = 'text';
toggleButton.textContent = 'Hide Password';
} else {
passwordInput.type = 'password';
toggleButton.textContent = 'Show Password';
}
});
</script>
</body>

2. Create a program that will select all the classes and loop over and
whenever i click the button the alert should show
Ans.
<body>

<button id="show-content">Show Content</button>
<p class="content">Element 1</p>
<p class="content">Element 2</p>
<p class="content">Element 3</p>

<script>
const contentElements = document.querySelectorAll('.content');
const showButton = document.getElementById('show-content');

contentElements.forEach(element => {
element.addEventListener('click', () => {
alert(`You clicked on ${element.textContent}`);
});
});

showButton.addEventListener('click', () => {
contentElements.forEach(element => {
alert(element.textContent);
});
});

</script>
</body>

3. Create a responsive header using proper JavaScript
Ans.
<body>

<label for="password">Password:</label>
<input type="password" id="password" />
<button id="toggle-password">Show/Hide Password</button>
<script>
const passwordInput = document.getElementById('password');
const toggleButton = document.getElementById('toggle-password');

toggleButton.addEventListener('click', () => {
if (passwordInput.type === 'password') {
passwordInput.type = 'text';
toggleButton.textContent = 'Hide Password';
} else {
passwordInput.type = 'password';
toggleButton.textContent = 'Show Password';
}
});

</script>

</body>

4. .Create a form and validate using JavaScript
Ans.
<body
>

<label for="password">Password:</label>
<input type="password" id="password" />
<button id="toggle-password">Show/Hide Password</button>
<script>
const passwordInput =
document.getElementById('password');
const toggleButton =
document.getElementById('toggle-password');

toggleButton.addEventListener('click', () => {
if (passwordInput.type === 'password') {
passwordInput.type = 'text';
toggleButton.textContent = 'Hide Password';
} else {
passwordInput.type = 'password';
toggleButton.textContent = 'Show Password';
}

});

</script>
</body>

5. Create a modal box using css and Js with three buttons
Ans.
<style>
.modal {
display: none;
position: fixed;
width: 100%;
height: 100%;
background-color: rgba(0,0,0,0.4);
}

.content {
background-color: #fefefe;
margin: 15% auto;
padding: 20px;
border: 1px solid #888;
width: 80%;
}

.close {
color: #aaa;
float: right;
font-size: 28px;
font-weight: bold;
}

.close:hover {
color: black;
text-decoration: none;
cursor: pointer;
}
</style>
<body>
<button onclick="openModal()">Open Modal</button>
<div id="myModal" class="modal">
<div class="content">
<span class="close" onclick="closeModal()"></span>
<p>Modal Content Goes Here</p>
<button>Button 1</button>
<button>Button 2</button>
<button>Button 3</button>
</div>
</div>

<script>

var modal = document.getElementById("myModal");
var btn = document.querySelector("button");
var span = document.getElementsByClassName("close")[0];
function openModal() {
modal.style.display = "block";
}
function closeModal() {
modal.style.display = "none";
}
window.onclick = function(event) {
if (event.target == modal) {
modal.style.display = "none";
}
}

</script>
</body>

6. Use external js library to show slider
Ans.
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width,
initial-scale=1.0">
<title>Document</title>
<link rel="stylesheet"
href="https://unpkg.com/swiper/swiper-bundle.min.css" />
</head>
<body>
<div id="myslider"></div>
<script>
var mySwiper = new Swiper('#mySlider', {
direction: 'horizontal',
loop: true,
pagination: {
el: '.swiper-pagination',
},
navigation: {
nextEl: '.swiper-button-next',
prevEl: '.swiper-button-prev',
},
scrollbar: {
el: '.swiper-scrollbar',
},

})

</script>

</body>
</html>

7. Prevent the browser when i click the form submit button
Ans.
<form id="myForm">
<button type="submit" id="submitButton">Submit</button>
</form>

<script>
const form = document.getElementById("myForm");
const submitButton = document.getElementById("submitButton");

submitButton.addEventListener("click", function(event) {
event.preventDefault();
});

</script>
