Code Style Guide
===========

## Background

http://developer.apple.com/documentation/Cocoa/Conceptual/CodingGuidelines/index.html

## Formatting

1. Tabs instead of spaces (Xcode -> preferences -> text editing -> indentation)
2. Opening brace stays on the same line
3. One space should be used between the - or + and the return type, and no spacing in the parameter list except between parameters  
```
- (void)setTabBarHidden:(BOOL)hidden animated:(BOOL)animated
```
4. Fractional numbers  
	Correct:  
	0.0f  
	1.0f  
	Incorrect:  
	.5f
	2.f

## Naming

1. Class names (along with category and protocol names) should start as uppercase and use mixed case to delimit words
2. Method names should start as lowercase and then use mixed case. Each named parameter should also start as lowercase
3. Variables names start with a lowercase and use mixed case to delimit words. Instance variables have leading underscores

## Obj-C Features

1. Variables and private methods should be declared in implementation file. Keep your class simple; avoid "kitchen-sink" APIs. If a method doesn't need to be public, don't make it so. Use a private category to prevent cluttering the public header
2. Do not invoke the NSObject class method new, nor override it in a subclass. Instead, use alloc and init methods to instantiate retained objects
3. Instance subclasses may be in an inconsistent state during init and dealloc method execution, so code in those methods should avoid invoking accessors


## Project folder structure

	Classes
		Controllers
		Models
		Views
	Images
		Backgrounds
		Icons
	Interface
	Fonts
	*.xcodeproj



