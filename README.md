jekyll-fluidbox
===============

Jekyll plugin to make figures work with the fluidbox jQuery

## Requirements

* [Nokogiri](http://nokogiri.org/), should be part of the standard Jekyll install
* [Fluidbox](http://terrymun.github.io/Fluidbox/)

To install Fluidbox for your Jekyll blog, add the following files:

```
js
  imagesloaded.pkgd.min.js
  jquery.fluidbox.min.js
_assets
  stylesheets
    fluidbox.css
```

And put the following into `layouts/default.html` (the paths might be different depending on your Jekyll setup):

```
<link href="assets/fluidbox.css" media="all" rel="stylesheet" type="text/css" />

<script src="/js/imagesloaded.pkgd.min.js"></script>
<script src="/js/jquery.fluidbox.min.js"></script>
<script type='text/javascript'>
  $(function () {
    $("a").fluidbox();
  });
</script>
```

## License

See [LICENSE](LICENSE).