<!--docs:
title: "Color Theming"
layout: detail
section: components
excerpt: "How to theme Flexible Header using the Material Design color system."
iconId: header
path: /catalog/flexible-headers/color-theming/
-->

# Flexible Header Color Theming

You can theme a flexible header with your app's color scheme using the ColorThemer extension.

You must first add the Color Themer extension to your project:

``` bash
pod 'MaterialComponents/FlexibleHeader+Extensions/ColorThemer'
```

## Example code

<!--<div class="material-code-render" markdown="1">-->
#### Swift
``` swift
// Step 1: Import the ColorThemer extension
import MaterialComponents.MaterialFlexibleHeader_ColorThemer

// Step 2: Create or get a color scheme
let colorScheme = MDCSemanticColorScheme()

// Step 3: Apply the color scheme to your component
MDCFlexibleHeaderColorThemer.applySemanticColorScheme(colorScheme, to: component)
```

#### Objective-C

``` objc
// Step 1: Import the ColorThemer extension
#import "MaterialFlexibleHeader+ColorThemer.h"

// Step 2: Create or get a color scheme
id<MDCColorScheming> colorScheme = [[MDCSemanticColorScheme alloc] init];

// Step 3: Apply the color scheme to your component
[MDCFlexibleHeaderColorThemer applySemanticColorScheme:colorScheme
     toFlexibleHeaderView:component];
```
<!--</div>-->
