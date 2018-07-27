# [HTML-CSS] Animations d'UI

<ul>
    <li>
        <div id="easing"><span></span></div>
        <h4>Easing</h4>
    </li>
    <li>
        <div id="parenting"><span></span><span></span></div>
        <h4>Parenting</h4>
    </li>
    <li>
        <div id="obscuration"><span></span></div>
        <h4>Obscuration</h4>
    </li>
    <li>
        <div id="parallax"><span></span></div>
        <h4>Parallax</h4>
    </li>
    <li>
        <div id="dimension"></div>
        <h4>Dimentionality</h4>
    </li>
    <li>
        <div id="transformation"></div>
        <h4>Transformation</h4>
    </li>
    <li>
        <div id="dollyZoom">
            <ul>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
            </ul>
        </div>
        <h4>Dolly & Zoom</h4>
    </li>
    <li>
        <div id="masking"><span></span></div>
        <h4>Masking</h4>
    </li>
</ul>

[CodePen](https://codepen.io/prvnbist/pen/zRMaeK)

<style>
@import url("https://fonts.googleapis.com/css?family=Open+Sans");
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
ul {
  background-image: linear-gradient(-45deg, #00c6fb 0%, #005bea 100%);

  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: 50vh;
}
li {
  border: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
h4 {
  position: absolute;
  left: 50%;
  bottom: 8vh;
  transform: translate(-50%, 0);
  text-align: center;
  margin-top: 40px;
  color: #fff;
  font-family: 'Open Sans', sans-serif;
}
@media screen and (max-width: 767px) {
  ul {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media screen and (max-width: 567px) {
  ul {
    grid-template-columns: 1fr;
    grid-auto-rows: 100vh;
  }
}
span {
  border-radius: 4px;
  display: block;
}
/***
 Easing
 ***/
#easing {
  overflow: hidden;
  width: 200px;
}
#easing span {
  width: 80px;
  height: 80px;
  background: #fff;
  animation: easing 2s ease-out infinite;
}
@keyframes easing {
  0% {
    transform: translateX(-120px);
  }
  75% {
    transform: translateX(40px);
  }
  100% {
    transform: translateX(250px);
  }
}
/***
 Parenting
 ***/
#parenting span {
  width: 100px;
  height: 40px;
  background: #fff;
  margin: 10px 0;
  animation: slide 1s ease-in-out infinite alternate;
}
@keyframes slide {
  0% {
    transform: translateX(-50px);
  }
  100% {
    transform: translateX(50px);
  }
}
#parenting span:first-child {
  transform-origin: 50% 100%;
  animation: growShrink 1s ease-in-out infinite alternate;
}
@keyframes growShrink {
  0% {
    transform: translateX(-50px) scale(0.1);
  }
  100% {
    transform: translateX(50px) scale(1);
  }
}
/***
 Obscuration
 ***/
#obscuration {
  width: 60px;
  height: 80px;
  background: #fff;
  border-radius: 4px;
  position: relative;
}
#obscuration span {
  opacity: 0.7;
  width: 90px;
  height: 110px;
  background: #f7f7f7;
  position: absolute;
  top: 50%;
  left: -60px;
  transform: translate(0, -50%);
  animation: obscure 1s cubic-bezier(0.6, 0, 0.4, 1) infinite alternate;
}
@keyframes obscure {
  100% {
    left: 30px;
  }
}
/***
 Dolly & Zoom
 ***/
#dollyZoom {
  width: 160px;
  height: 100px;
  background: transparent;
  overflow: hidden;
  border-radius: 4px;
  position: relative;
}
#dollyZoom ul {
  width: 480px;
  height: 300px;
  background: transparent;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border-radius: 4px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: 100px;
  grid-gap: 3px;
  transform-origin: -34% -34%;
  animation: zoom 1s ease-in-out infinite alternate;
}
@keyframes zoom {
  100% {
    transform: scale(0.4);
  }
}
#dollyZoom li {
  background: #fff;
  border-radius: 0;
}
/***
 Transformation
 ***/
#transformation {
  width: 60px;
  height: 60px;
  background: #fff;
  border-radius: 50%;
  animation: transform 1s ease-in-out infinite alternate;
}
@keyframes transform {
  100% {
    width: 150px;
    border-radius: 4px;
  }
}
/***
 Masking
 ***/
#masking {
  width: 150px;
  height: 60px;
  background: #eaeaea;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4px;
}
#masking span {
  width: 30px;
  height: 30px;
  background: #fff;
  border-radius: 50%;
  animation: transform 1s ease-in-out infinite alternate;
}
@keyframes transform {
  100% {
    width: 150px;
    height: 60px;
    border-radius: 4px;
  }
}
/***
 Parallax
 ***/
#parallax {
  width: 160px;
  height: 90px;
  background: #eaeaea;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4px;
}
#parallax span {
  width: 120px;
  height: 90px;
  background: #fff;
  animation: parallax 1s ease-in-out infinite alternate;
}
@keyframes parallax {
  0% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(20px);
  }
}
/***
 Dimentionality
 ***/
li:nth-child(5) {
  perspective: 400px;
}
#dimension {
  width: 190px;
  height: 60px;
  background: #fff;
  border-radius: 4px;
  animation: dimension 1s ease-in-out infinite alternate;
}
@keyframes dimension {
  100% {
    transform: rotateX(-90deg);
  }
}

</style>
