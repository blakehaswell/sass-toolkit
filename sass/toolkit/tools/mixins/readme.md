Mixins
======

## backgroundImageRetina($fileName, $width, $height)

The `backgroundImageRetina` mixin takes a filename, a width, and a height. It will set the `background-image` property to `filename + ".png"`, as well as creating a media query which will set the `background-image` property to `filename + "@2x.png"` as well as the `background-size` property.

### Example

#### SASS:

    @include backgroundImageRetina("../images/image", 32px, 16px);

#### Produces:

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

## fluidImage

## generatedContent

## hidden

## horizontallyCentred

## imageReplacement

## positionAbs($left, $top)

## positionRel($left, $top)

## size($width, $height)

## square($size)
