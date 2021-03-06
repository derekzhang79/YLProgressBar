YLProgressBar
=================
The YLProgressBar is an UIProgressView replacement with an highly and fully customizable animated progress bar in pure Core Graphics

![](https://github.com/YannickL/YLProgressBar/raw/master/YLProgressBarSample/Resources/Images/YLProgressBar.gif)

It has been implemented using the Core Graphics framework without any images. So it can be customize freely and independently the plateform.

Installation
============

### Manually
Copy the YLProgressBar folder into your project and then simply import the "YLProgressBar.h" in the file(s) you would like to use it in.

### Using CocoaPods

The YLProgressBar can also be added to a project using [CocoaPods](https://github.com/CocoaPods/CocoaPods) by adding this line to your podfile:

```
// Podfile
pod 'YLProgressBar'
```
and
```
pod install
```

# How To Use

Here are some examples to show you how you can configure the YLProgressBar:

```objc
// Blue flat progress, with no stripes
_progressBar.type               = YLProgressBarTypeFlat;
_progressBar.progressTintColor  = [UIColor blueColor];
_progressBar.hideStripes        = YES;

// Green rounded/gloss progress, with vertical animated stripes
_progressBar.type               = YLProgressBarTypeRounded;
_progressBar.progressTintColor  = [UIColor greenColor];
_progressBar.stripesOrientation = YLProgressBarStripesOrientationVertical;

// Rainbow flat progress, with the indicator text displayed over the progress bar
_progressBar.type                     = YLProgressBarTypeFlat;
_progressBar.hideStripes              = YES;
_progressBar.indicatorTextDisplayMode = YLProgressBarIndicatorTextDisplayModeProgress;
_progressBar.progressTintColors       = @[[UIColor colorWithRed:33/255.0f green:180/255.0f blue:162/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:3/255.0f green:137/255.0f blue:166/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:91/255.0f green:63/255.0f blue:150/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:87/255.0f green:26/255.0f blue:70/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:126/255.0f green:26/255.0f blue:36/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:149/255.0f green:37/255.0f blue:36/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:228/255.0f green:69/255.0f blue:39/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:245/255.0f green:166/255.0f blue:35/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:165/255.0f green:202/255.0f blue:60/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:202/255.0f green:217/255.0f blue:54/255.0f alpha:1.0f],
                                          [UIColor colorWithRed:111/255.0f green:188/255.0f blue:84/255.0f alpha:1.0f]];
```

You can also configure every YLProgressBar using the UIAppearence protocol, which can be done in your app delegate:

```objc
[[YLProgressBar appearance] setType:YLProgressBarTypeFlat];
[[YLProgressBar appearance] setProgressTintColor:[UIColor blueColor]];
```

License
====================
Copyright 2013 Yannick Loriot.<br />
http://yannickloriot.com

Permission is hereby granted, free of charge, to any person obtaining a copy<br />
of this software and associated documentation files (the "Software"), to deal<br />
in the Software without restriction, including without limitation the rights<br />
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell<br />
copies of the Software, and to permit persons to whom the Software is<br />
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in<br />
all copies or substantial portions of the Software.
 
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR<br />
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,<br />
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE<br />
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER<br />
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,<br />
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN<br />
THE SOFTWARE.
