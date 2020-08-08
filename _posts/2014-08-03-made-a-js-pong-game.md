---
layout: post
title:  "Pong like it's 1978"
date:   2014-08-03 13:06:02 -0500
categories: js javascript archive update
---

**NOTE:**This was one of the first things I ever created on the web and is also an old post from 2014 according to the [repo history](https://github.com/cartothemax/pongjs/tree/master).
Hello again, I have created another game using Javascript. This time I created pong!

My reasoning for learning this time was to use good coding practices associated with Javascript using the [constructor pattern](https://addyosmani.com/resources/essentialjsdesignpatterns/book/#constructorpatternjavascript). This also introduced me to [setInterval](https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setInterval) and other [asynchronous](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Synchronous_and_Asynchronous_Requests) topics within Javascript.

Here is a copy of my version of the game.
<div>
<p>Player 1 controls: up -> "W" down -> "S"</p>
<p>Player 2 controls: up -> "O" down -> "K"</p>
Player 1: <div id='playerone'>0</div>
Player 2: <div id='playertwo'>0</div>
<div id="startMenu" style="background-color: black; position: absolute; text-align: center; width: 500px; height: 500px; visibility: visible;">
<h1 style="color: white;">PongJS</h1>
<button style="margin-top: 50%;" onclick="startGame()">Start Game?</button>
</div>
<canvas id="gameBoard" style="width: 500px; height: 500px; visibility: none;">
    Your browser doesn't support canvas
</canvas>
</div>
<script src="../../../../../../paddle.js" type="text/javascript"></script>
<script src="../../../../../../ball.js" type="text/javascript"></script>
<script src="../../../../../../gameBoard.js" type="text/javascript"></script>
<script src="../../../../../../pong.js" type="text/javascript"></script>
