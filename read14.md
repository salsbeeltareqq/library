<html>
<style>
body {
  color: #fff;
  font:  14px/24px "Open Sans", "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", Sans-Serif;
}
.box {
  background: #2db34a;
  border-radius: 6px;
  cursor: pointer;
  height: 95px;
  line-height: 95px;
  text-align: center;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
  width: 95px;
  float : right;
}
.box:hover {
  background: #ff7b29;
}
</style>
<div class="box">Box</div>
</html>

A handful of the more popular transitional properties include the following.

- **Transition Duration** : The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

<html>
<style>
body {
  color: #fff;
  font:  14px/24px "Open Sans", "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", Sans-Serif;
}
.box1 {
    background: #2db34a;
  border-radius: 6px;
  cursor: pointer;
  height: 95px;
  line-height: 95px;
  text-align: center;
  width: 95px;
  float : right;
  transition: background .2s linear, border-radius 1s ease-in 1s;
}
.box1:hover {
  background: #ff7b29;
  border-radius: 50%;
}
</style>
<div class="box1">Box</div>
</html>

- **Transition Delay** : you can also set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.

### Animation.

Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

- **Animation Keyframes** : To set multiple points at which an element should undergo a transition, use the`@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

<html>
<style>
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
.stage {
  background: #eaeaed;
  border-radius: 6px;
  height: 150px;
  position: relative;
  min-width: 538px;
}
.stage:hover .ball {
  animation: slide 2s linear;
}
.ball {
  background: #2db34a;
  border-radius: 50%;
  height: 50px;
  position: absolute;
  width: 50px;
}
</style>
<div class="stage">
  <figure class="ball"></figure>
</div>
</html>

- **Animation Iteration** : By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the `animation-iteration-count : infinite` property may be used

<html>
<style>
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
.stage1 {
  background: #eaeaed;
  border-radius: 6px;
  height: 150px;
  position: relative;
  min-width: 538px;
}
.stage1:hover .ball1 {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-iteration-count: infinite;
}
.ball1 {
  background: #2db34a;
  border-radius: 50%;
  height: 50px;
  position: absolute;
  width: 50px;
}
</style>
<div class="stage1">
  <figure class="ball1"></figure>
</div>
</html>
