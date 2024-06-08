# Add browser version guard by default(as an aside)

* User-Agent文字列を用いたブラウザーの判定をやるのは今どうなのか
* mdnはもっと良い方法があるよね、というスタンス
  * [Browser detection using the user agent \- HTTP \| MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Browser_detection_using_the_user_agent)
*  User-Agent Client Hints APIもあるが…
  * [User\-Agent Client Hints API \- Web APIs \| MDN](https://developer.mozilla.org/en-US/docs/Web/API/User-Agent_Client_Hints_API)
* 現実的にはまだUser-Agentに頼るしか無いか、という印象
  * 参考：[UserAgentに依存した分岐を捨てられるか \(または何故捨てられていないのか\) \- Speaker Deck](https://speakerdeck.com/pastak/useragentniyi-cun-sitafen-qi-woshe-terareruka-matahahe-gu-she-terareteinainoka)
