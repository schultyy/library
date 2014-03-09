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
Control flow never reaches the actual IBAction, already stopped with EXC_BAD_ACCESS. 
This is because an object is called which was already released.