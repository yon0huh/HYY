# ie8Gallery with jQuery

A very simple jQuery gallery plugin, supported by Internet Explorer 8.

>use jQuery 1.9.1 (cause of Internet Explorer 8)

## Example for initialization and options

### Javascript part
```
<script type="text/javascript">  
    $(document).ready(function(){
        // change classnames (this block is optional)
        $('.thumbs').ie8Gallery({
            thumbs:         '.thumbs',          // classname for thumbnail container
            thumb:          '.thumb',           // classname for thumbnails
            galleryImage:   '.galleryimage',    // classname for the gallery image
            underlay:       '.underlay',        // classname for underlay
            overlay:        '.overlay',         // classname for overlay
            btnPrev:        '.prev',            // classname for previous button
            btnNext:        '.next',            // classname for next button
        });
        // init plugin
        $('.thumbs').ie8Gallery();
    });
</script>
```
### HTML part
The src attribute is the source for the thumbnail. The data-img-src is the source of the big image.
```
<div class="thumbs">
    <img class="thumb" src="img/cat1-thumb.jpg" data-img-src="img/cat1.jpg" />
    <img class="thumb" src="img/cat2-thumb.jpg" data-img-src="img/cat2.jpg" />
    <img class="thumb" src="img/cat3-thumb.jpg" data-img-src="img/cat3.jpg" />
    <img class="thumb" src="img/cat4-thumb.jpg" data-img-src="img/cat4.jpg" />
</div>
```
