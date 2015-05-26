# css3-loading
css3-loading

##css
```css
.loading {position: relative;}
	.loading .r1 , .loading .r2{border: 3px solid black;border-radius: 15px;position: absolute;}
	.loading .r1{ top: 0 ; left: 0; width: 20px;height: 20px;border-left-color: transparent;}
	.loading .r2{ top: 4px ; left:4px ;width: 12px;height: 12px;border-right-color: transparent;}

	.loading .r1{
	 -webkit-animation:r1Animate 1s  ease infinite;
       -moz-animation: r1Animate 1s  ease infinite;
        -ms-animation: r1Animate 1s  ease infinite;
         -o-animation: r1Animate 1s  ease infinite;
            animation: r1Animate 1s  ease infinite;
	}
	.loading .r2{
	 -webkit-animation:r2Animate 0.8s  ease infinite;
       -moz-animation: r2Animate 0.8s  ease infinite;
        -ms-animation: r2Animate 0.8s  ease infinite;
         -o-animation: r2Animate 0.8s  ease infinite;
            animation: r2Animate 0.8s  ease infinite;
	}
	@-webkit-keyframes r1Animate{from{-webkit-transform: rotate(0deg);} to  {-webkit-transform: rotate(360deg);}}
	@-moz-keyframes r1Animate{from{-moz-transform: rotate(0deg);} to  {-moz-transform: rotate(360deg);}}
	@-ms-keyframes r1Animate{from{-ms-transform: rotate(0deg);} to  {-ms-transform: rotate(360deg);}}
	@-o-keyframes r1Animate{from{-o-transform: rotate(0deg);} to  {-o-transform: rotate(360deg);}}
	@keyframes r1Animate{from{transform: rotate(0deg);} to  {transform: rotate(360deg);}}


	@-webkit-keyframes r2Animate{from{-webkit-transform: rotate(0deg);}to  {-webkit-transform: rotate(-360deg);}}
	@-moz-keyframes r2Animate{from{-moz-transform: rotate(0deg);}to  {-moz-transform: rotate(-360deg);}}
	@-ms-keyframes r2Animate{from{-ms-transform: rotate(0deg);}to  {-ms-transform: rotate(-360deg);}}
	@-o-keyframes r2Animate{from{-o-transform: rotate(0deg);}to  {-o-transform: rotate(-360deg);}}
	@keyframes r2Animate{from{transform: rotate(0deg);}to  {transform: rotate(-360deg);}}
```

##html
```html
<div class=loading >
	<div class=r1 ></div>
	<div class=r2 ></div>
</div>
```
