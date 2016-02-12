---
layout: main
title: "Create a blog post using Jekyll 3.1.1"
Keywords: Jekyll3, Blog, Create, Front matter
---

<div class="container">
<h1> {{ page.title }} </h1>

{% include sbutts.html %}

<p>Welcome to our page. In this very first blog-post you will learn how to create a blog-post using Jekyll 3.1.1</p>

<p>Jekyll is a powerful static website generator! It has loads of features that make it very usable.</p>
<p>Assuming, Jekyll is installed you must navigate to _posts folder and create a file that looks like this:</p>

<pre>
---
layout: main
title: "Create a blog post using Jekyll 3.1.1"
Keywords: Jekyll3, Blog, Create

I love you more than LoLlYpOp! Yummy! <3

---
</pre>

<p>Jekyll uses a front matter to define YAML content. Begin and end your page with three dashes(---) and define variables.</p>
<p>Below the Front matter block write anything you love to post. That's it! Now issues a jekyll serve and you'll have a web-page. Assuming you have many posts, you'll use a for loop to iterate through them using the url attribute available in the posts global variable as seen below.</p>

<pre>
		  { % for post in site.posts % }
		      Loop through whatever you need here ... post.url or post.keywords etc
		  { % endfor % }
</pre>

<p>Note: Do not use a space between the { and % symbols. In this case, I've put a space intentionally.</p>

<p>That's how you create a post in Jekyll. If you did not follow along, don't worry. :) Check the video below.</p>

<h2>Video: Creating a blog post in Jekyll</h2>
<h4>Coming soon.</h4>
{{page.Keywords}}

</div>