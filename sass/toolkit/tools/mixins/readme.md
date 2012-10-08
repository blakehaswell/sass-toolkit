Mixins
======

## backgroundImageRetina($fileName, $width, $height)

The `backgroundImageRetina` mixin takes a filename, a width, and a height. It will set the `background-image` property to `filename + ".png"`, as well as creating a media query which will set the `background-image` property to `filename + "@2x.png"` as well as the `background-size` property.

### Example:

    @include backgroundImageRetina("../images/image", 32px, 16px);

### Produces:

    background-image: url("../images/image.png");
    
    @media only screen and (-webkit-min-device-pixel-ratio: 1.5),
            only screen and (-o-min-device-pixel-ratio: 3/2),
            only screen and (min--moz-device-pixel-ratio: 1.5),
            only screen and (min-device-pixel-ratio: 1.5) {
        background-image: url("../images/image@2x.png");
        -webkit-background-size: 32px 16px;
        -moz-background-size: 32px 16px;
        background-size: 32px 16px;
    }

## clearfix

### Example:

    @include clearfix;

### Produces:

    zoom: 1; // Trigger hasLayout in IE6/7

    &:before,
    &:after {
        content: "";
        display: table;
    }
    &:after {
        clear: both;
    }

## fluidImage

### Example:

    @include fluidImage;

### Produces:

    display: block;
    max-width: 100%;
    height: auto;

## generatedContent

### Example:

    @include generatedContent;

### Produces:

    content: '';
    display: block;

## horizontallyCentred

### Example:

    @include horizontallyCentred;

### Produces:

    margin-left: auto;
    margin-right: auto;

## imageReplacement

### Example:

    @include imageReplacement;

### Produces:

    text-indent: -9999px;

## positionAbs($left, $top)

### Example:

    @include positionAbs(40px, 10px);

### Produces:

    position: absolute;
    left: 40px;
    top: 10px;

## positionRel($left, $top)

### Example:

    @include positionRel(30px, 15px);

### Produces:

    position: relative;
    left: 30px;
    top: 15px;

## size($width, $height)

### Example:

    @include size(300px, 40px);

### Produces:

    width: 300px;
    height: 40px;

## square($size)

### Example:

    @include square(16px);

### Produces:

    width: 16px;
    height: 16px;
