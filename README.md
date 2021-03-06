###Speed Maths library####

This is a library for faster math functions execution in Javascript. It only implements sine and cosine for now.

It revolves around approximation and cached values, meaning that if you need precise results, you should not use this library. But if you want faster calculation where you can afford results that are a bit off, you can go with that.

[JSPerf test](http://jsperf.com/smath-test/4) We get something around +400% speed in Chrome, which is nice.

![jsperf_results.png](http://Malharhak.github.io/smath.js/assets/jsperf.png)

###Usage###

``` javascript
var sMath = new SMath();

var angle = Math.PI;
sMath.cos(angle);
sMath.sin(angle);
```

###Difference in results###
To get an idea of the difference in results between the native functions and the cached ones, you can run the index page which takes 100 random angles and shows the difference in result in the console. It also outputs a canvas circle with blue dots so you can visualize the granularity of the approximation
