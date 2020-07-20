# Exploring the HTML :

**Open the HTML index file. You'll see a number of features; the HTML is dominated by the video player and its controls:**
```
<div class="player">
<video controls>
<source src="video/sintel-short.mp4" type="video/mp4">
<source src="video/sintel-short.webm" type="video/webm">
<!-- fallback content here -->
</video>
<div class="controls">
<button class="play" data-icon="P" aria-label="play pause toggle"></button>
<button class="stop" data-icon="S" aria-label="stop"></button>
<div class="timer">
<div></div>
<span aria-label="timer">00:00</span>
</div>
<button class="rwd" data-icon="B" aria-label="rewind"></button>
<button class="fwd" data-icon="F" aria-label="fast forward"></button>
</div>
</div>
```

The whole player is wrapped in a `<div>` element, so it can all be styled as one unit if needed.
The `<video>` element contains two `<source>` elements so that different formats can be loaded depending on the browser viewing the site.
The controls HTML is probably the most interesting:
We have four `<button>`s — play/pause, stop, rewind, and fast forward.
Each `<button>` has a class name, a data-icon attribute for defining what icon should be shown on each button (we'll show how this works in the below section), and an aria-label attribute to provide an understandable description of each button, since we're not providing a human-readable label inside the tags. The contents of aria-label attributes are read out by screenreaders when their users focus on the elements that contain them.
There is also a timer `<div>`, which will report the elapsed time when the video is playing. Just for fun, we are providing two reporting mechanisms — a `<span>` containing the elapsed time in minutes and seconds, and an extra `<div>` that we will use to create a horizontal indicator bar that gets longer as the time elapses. To get an idea of what the finished product will look like, check out our finished version.
Exploring the CSS
Now open the CSS file and have a look inside. The CSS for the example is not too complicated, but we'll highlight the most interesting bits here. First of all, notice the .controls styling:
```
.controls {
visibility: hidden;
opacity: 0.5;
width: 400px;
border-radius: 10px;
position: absolute;
bottom: 20px;
left: 50%;
margin-left: -200px;
background-color: black;
box-shadow: 3px 3px 5px black;
transition: 1s all;
display: flex;
}
```
```
.player:hover .controls, player:focus .controls {
opacity: 1;
}
```
**We start off with the visibility of the custom controls set to hidden. In our JavaScript later on, we will set the controls to visible, and remove the controls attribute from the `<video>` element. This is so that, if the JavaScript doesn't load for some reason, users can still use the video with the native controls.**
**We give the controls an opacity of 0.5 by default, so that they are less distracting when you are trying to watch the video. Only when you are hovering/focusing over the player do the controls appear at full opacity.**
**We lay out the buttons inside the control bar using Flexbox (display: flex), to make things easier.**