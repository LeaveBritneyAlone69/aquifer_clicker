## What does Aquifer Clicker do? 
### Aquifer Clicker will automatically click through your aquifer quizzes 


## Steps to Install
### 1) Get [ViolentMonkey](https://violentmonkey.github.io/) Extension for Firefox. It will not work on Google Chrome or Edge.  
### 2) Following the [guide](https://violentmonkey.github.io/guide/creating-a-userscript/) on the violentmonkey website, create a new extension and copy the code below in. Be sure to save it. 

```javascript 
// ==UserScript==
// @name        aquifer script
// @namespace   aquifer script
// @match       https://*.meduapp.com/quiz_item_responses/*
// @grant       none
// @version     1.0
// @author      joe
// @description this script will auto click through aquifer quizzes
// ==/UserScript==

const waitForAngular = () => {
  el1 = document.getElementById("quiz_item_response_answer_index_0")
  el2 = document.getElementById("btn1")
  el3 = document.getElementsByClassName("aq-button-2")[1]
  // el4 = document.getElementsByClassName("next-question")[0]
  console.log('here')
  if(el1) {
    el1.click()
    el2.click()
    el3.click()
  }

  setTimeout(waitForAngular, 1000)
}
waitForAngular()
```
### 3) All you have to do is click the "Let's Get Started" button on aquifer to begin the quiz and the rest is handled for you:
<img width="1186" height="306" alt="image" src="https://github.com/user-attachments/assets/856a48ae-04e7-4550-9463-56da6698908f" />

### Enjoy the 30+ minutes you will save each rotation

 
