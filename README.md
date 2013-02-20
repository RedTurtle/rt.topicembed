rt.topicembed introduction
==========================

This product add's new tab to the topic content type called `embed`, and
publish topic's items similar to **twitter** widget.


Embed
-----

This is practically a simple form that allows user to configure a web widget.
The code can be found in the `textarea` in the same view. An example code
looks like that:

```html
<script>
    (function() {
        var s = document.createElement('script');
        s.src = 'http://nohost/plone/events/embed.js';
        s.async = true;
        window.topic_options = (window.topic_options || []).concat([ { element_id: 'embeded_id', elements_length: 5, embed_css: true, new_window: true }]);
        document.body.appendChild(s);
    }());
</script>
```


This code can be later embeded on the external site, the same as **twitter** widget.
