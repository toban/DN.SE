# DAGENS NYHETER (HTTP://WWW.DN.SE)
DN.SE gratis utan paywall

1. Lägg till följande som bokmärke

```javascript
javascript:(function(){
if(window.location.origin.indexOf('dn.se') != -1){
	$("#pwOverlay").remove();
	$(".js-paywall").hide();
	$(".article__premium-content").show();  
	$(".article__body.article__body--mask").removeClass("article__body article__body--mask");
	sessionStorage.setItem('adBlockTracked', 'false');
}else{
	window.location = "https://www.dn.se";
}
})();
```


