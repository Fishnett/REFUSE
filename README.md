Fatal destination...

Installing Virus...

■■■■■■■■□

95%
Fuck your mind.!
|  ∧∧
|(´･ω･`)Maam Your Pizza Here
|ﾉ _つ つ
|―ｕ’🍕
￣￣￣￣￣￣

System shutdown..haahhaaaa

*/
/* User config */
var msgcount = 1;
var delay = 250;
var emojiTab = 8;	/* There is no 0, from 1 to 6. */
var emojiNumber = Math.floor(Math.random() * 5) + 1  ;	/* No 0 either. */
/* The actual code */
function getElementByXpath(path) { return document.evaluate(path, document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue; }
var winnniey = 0;
function sendMessage() {         
   setTimeout(function () {
	var emojiButton = getElementByXpath('//*[@id="main"]/footer/div/button[1]');
   	emojiButton.click();
   	setTimeout(function () {
	var tab = getElementByXpath('//*[@id="main"]/footer/span/div/div[1]/button[' + emojiTab + ']');
	tab.click();
   	setTimeout(function () {
   		var emoji = getElementByXpath('//*[@id="main"]/footer/span/div/span/div/div/span[' + emojiNumber + ']');
	  	emoji.click();
	  	setTimeout(function () {
		  	var sendButton = getElementByXpath('//*[@id="main"]/footer/div/button[2]');
			sendButton.click();  
			setTimeout(function () {
			    winnniey++;        
			    if (winnniey < msgcount) {
			    	sendMessage();   
			    }
		    }, delay);
		}, delay);
    }, delay);
   }, delay);
  }, delay);
}
sendMessage();
