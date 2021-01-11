# Code 201, 11th Jan, Read 12
# Chart.js API 
So basiclly the framework is code written by someone else and you can use it so you don't need to write you hole program from scratch.
API is the acronym for Application Programming Interface, which is a software intermediary that allows two applications to talk to each other. Each time you use an app like Facebook, send an instant message, or check the weather on your phone, you’re using an API.

Chart.js is a framework that allow you to visulaize data far better than using table.and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.
![chart](https://cdn.mos.cms.futurecdn.net/S5bicwPe8vbP9nt3iwAwwi.jpg)

you need also to read docs for chart js to know how to use all features
her an examples:
```javascript
var myLineChart = new Chart(ctx, {
    type: 'line',
    data: data,
    options: options
});
```
I don't know how install it but here is some link you can download  Chart.js from the [GitHub releases](https://github.com/chartjs/Chart.js/releases/latest) or use a [Chart.js CDN](https://www.jsdelivr.com/package/npm/chart.js). Detailed installation instructions can be found on the [installation](https://www.chartjs.org/docs/latest/getting-started/installation.html) page.

## Canvas API 

The **Canvas API** provides a means for drawing graphics via [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) and the [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)  [`<canvas>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/canvas) element. Among other things, it can be used for animation, game graphics, data visualization, photo manipulation, and real-time video processing.
![](https://wersm.com/wp-content/uploads/2017/04/Screen-Shot-2017-03-31-at-3.56.40-PM-1024x598-1024x598.jpg)

example
```html
<canvas id="tutorial" width="150" height="150"></canvas>
```

```css
ctx.fillStyle = 'orange';
ctx.fillStyle = '#FFA500';
ctx.fillStyle = 'rgb(255, 165, 0)';
ctx.fillStyle = 'rgba(255, 165, 0, 1)';
```

[My GitHub Page](https://omar-tarawneh.github.io/reading-notes/class-12)