# Show/Hide Password Toggle

This repository provides a simple example of how to implement a "Show/Hide Password" feature in a web form using HTML, CSS, and JavaScript.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Demo

You can see a live demo of this feature [here](https://example.com/show-hide-password-demo).

## Features

- Allows users to toggle the visibility of their password input in a web form.
- Enhances user experience and security in web applications.

## Usage

To use this feature in your project, follow these steps:

1. Clone this repository to your local machine.
2. Copy the relevant HTML, CSS, and JavaScript code to your project.
3. Modify the code as needed to integrate it with your existing web form.

```html
<!-- Include the HTML code for the password input and toggle button -->
<div class="input-box">
        <input type="password" placeholder="Password" id="password">
        <img src="eye-close.png" id="eyeicon">
    </div>

<!-- Include the JavaScript code to toggle the password visibility -->
<script>
  let eyeicon = document.getElementById("eyeicon");
let password = document.getElementById("password");

eyeicon.onclick = function () {
    if (password.type == "password") {
        password.type = "text";
        eyeicon.src = "eye-open.png";
    } else {
        password.type = "password";
        eyeicon.src = "eye-close.png"
    }
}
</script>
