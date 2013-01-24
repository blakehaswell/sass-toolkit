Mixins
======

## backgroundImageRetina($fileName, $width, $height: null)

The `backgroundImageRetina` mixin allows you to easily set a background image that supports standard and retina displays. The mixin only supports `.png` files. The background image for retina devices is expected to have the same name as the standard background image, except with @2x at the end (e.g. `"background@2x.png"`).

### Arguments:

*   `$fileName`: The relative path to the background images, minus the extension (which is assumed to be `.png` for the standard image and `@2x.png` for the retina image).
*   `$width`: The width of the standard background image.
*   `$height` (optional): The height of the standard background image. If not provided it is presumed that the height is the same as the width.

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

Including the `clearfix` mixin forces the element to contain any floated child elements.

### Example:
    
    .container {
        @include clearfix;
    }

### Produces:

    .container:after {
        content: "";
        display: table;
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
