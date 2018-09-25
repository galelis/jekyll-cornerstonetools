# How to set up the {{page.toolName}} tool:

- Create a cornerstone element
{% highlight html %}
<div class="cornerstone-element" data-index="0" oncontextmenu="return false"></div>
{% endhighlight %}

- Enable the element
{% highlight javascript %}
const element = document.querySelector('.cornerstone-element');
cornerstone.enable(element);
{% endhighlight %}

- Initialize cornerstoneTools v3 and add the enabled elements
{% highlight javascript %}
const cTools = cornerstoneTools.init();
cTools.addEnabledElement(element);
{% endhighlight %}

- Get the apiTool and add the tool into all enabled elements
{% highlight javascript %}
const apiTool = cornerstoneTools.{{page.toolName}}Tool;
cTools.addTool(apiTool);
{% endhighlight %}

## Setting tool mode 
- Activate
{% highlight javascript %}
cTools.setToolActive({{page.toolName}}, options);
{% endhighlight %}

**Options**
* mouseButtonMask (default: 1)

`mouseButtonMask: 0` for no button

`mouseButtonMask: 1` for left button

`mouseButtonMask: 2` for middle button

`mouseButtonMask: 3` for right button

- Passive
{% highlight javascript %}
cTools.setToolPassive({{page.toolName}});
{% endhighlight %}

- Enable
{% highlight javascript %}
cTools.setToolEnable({{page.toolName}});
{% endhighlight %}

- Disable
{% highlight javascript %}
cTools.setToolDisable({{page.toolName}});
{% endhighlight %}