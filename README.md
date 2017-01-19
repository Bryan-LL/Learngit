# fullScreen
This is a plugin for fullScreen, supports Chrome, Firefox, and IE11+;

# How to use?

$("#dom").fullScreen();it has three params, 			
            'background'      : '#000',
			'callback'        : function(isFullScreen),
			'fullscreenClass' : 'fullScreen'
user callback function to add aditional actions, background to set the background color when in fullScreen,
user #dom.fullScreen to custom your own style in fullScreen, the added css style will disappear when exit fullScreen;
example:
		$("#mainLayout").fullScreen({
			'callback' : function(isFullScreen){
				if(!isFullScreen){
					$("#text").text("全屏");
				}else{
					$("#text").text("退出");
				}
			}
		});
in css file:
#mainLayout.fullScreen .text{
	height: 265px;
}
