---
layout: page
title: Project1
permalink: docs/project1/
nav_order: 1
has_children: true
---


# Das ist Projekt Nr. 1
{: .no_toc }

Hier eine Einleitung 

---

{% capture code_fence %}
```js
// Javascript code with syntax highlighting in fences
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```
{% endcapture %}
{% assign code_fence = code_fence | markdownify %}
{% include fix_linenos.html code=code_fence %}

{% capture code %}
{% highlight ruby linenos %}
# Ruby code with syntax highlighting and fixed line numbers using Liquid
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
{% endhighlight %}
{% endcapture %}
{% include fix_linenos.html code=code %}
{% assign code = nil %}

{% capture code_fence %}
```bash
cd /path/to
git clone https://github.com/openframeworks/openFrameworks.git
cd /path/to/OF/scripts/{DISTRO}/
sudo ./install_dependencies.sh
sudo ./install_codecs.sh
cd ../linux/
# Compile OpenFrameworks
sudo ./compileOF.sh -j2 
# Compile projectgenerator
sudo ./compilePG.sh 
```
{% endcapture %}
{% assign code_fence = code_fence | markdownify %}
{% include fix_linenos.html code=code_fence %}




