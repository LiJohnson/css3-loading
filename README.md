# css3-loading
css3-loading

## css
```css
.loading {
	position: relative;
}
.loading:before, .loading:after {
	position: absolute;
	content: ' ';
	display: block;
	border: 1.8px solid #888888;
	border-radius: 50%;
}
.loading:before {
	top: 0;
	left: 0;
	width: 12px;
	height: 12px;
	border-left-color: transparent;
}
.loading:after {
	top: 2.4px;
	left: 2.4px;
	width: 7.2px;
	height: 7.2px;
	border-right-color: transparent;
}
.loading:before {
	-webkit-animation: r1Animate 1s ease infinite;
	-moz-animation: r1Animate 1s ease infinite;
	-ms-animation: r1Animate 1s ease infinite;
	-o-animation: r1Animate 1s ease infinite;
	animation: r1Animate 1s ease infinite;
}
.loading:after {
	-webkit-animation: r2Animate 0.8s ease infinite;
	-moz-animation: r2Animate 0.8s ease infinite;
	-ms-animation: r2Animate 0.8s ease infinite;
	-o-animation: r2Animate 0.8s ease infinite;
	animation: r2Animate 0.8s ease infinite;
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

## less
```css
.loading {
	@width:12px;
	@color:#888;
	@speed:1s;
	position: relative;
	&:before,&:after{
		position: absolute;
		content:' ';
		display: block;
		border: @width*0.15 solid @color;
		border-radius: 50%;
	}
	&:before{ 
		top: 0 ;
		left: 0;
		width: @width;
		height: @width;
		border-left-color: transparent;
	}
	&:after{ 
		top: @width*0.2 ;
		left:@width*0.2 ;
		width:@width*0.6;
		height:@width*0.6;
		border-right-color: transparent;
	}
 
	&:before{
	-webkit-animation: r1Animate @speed ease infinite;
	   -moz-animation: r1Animate @speed ease infinite;
		-ms-animation: r1Animate @speed ease infinite;
		 -o-animation: r1Animate @speed ease infinite;
			animation: r1Animate @speed ease infinite;
	}

	&:after{
	-webkit-animation: r2Animate @speed*0.8 ease infinite;
	   -moz-animation: r2Animate @speed*0.8 ease infinite;
		-ms-animation: r2Animate @speed*0.8 ease infinite;
		 -o-animation: r2Animate @speed*0.8 ease infinite;
			animation: r2Animate @speed*0.8 ease infinite;
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
}
```

##html
```html
<div class=loading ></div>
```
