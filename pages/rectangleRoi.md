---
layout: page
title: RectangleRoi Tool
toolName: rectangleRoi
htmlFile: simpleTool.html
permalink: /rectangleRoi/
---

How to set up the {{page.toolName}} tool:

{% highlight javascript %}
const cTools = cornerstoneTools.init({});
cTools.addTool('{{page.toolName}}')
{% endhighlight %}
