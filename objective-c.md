# Objective-C

## File’s owner
Given the following files:

- PreferencesController.h
- PreferencesController.m
- PreferencesView.xib

In the NIB File, you will not instantiate a `PreferencesController` directly. Instead the NIB just gets informed that the owner (which will be provided when the NIB file is loaded) is a `PreferencesController`.