---
toc: true
comments: false
layout: post
title: Tri 2 indivisual review
description: A simple game where you drag and drop shapes!
type: tangibles
courses: { compsci: {week: 3} }
---
Project Overview
Our team built an image editor/painting website which would allow users to sign in, edit and save images, paint on a small board, and finally share their work with others. This involved a lot of input and output between users and the system, using JSON and JWT. There is a home page, painter, posting page, and profile tab.

My Feature
My feature was the drawing/painter included in our project. It asks the user to select what they want to draw between three options, and then a simple image of the answer is displayed. The image is displayed onto a working whiteboard, which the user can draw on with their mouse. They can select different colors, line width, and the eraser to color or draw something with the images.

Component A: Program Code
Collegeboard Requirements	Me
Instructions for input from one of the following: the user, a device, an online datas stream, a file.	My feature takes in user input in the form of button inputs. It asks the question and then waits for the user to select between 3 buttons.
Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the user's purpose.	In the JS, a list named drawingChoices is created to store a collection of input elements with the name "drawingChoice". This list is populated using the querySelectorAll method, which selects all input elements matching the specified criteria. Each element in the list represents a drawing choice input field on the webpage. This then manages the user's answer and handles the image displaying for them, so they can just draw as the painter wants to let them select an image and color/draw. LinktoPic
At least one procedure that contributed to the program’s intended purpose where you have defined: the name, return type, one or more parameters:	in this code, the displayAnswerImage is the name, the paramater is the choice string, and the return is in the code below, where it sets up the image to be loaded onto the canvas LinktoPic
An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure	In this JS, the code sequences the initialization of variables and the setup of event listeners for canvas interactions such as mouse down, move, up, and out actions. Then, the code engages in selection-based operations within the event listeners. For example, in the event listener for the eraser, the code employs conditional statements to select an action based on the current state of the variable eraserEnabled. Finally, the code utilizes iteration to efficiently handle the assignment of event listeners to multiple elements with the classes .colorSelector and .lineWidthSelector. LinktoPic
Calls to your student-developed procedure:	In the JS, within displayAnswerImage(choice), a switch statement is used to compute the value of the choice parameter, which represents the user's selection of a drawing option. Depending on the value of choice, corresponding calls are made to drawImageOnCanvas(imgSource) with specific image sources as the answers/response.LinktoPic
Instructions for output (tactile, audible, visual, or ) based on input and program functionality	In the JS, the program responds by triggering the handleDrawingOptionSelection(), which happens when the user interacts with one of the drawing selections. This function retrieves the value of the selected drawing option and uses the alert() method to generate a popup message about the users choice. this serves as the instructions on what to generate when the user clicks on something. LinkToPic
Component B: Video
LinkToVid

| Collegeboard Requirements | Me
|---------------------|-------------------------------------| | input to program | Inputting and pressing the button of 'cat' in the question container. | | at least one aspect of the functionality of your program | It has the ability to let the user draw with their mouse and select different colors on a whiteboard
| Output produced by program: | Outputs the image corresponding to the cat, and displays "You are drawing a cat" | | My video does not have: | Any distinguishing information and voice narration | | My video is| A .mp4, less than 1 minute in length, less than 30MB in file size. |