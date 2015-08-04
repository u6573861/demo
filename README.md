# demo
<!DOCTYPE html>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0,user-scalable=0,minimum-scale=1.0, maximum-scale=1.0">
<meta content="telephone=no" name="format-detection">
<title>帮5买触屏版手机wap淘宝客购物网站模板下载</title>
</head>
<body>

<div id="213" ng-app="" ng-controller="namesController" style="display:none"> 

<p>循环对象:</p>
<ul>
	<div ng-repeat="x in names">
	<a href="#" ng-click="saidey(x.xunha)" >
		<div style="color:red">姓名：{{ x.name}}</div>
		<div><img width="100%" src="http://img1.40017.cn/touch/pushcode/maerfu/daimay_13.jpg"></div>
		<div>价格：{{x.jiage }}</div>
		<div><a href="{{x.lianje }}">lianjie：{{x.jiage }}</a></div>
	</a>
	</div>
</ul>

</div>

<script src="http://www.runoob.com/try/angularjs/1.2.5/angular.min.js"></script>
<script type="text/javascript" src="http://js.40017.cn/cn/min/??/touch/app/public/zepto.20140624.js"></script>
<script src="http://js.40017.cn/cn/min/??/touch/hb/c/bridge.1.1.0.js?v=33261316"></script>
<script src="http://js.40017.cn/touch/pushcode/record.js?v=332"></script>


<script>
function namesController($scope) {
    $scope.names = [
        {name:'Jani',country:'Norway',jiage:'1',xunha:'params1',lianje:'http://m.ly.com'},
        {name:'Hege',country:'Sweden',jiage:'2',xunha:'params2',lianje:'http://m.ly.com'},
        {name:'Kai',country:'Denmark',jiage:'3',xunha:'params3',lianje:'http://m.ly.com'},
		{name:'1Hege',country:'Sweden',jiage:'21',xunha:'params1',lianje:'http://m.ly.com'},
		{name:'2Hege',country:'Sweden',jiage:'22',xunha:'params1',lianje:'http://m.ly.com'},
		{name:'3Hege',country:'Sweden',jiage:'22',lianje:'http://m.ly.com'},
    ];
	$scope.saidey = function (params) {  
			alert(params);
			var str = JSON.stringify(params);  
var str1 = JSON.parse(str); 
			alert(str1); 
			window._tc_bridge_util.set_event(params1); 
			alert(str1);
        } 
	document.getElementById("213").style.display="block";
}
</script>
</body>
</html>
		
