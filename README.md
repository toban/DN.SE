# DAGENS NYHETER (HTTP://WWW.DN.SE)
DN.SE gratis utan paywall

1. Encoda(https://mrcoles.com/bookmarklet/) och lägg till följande javascript som bokmärke

```javascript
javascript:(function(){
if(window.location.origin.indexOf('dn.se') != -1){
	$("#pwOverlay").remove();
	$(".js-paywall").hide();
	$(".article__premium-content").show();  
	$(".article__body.article__body--mask").removeClass("article__body article__body--mask");
	sessionStorage.setItem('adBlockTracked', 'false');
	$(".modal.takeover-modal").remove();
	$(".modal.takeover-modal.test-a").remove();
	$(".gdpr-header").remove();
}else{
	window.location = "https://www.dn.se";
}
})();
```


