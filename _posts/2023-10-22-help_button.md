---
toc: false
comments: false
layout: post
title: My help button work
description: work on Passion Project
type: tangibles
courses: { compsci: {week: 9} }
---
# This is my code for the help button

```js


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>User Profiles</title>
    <link rel="stylesheet" href="style.css"> <!-- Add your Phoenix theme stylesheet -->
    <link rel="icon" type="image/x-icon" href="images/Pheonix.jpg">
</head>
<body> 
    <div style = "position:relative; left: 25%; width:50%; border:white; border-left: solid 1px; border-right: solid 1px; padding: 5px; height:100%">
        <h1>Help</h1>
        <h3>Images: Make sure if you want to post an image, you make the link end with ".jpg"</h3>
        <h3>Link: Add the link to the post to link a website</h3>
        <h3>Code format:</h3>
        <h4>```(Write your programming language)</h4>
        <h4>your code</h4>
        <h4>```</h4>
        <button id="showexample">Example</button>
        <div id="image-container" style="display: none;">
            <img id="example-image" src="images/code_example.jpg" alt="Example Image" style = "left: 10%; position: relative; top: 20px">
            <br>
            <img id="result-image" src="images/code_result.jpg" alt="Result Image" style = "max-width:150%; left: 10%; position: relative; height:auto; top: 40px">
        </div>
        <h3 style = "position:relative; top:40px">Click the Friend page at the top bar to view your friends</h3>
        <h3></h3>

        <script>
            document.addEventListener('DOMContentLoaded', function () {
                const showExampleButton = document.getElementById('showexample');
                const imageContainer = document.getElementById('image-container');

                showExampleButton.addEventListener('click', function () {
                    // Toggle the image container's visibility
                    if (imageContainer.style.display === 'none') {
                        imageContainer.style.display = 'block';
                    } else {
                        imageContainer.style.display = 'none';
                    }
                });
            });
        </script>
    </div>
</body>
</html>
```