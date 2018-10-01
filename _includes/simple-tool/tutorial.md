# How to set up the {{page.toolName}} tool:

- HTML:
{% highlight html %}
{% include simple-tool/elements-html.html %}
{% endhighlight %}

- Javascript:
{% highlight javascript %}
const csTools = cornerstoneTools.init();
const LengthTool = cornerstoneTools.LengthTool;

// Make sure we have at least one element enabled
const element = document.querySelector("#element-1");
cornerstone.enable(element);

// Adds tool to ALL currently enabledElements
csTools.addTool(LengthTool);

// OR add the tool to a specific enabledElement
csTools.addToolForElement(element, LengthTool);
{% endhighlight %}

## Setting tool mode 
- Activate an added tool:
{% highlight javascript %}
// Activate the tool for ALL currently enabledElements
csTools.setToolActive(LengthTool.name, { mouseButtonMask: 1 });

// OR activate the tool for a specific enabledElement
csTools.setToolActiveForElement(enabledElement, LengthTool.name, {
  mouseButtonMask: 1
});
{% endhighlight %}
