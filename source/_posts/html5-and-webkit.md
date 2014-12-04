title: 谈谈HTML5和webkit
date: 2014-12-03 23:53:41
tags:
---

最近看了豆瓣云音乐码农和和intel朱永盛谈webkit，HTML5的视频，朱永盛的观点主要就是

* webkit跨平台的，所以好好好
* HTML5因为用了webkit，所以好好好

仔细想了一下这个问题，包括他提到未来可能提供一个跨PC(Windows, OS X, Linux), Mobile(Android, iOS)的`WebView`，事实上他们做的这个事情和Adobe的Flash/AIR区别不大：

 * 底层runtime:
 	* web/native => Flash/AIR 
 	* web/native => Browser/WebView
 * 解释器：
 	* avm2
 	* v8 engine
 
现在看，webkit从指标上并没有超过Flash/AIR, canvas渲染，SVG，WebGL各方面超过了吗？我看没有。工具链上webkit更是差得远。技术这个事情上是个占山头的游戏，你Adobe推的东西我不能受制于你，我就是不用，Borland被MS折腾的故事历历在目呢。而webkit不属于任何一个大公司，所以大家都可以支持它，这就是一个妥协的产物。只能用JS写代码真的好吗？HTML去写界面真的好吗？好不好没人关心，它只是妥协的产物。

后面关于webkit跨平台，朱永盛还提到一个问题就是没有一个`官方打包的webkit`，豆瓣的`OneRing`是解决这个问题的，`node-webkit`是解决这个问题的，听说豌豆荚也自己搞了一个`OneRing`修改版解决这个问题，想用webkit做跨平台仍然是相当之麻烦的。`node-webkit`你敢用吗？`OneRing`你敢用吗？狠狠心用了，最后各种问题需要解决，而且安装包贼大。

webkit开源能够让巨头们搭成妥协这是它的优势，但是这使得webkit包含的音视频解码器涉及专利问题迟迟得不到解决，这也是开源的劣势，没娘的孩子嘛。

最后就是，我希望能够有个终结一切的跨平台框架诞生，webkit是最有希望的，但也不代表别的技术没有机会。
