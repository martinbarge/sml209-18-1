<h1>HTML and CSS Part 1</h1>
<h2>1. Making Images Clickable</h2>
<p>Sometimes it can be helpful for your page visitors to view images in a larger window. This can be done by adding a <code> &lt;a href=&gt; </code> tag around the image. This is also useful if you want an image to link to another website or page in your own website.<p>
<p>Here is an example of an image from Wikipedia that is now clickable</p>
<p>
<a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source">
<img src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"></a>
</p>
<div class="clearLeft"></div>

<p>Ths code for this is:</p>
<code>
&lt;a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source"&gt;
  
  
&lt;img  src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"&gt;


&lt;/a&gt;
</code>
<p>Look at the above lines of code carefully. Notice the order in which the tags are placed:</p> 

<ol>
<li>We open the familiar link tag: <code> &lt;a href=&gt; </code> and include the URL of the image source. Notice also that we can add a <code> title= </code> attribute to the tag. The title attribute specifies text that appears over the image when the user hovers their mouse on the image.</li>
<li>Next, we have the familiar image tag: <code> &lt;img src=&gt; </code>. You will notice that in this case the URL to the image is the same as in the href tag.</li>
<li>Finally, we must close the <code> &lt;/a&gt; </code> tag.</li>
</ol>

<h2>2. Changing the size of the image on the page.</h2>
<p>Sometimes we might want our image to occupy less space on the page. This can be done by adding a style attribute to the tag.</p>
<p>Here is an example of a simple style attribute added to the image tag that specifies the image to occupy only 70% of the width of the page content area: <code> &lt;a style="width:70%;"&gt; </code>.</p>

<p>In the example above, the word 'width' is known as a style 'property', and the number '70%' is called the 'value'. The Mozilla Developer Network provides a <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#Keyword_index">full reference for all possible style properties</a>. But you don't need to worry about learning them all! Just a few are useful for our purposes.</p>
<p>We can add other properties and values to our style entry. For example: <code> &lt;a style="width:70%; border:1px solid green;"&gt; </code>. Adding the 'border' property specifies a border around the image. In this example, the border property is followed by 3 values: <code> 1px solid green </code>. This means the border will be a solid green line, one pixel thick.</p>
<p>So the full code for our image tag would now look like this:</p>
<code> 
&lt;img class="imgLeft" style="width:70%; border:1px solid green;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe" &gt;
</code>
<p>And the result is this:</p>
<a href="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" title="View Image Source">
<img class="imgLeft" style="width:70%; border:1px solid green;" src="https://upload.wikimedia.org/wikipedia/commons/3/39/Europe_biogeography_countries.svg" alt="image of biogeography of Europe"></a>
