# EasyTransition
EasyTransition is a simple library for make a transition in iOS.

## Features
- [x] Transition from corners
- [x] Interactive dismissal transition

## Requirements
Swift 2 or later

##  Installation
-

## Usage
Import and declare EasyTransition:
```swift
import EasyTransition

class ViewController: UIViewController {
  var transition: EasyTransition?
}
```
Customise transition and present normally:

```swift
let vc = TargetViewController()
transition = EasyTransition(attachedViewController: vc)
transition?.transitionDuration = 0.4
transition?.direction = .Right
transition?.margins = UIEdgeInsets(top: 0, left: 100, bottom: 0, right: 0)
presentViewController(vc, animated: true, completion: nil)
```
You can also make a direction from a corner:
```swift
transition?.direction = [.Top,.Right]
```
And more on EasyTransitionExample.xcodeproj

## Sources Used
Background Images: www.subtlepatterns.com 

## The MIT License (MIT)

Copyright (c) 2016 Nattawut Singhchai

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.