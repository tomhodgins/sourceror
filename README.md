# Sourceror

Sourceror lets you view the source code of web pages, adding a way to view source in browsers that don't include a native 'View Source' feature.

It works by loading the site using a single-line PHP proxy, then it displays the source code of the website it loads on the page with syntax highlighting and an easy-to-read font, Source Code Pro.

## How to use Sourceror

There are two ways to use Sourceror. I have a copy installed at [http://caduceus.io/inspect](http://caduceus.io/inspect). If I wanted to view the source code I could append it to the URL after a `?` character, like this:

[http://caduceus.io/inspect?https://github.com/tomhodgins/sourceror](http://caduceus.io/inspect?https://github.com/tomhodgins/sourceror)

The second way to use Sourceror is by adding a bookmark to your browser (of any page) and then editing the bookmark and replacing the URL with:

```
javascript:(function(){window.open('http://caduceus.io/inspect?'+window.location.href)})();
```

If you are hosting your own version of the script, you'll want to replace the reference to `http://caduceus.io` with your own domain.

## Why to use Sourceror

This tool can be used in conjunction with [SpeedTest](http://staticresource.com/speedtest.html) to carry out responsive testing right on mobile devices.