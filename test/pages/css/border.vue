<template>
  <scroller>
    <div class="container">
        <text class="radius box solid"></text>
        <text class="topleft box solid"></text>
        <text class="topright box solid"></text>
        <text class="bottomleft box solid"></text>
        <text class="bottomright box solid"></text>
        <text>solid</text>
    </div>
    <div class="container">
        <text class="radius box dotted"></text>
        <text class="topleft box dotted"></text>
        <text class="topright box dotted"></text>
        <text class="bottomleft box dotted"></text>
        <text class="bottomright box dotted"></text>
        <text class="box dotted dottedLarge"></text>
        <text>dotted</text>
    </div>
    <div class="container">
        <text class="radius box dashed"></text>
        <text class="topleft box dashed"></text>
        <text class="topright box dashed"></text>
        <text class="bottomleft box dashed"></text>
        <text class="bottomright box dashed"></text>
        <text class="box dashed dashedLarge"></text>
        <text>dashed</text>
    </div>
    <div class="container">
        <text class="constrained1"></text>
        <text class="constrained2"></text>
        <text class="constrained1 dashed"></text>
        <text class="constrained2 dashed" ></text>
        <text class="constrained1 dotted" ></text>
        <text class="constrained2 dotted" ></text>
        <text>constrained</text>
    </div>
    <div class="container">
        <text class="box radius differentWidth1"></text>
        <text class="box radius differentWidth2"></text>
        <text class="box radius differentWidth3"></text>
        <text class="box radius differentWidth4" ></text>
        <text class="box radius differentWidth5" ></text>
        <text>different width</text>
    </div>
     <div class="container">
        <text class="box borderClipping1"></text>
        <text class="box borderClipping2"></text>
        <text class="box borderClipping3"></text>
        <text>border clipping</text>
    </div>
    <div class="container">
        <text class="boxShadow1"></text>
        <text class="boxShadow2"></text>
        <text test-id="test-text">box shadow</text>
    </div>
    <div class="container">
        <text class="circle transparent1"></text>
        <text class="circle transparent2"></text>
        <text class="circle transparent3"></text>
        <text class="circle transparent4"></text>
        <text>transparent</text>
    </div>
    <div class="container">
        <image class="box topleft" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <image class="box topright" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <image class="box bottomleft" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <image class="box bottomright" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <image class="box" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <image class="circle" src="https://gw.alicdn.com/tps/TB1EP9bPFXXXXbpXVXXXXXXXXXX-150-110.jpg"></image>
        <text>image</text>
    </div>
  </scroller>
</template>

<style>
.container {
  flex-direction: row;
}
.box {
  width: 100px;
  height: 100px;
  margin: 2px;
  background-color: #ccc;
  border-width: 6px;
  border-color: #f00;
}
/* the different border-radii styles defined in CSS3 */
.radius {
  border-radius: 20px;
}
.topleft {
  border-top-left-radius: 20px; 
}
.topright {
  border-top-right-radius: 20px; 
}
.bottomright {
  border-bottom-right-radius: 20px; 
}
.bottomleft {
  border-bottom-left-radius: 20px; 
}
.dottedLarge {
  border-width: 21px;
  border-radius: 40px;
  border-left-color: rgba(0,0,255,1);
  border-bottom-color: rgba(0,128,0,0.5);
  border-right-color: rgba(0,128,0,0.5);
}
.dashedLarge {
  border-top-width: 19px;
  border-bottom-width: 19px;
  border-left-width: 38px;
  border-right-width: 38px;
  border-top-left-radius: 50px;
  border-top-right-radius: 50px;
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
  border-left-color: rgba(0,0,255,1);
}

/* the different border styles defined in CSS3 */
.dotted { 
  border-style: dotted;
}
.dashed {
  border-style: dashed;
}
.solid {
  border-style: solid;
}

.constrained1 {
  width: 100px;
  height: 40px;
  border-width: 10px ;
  border-color: #f00;
  border-top-left-radius: 15px;
  border-top-right-radius: 40px;
  border-bottom-left-radius: 40px;
  border-bottom-right-radius: 15px;
}
    
.constrained2 {
  width: 40px;
  height: 100px;
  margin-left: 10px;
  border-width: 10px ;
  border-color: #f00;
  border-top-left-radius: 15px;
  border-top-right-radius: 40px;
  border-bottom-left-radius: 40px;
  border-bottom-right-radius: 15px;
}

.differentWidth1
{
  border-top-width: 10px;
  border-right-width: 15px;
  border-bottom-width: 20px;
  border-left-width: 30px;
}
.differentWidth2
{
  border-top-width: 10px;
  border-right-width: 25px;
  border-bottom-width: 40px;
  border-left-width: 25px;
}
.differentWidth3
{
  border-top-width: 10px;
  border-right-width: 25px;
  border-bottom-width: 10px;
  border-left-width: 25px;
}
.differentWidth4
{
  border-top-width: 16px;
  border-right-width: 4px;
  border-bottom-width: 110px;
  border-left-width: 32px;
}
.differentWidth5
{
  border-right-width: 50px;
}

.borderClipping1 {
  border-radius: 30px;
  border-top-color: red;
  border-top-width: 10px;
  border-left-color: blue;
  border-left-width: 10px;
  border-right-color: green;
  border-right-width: 30px;
  border-bottom-color: yellow;
  border-bottom-width: 30px;
}
.borderClipping2 {
  border: solid rgba(255,0,0,1);
  border-top-width: 20px;
  border-bottom-width: 20px;
  border-left-width: 40px;
  border-right-width: 40px;
  border-top-left-radius: 50px;
  border-top-right-radius: 50px;
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
  border-left-color: rgba(0,0,255,1);
  border-bottom-color: rgba(0,128,0,0.5);
  border-right-color: rgba(0,128,0,0.5);
}   
.borderClipping3 {
  border-width:10px;
  border-radius: 50px;
  border-top-right-radius: 0px;
  border-bottom-left-radius: 0px;
  border-left-color: rgba(0,0,255,1);
  background-color: green;
  border-top-width: 5px;
  border-bottom-width: 5px;
  border-left-width: 18px;
  border-right-width: 0px;
}

.boxShadow1 {
  width: 100px;
  height: 45px;
  background-color: #000000;
  border-top-left-radius: 30px;
  border-top-right-radius: 30px;
  box-shadow: 0px 0px 1px 1px #000000;
  margin-top: 20px;
}
.boxShadow2 {
  width: 100px;
  height: 45px;
  background-color: #000000;
  box-shadow: 30px 15px 0px -10px lime;
  border-bottom-right-radius: 50px;
  margin:30px;
}

.circle {
  width: 100px;
  height: 100px;
  border-width: 33px;
  border-color: rgba(255, 0, 0, 0.5);
  border-style: solid;
  border-radius:50px;
}
.transparent1 {
  border-right-color: transparent;
}
.transparent2 {
  border-right-color: transparent; 
  border-right-width: 33px;
}
.transparent3 {
  border-right-color: transparent; 
  border-right-width: 0;
  border-bottom-color: transparent;
  border-bottom-width: 0;
}
.transparent4 {
  border-right-color: transparent; 
  border-right-width: 0;
  border-bottom-color: transparent;
}
</style>

<script>
  module.exports = {
    data : function(){
      return {
      }
    },
    methods : {
    }
  }
</script>