# ng-im-cr

![Альтернативный текст](https://pp.vk.me/c623729/v623729947/3982b/hl1AfInvwvA.jpg)
![Альтернативный текст](https://pp.vk.me/c623729/v623729947/39832/mmF_Wfc3IEw.jpg)


```sh
    .config(["cropFactoryProvider", function (cropFactoryProvider) {
 			 cropFactoryProvider.colorOutline("#000");
 			 cropFactoryProvider.colorCircleFill("#000");

 			 cropFactoryProvider.setResImgSize(1000);
 			 cropFactoryProvider.setResImgFormat("image/png");
 			 cropFactoryProvider.setsetAreaMinSize(200);
 			 cropFactoryProvider.setResultImageQuality(1);
 		     cropFactoryProvider.setChangeOnFly(true);

 			 cropFactoryProvider.setresizeCtrlBaseRadius(8);	
 			 cropFactoryProvider.setresizeCtrlNormalRatio(8);
             cropFactoryProvider.setresizeCtrlHoverRatioSet(8);
   	         cropFactoryProvider.seticonMoveNormalRatioSet(8);
   	         cropFactoryProvider.seticonMoveHoverRatioSet(8);

   	         cropFactoryProvider.setboxResizeBaseSize(4);
   	        cropFactoryProvider.setboxResizeNormalRatio(4);
   	         cropFactoryProvider.setboxResizeHoverRatio(4);
   	         cropFactoryProvider.seticonMoveNormalRatio(4);
   	         cropFactoryProvider.seticonMoveHoverRatio(4);
   		 }])
```
or in controller
```sh
.controller('Ctrl', function($scope, cropFactory) {
      	$scope.changeOnFly=false;
        $scope.resultImageQuality=1;
        $scope.selMinSize=100;
    	$scope.resultImageSize=200;
  	    $scope.resultImageFormat="image/png"
        $scope.colorset={
    	 Outline: "#fff",
    	 BoxStroke: "#000",
   	     BoxFill: "#000",
  	     boxArrowFill: "#000",
         CircleStroke: "#000",
         CircleFill: "#fff",
         IconFill: "#000"
  }
  ```
    and  in  index
```sh

  <img-crop image="imageDataURI"
              result-image="$parent.resImageDataURI"
              area-type="{{type}}" 
              aspect-ratio="aspectRatio"
			  options="obj" 
		      result-image-size="resultImageSize"
			  result-image-format="resultImageFormat"
			  area-min-size="selMinSize"
			  result-image-quality="resultImageQuality"
			  change-on-fly="changeOnFly"				                 
	          on-load-begin="onLoadBegin()"
	          on-load-done="onLoadDone()"
	          on-load-error="onLoadError()"
    ></img-crop>
```





