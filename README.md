# fullScreen
This is a plugin for fullScreen, supports Chrome, Firefox, and IE11+;   

# How to use?   

$("#dom").fullScreen();it has three params, 			   
                        'background'      : '#000',</br>
			'callback'        : function(isFullScreen),</br>
			'fullscreenClass' : 'fullScreen'</br>
user callback function to add aditional actions, background to set the background color when in fullScreen,</br>
user #dom.fullScreen to custom your own style in fullScreen, the added css style will disappear when exit fullScreen;</br>
example:</br>
		$("#mainLayout").fullScreen({</br>
			'callback' : function(isFullScreen){</br>
				if(!isFullScreen){</br>
					$("#text").text("全屏");</br>
				}else{</br>
					$("#text").text("退出");</br>
				}</br>
			}</br>
		});</br>
in css file:</br>
##mainLayout.fullScreen .text{</br>
	height: 265px;</br>
}</br>
