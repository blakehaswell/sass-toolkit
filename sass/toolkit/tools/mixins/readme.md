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

### Example

#### SASS:

    @include clearfix;

#### Produces:

## fluidImage

### Example

#### SASS:

    @include fluidImage;

#### Produces:

## generatedContent

### Example

#### SASS:

    @include generatedContent;

#### Produces:

## hidden

### Example

#### SASS:

    @include hidden;

#### Produces:

## horizontallyCentred

### Example

#### SASS:

    @include horizontallyCentred;

#### Produces:

## imageReplacement

### Example

#### SASS:

    @include imageReplacement;

#### Produces:

## positionAbs($left, $top)

### Example

#### SASS:

    @include positionAbs(40px, 10px);

#### Produces:

## positionRel($left, $top)

### Example

#### SASS:

    @include positionAbs(40px, 10px);

#### Produces:

## size($width, $height)

### Example

#### SASS:

    @include size(300px, 40px);

#### Produces:

## square($size)

### Example

#### SASS:

    @include square(16px);

#### Produces:
