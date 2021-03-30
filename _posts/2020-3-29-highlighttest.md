---
layout: page
title: HTML CSS JS
---
JavaScript

{% highlight javascript %}
document.write("JavaScript is a simple language for javatpoint learners");
{% endhighlight %}

HTML
{% highlight html %}
<input type="checkbox" class="openMenu" id="openMenu"/>
  <label for="openMenu" class="ToggleIcon">
    <div class="spinner diagonal part-1"></div>
    <div class="spinner horizontal"></div>
    <div class="spinner diagonal part-2"></div>
</label>
{% endhighlight %}

CSS
{% highlight css %}
/* Toggle Icon Burger) */
.ToggleIcon {
  transition: all 0.3s;
  box-sizing: border-box;
  cursor: pointer;
  position: absolute;
  z-index: 99;
  height: 100%;
  width: 100%;
  top: 27px; /* jarak icon burger dari atas */
  right: 27px;  /* jarak icon burger dari kanan */
  height: 22px; /* sesuaikan ukuran */
  width: 22px;	
}
.spinner {
  transition: all 0.3s;
  box-sizing: border-box;
  position: absolute;
  height: 3px;
  width: 100%;
  background-color: #fff;
  display:block;
}
.horizontal {
  transition: all 0.3s;
  box-sizing: border-box;
  position: relative;
  float: left;
  margin-top: 3px;
}
.diagonal.part-1 {
  position: relative;
  transition: all 0.3s;
  box-sizing: border-box;
  float: left;
}
.diagonal.part-2 {
  transition: all 0.3s;
  box-sizing: border-box;
  position: relative;
  float: left;
  margin-top: 3px;
}
{% endhighlight %}


