
<h1>What is jquery.preloaders.js</h1>
<p>
    jquery.preloaders.js is a lightweight jQuery plugin that helps you create an animated spinner while the ajax content is loading.
</p>
<h3>Check out the <a href="http://ebenites.github.io/jquery.preloaders.js/index.html" target="_blank">Demo</a></h3>
<h1>Install by Bower</h1>
<p>jquery.preloaders.js is available as a Bower package. Just run</p>
<pre>bower install jquery.preloaders.js</pre>

<h1>1. Include Folowing Libraries</h1>
<p>JQuery reference and the jquery.preloaders.js</p>
<pre>
<p>&lt;script src="https://code.jquery.com/jquery-3.3.1.min.js"&gt;</p><p>&lt;script src="bower_components/jquery.preloaders.js/jquery.preloaders.min.js"&gt;</p>
</pre>

<h1>2. Basic Initialize</h1>
<p>Start loading</p>
<pre>
<code>
    &lt;script type="text/javascript"&gt;
        $.preloader.start({modal: true});
    &lt;/script&gt;
</code>
</pre>
<p>Stop loading</p>
<pre>
<code>
    &lt;script type="text/javascript"&gt;
        $.preloader.stop();
    &lt;/script&gt;
</code>
</pre>

<h1>3. Others Options</h1>
<pre>
<code>
    &lt;script type="text/javascript"&gt;
        var e = $('#loader').preloader({src:'sprites.png', frames:8, width:64, height:64, speed:9, className: 'mycss'}); // src: (in js/jquery/preloaders/img path)
        // var e = $('#loader').preloader('stop');
    &lt;/script&gt;
</code>

<code>
    &lt;script type="text/javascript"&gt;
        $.preloader.start({modal: true, position:'top-right'}); // position: [(default:'center') | 'top-left' | 'top-right' | ' bottom-left' | 'bottom-right' | {top:'200px', left:'200px'}]
        // $.preloader.stop();
    &lt;/script&gt;
</code>

<code>
    &lt;script type="text/javascript"&gt;
        var e = $('&lt;div/&gt;').css('margin', '0 auto').insertAfter($('#conteiner')).preloader(); // center into a 'container'
        // e.preloader('stop');
    &lt;/script&gt;
</code>

<code>
    &lt;script type="text/javascript"&gt;
        var e = $('&lt;div/&gt;').css({'margin-left': '8px', 'display': 'inline-block', 'vertical-align': 'middle'}).insertAfter($('#button')).preloader({src:'sprites.32.png'});   // next to a 'button'
        // e.preloader('stop');
    &lt;/script&gt;
</code>
</pre>
