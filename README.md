# BubblePicker

[![License](http://img.shields.io/badge/license-MIT-green.svg?style=flat)]()
[![](https://jitpack.io/v/apps-in/BubblePicker.svg)](https://jitpack.io/#apps-in/PickImage)


Simplified version of [PickImage widget](https://github.com/jrvansuita/PickImage)

## Requirements
- Android SDK 16+

## Usage

Add to your root build.gradle:
```Groovy
allprojects {
	repositories {
	...
	maven { url "https://jitpack.io" }
	}
}
```

Add the dependency:
```Groovy
dependencies {
	implementation 'com.github.apps-in:PickImage:1.0.5'
}
```

Customize dialog
```Groovy
PickSetup setup = new PickSetup()
	.setTitle(getString(R.string.take_a_photo))
	.setTitleColor(getColor(R.color.colorTextWhite))
	.setTitleTypeface(R.font.montserrat_bold)
	.setTitleSize(16)
	.setBackgroundColor(getColor(R.color.colorPrimaryDark))
	.setButtonTextColor(getColor(R.color.colorTextWhitePressed))
	.setButtonTextTypeface(R.font.montserrat_regular)
	.setButtonTextSize(14)
	.setCancelTextColor(getColor(R.color.colorTextOrange))
	.setCancelTextSize(12)
	.setCancelTextTypeface(R.font.montserrat_semibold);
```

Show dialog
```Groovy
PickImageDialog.build(setup).show(this);
```

## License

MIT License

Copyright (c) 2020 Ihor Nepomniashchyi

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
