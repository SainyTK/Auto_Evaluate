# Auto_Evaluate

for(var i of document.getElementsByTagName("input"))
{
	r = Math.floor(Math.random()*2+4);
	r==i.value&&"radio"==i.type&&0==i.checked&&(i.checked=!0),
	"submit"==i.type&&new RegExp("next|submit","i").test(i.name)&&(i.type="text");
}
	document.getElementsByTagName("form")[0].submit();
