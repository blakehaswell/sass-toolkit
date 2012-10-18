Placeholders
============

## clearfix

### Example:

    @extend %clearfix;

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

    @extend %fluidImage;

### Produces:

    display: block;
    max-width: 100%;
    height: auto;

## generatedContent

### Example:

    @extend %generatedContent;

### Produces:

    content: '';
    display: block;

## horizontallyCentred

### Example:

    @extend %horizontallyCentred;

### Produces:

    margin-left: auto;
    margin-right: auto;

## imageReplacement

### Example:

    @extend %imageReplacement;

### Produces:

    text-indent: -9999px;
