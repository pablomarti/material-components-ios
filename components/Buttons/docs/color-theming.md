<!--docs:
title: "Color Theming"
layout: detail
section: components
excerpt: "How to theme Buttons using the Material Design color system."
iconId: button
path: /catalog/buttons/color-theming/
-->

# Buttons Color Theming

You can theme buttons with your app's color scheme using the ColorThemer extension.

You must first add the Color Themer extension to your project:

``` bash
pod 'MaterialComponents/Buttons+Extensions/ColorThemer'
```

## Example code

<!--<div class="material-code-render" markdown="1">-->
#### Swift
``` swift
// Step 1: Import the ColorThemer extension
import MaterialComponents.MaterialButtons_ColorThemer

// Step 2: Create or get a color scheme
let colorScheme = MDCSemanticColorScheme()

// Step 3: Apply the color scheme to your component using the desired button style
MDCContainedButtonColorThemer.applySemanticColorScheme(colorScheme, to: component)
MDCFloatingButtonColorThemer.applySemanticColorScheme(colorScheme, to: component)
MDCTextButtonColorThemer.applySemanticColorScheme(colorScheme, to: component)
```

#### Objective-C

``` objc
// Step 1: Import the ColorThemer extension
#import "MaterialButtons+ColorThemer.h"

// Step 2: Create or get a color scheme
id<MDCColorScheming> colorScheme = [[MDCSemanticColorScheme alloc] init];

// Step 3: Apply the color scheme to your component using the desired button style
[MDCContainedButtonColorThemer applySemanticColorScheme:colorScheme
     toButton:component];
[MDCFloatingButtonColorThemer applySemanticColorScheme:colorScheme
     toButton:component];
[MDCTextButtonColorThemer applySemanticColorScheme:colorScheme
     toButton:component];
```
<!--</div>-->
