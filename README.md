# Fill-Between-Lines
Using D3.js to fill areas between lines in C3.js, works for subchart, resize and chart click possible even handling. 
There are two examples, one bisic simple example and one applied example.
[Basic]
A live demo could be found at: [fiddle demo](https://jsfiddle.net/Mandyzhu7/1xnc6y58/9/)
![Alt text](/images/basic.PNG "simple chart")

[Applied]
Whenever a resize or filetering from the subchart happens, the areas are needed to be removed and redraw. 
Data point displays different color based on the status (or else can be purely calculated as stated below in Note)

Note:
1. The calculation of the point color can be done using the data as well instead of using the status in this case. 
2. In order to enbale the click event, to redirect to the url where the point/closes point resides, a baseurl is needed and the commented out lines regarding this should be uncommented. 
```javascript
location.href = findNearestValueByKey(urldict, xValue);
```

![Alt text](/images/applied.PNG "applied chart")

