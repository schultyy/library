# Objective-C

## File’s owner
Given the following files:

- PreferencesController.h
- PreferencesController.m
- PreferencesView.xib

In the NIB File, you will not instantiate a `PreferencesController` directly. Instead the NIB just gets informed that the owner (which will be provided when the NIB file is loaded) is a `PreferencesController`.

## First responder

The first responder is the current view which gets keyboard events.

## Call to IBAction leads to EXC_BAD_ACCESS
Control flow never reaches the actual IBAction, already stopped with `EXC_BAD_ACCESS`.
This is because an object is called which was already released.

## Constants

```Objective-C
//Constants.h

#ifndef FOO_H
#define FOO_H

#import <Foundation/Foundation.h>

FOUNDATION_EXPORT NSString *const foo;

#endif

//Constants.m file

#import <Foundation/Foundation.h>
#import “Constants.h”

NSString *const Foo = @"Bar";
```

## Create a statusbar application

Open <appname>.plist and add a new row:

Key: `Application is agent (UIElement)`
Value: `YES`
