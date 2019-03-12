# ▤ SideMenu
[![Version](https://img.shields.io/cocoapods/v/SideMenu.svg?style=flat-square)](http://cocoapods.org/pods/SideMenu)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat-square)](https://github.com/Carthage/Carthage)
[![License](https://img.shields.io/cocoapods/l/SideMenu.svg?style=flat-square)](http://cocoapods.org/pods/SideMenu)
[![Platform](https://img.shields.io/cocoapods/p/SideMenu.svg?style=flat-square)](http://cocoapods.org/pods/SideMenu)
[![Total Downloads](https://img.shields.io/cocoapods/dt/SideMenu.svg?style=social)](http://cocoapods.org/pods/SideMenu)
[![Monthly Downloads](https://img.shields.io/cocoapods/dm/SideMenu.svg?style=social)](http://cocoapods.org/pods/SideMenu)
[![Weekly Downloads](https://img.shields.io/cocoapods/dw/SideMenu.svg?style=social)](http://cocoapods.org/pods/SideMenu)

### SideMenu for Legion

> Fork from jonkykong/SideMenu.

### We use
| Slide Out | Slide In |
| --- | --- |
| ![](https://raw.githubusercontent.com/jonkykong/SideMenu/master/etc/SlideOut.gif) | ![](https://raw.githubusercontent.com/jonkykong/SideMenu/master/etc/InOut.gif) |

## Requirements
- [x] Xcode 10.
- [x] Swift 4.2.
- [x] iOS 10 or higher.

## Installation
### CocoaPods

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

To integrate SideMenu into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '10.0'
use_frameworks!

pod 'SideMenu'

# For Swift 4 (no longer maintained), use:
# pod 'SideMenu', '~> 4.0.0'

# For Swift 3 (no longer maintained), use:
# pod 'SideMenu', '~> 2.3.4'
```

Then, run the following command:

```bash
$ pod install
```

## Usage
### Code Implementation

We use the SideMenuSetupable protocol that handles the styling of the menus.

### Customization

We use the SideMenuSetupable protocol that handles the styling of the menus, so you may ignore this part.

## Known Issues
* Important: displaying SideMenu instances directly over each other is not supported. Use `menuPushStyle = .subMenu` instead.
* Issue [#258](https://github.com/jonkykong/SideMenu/issues/258).
* Don't try to change the status bar appearance when presenting a menu. When used with quick gestures/animations, it causes the presentation animation to not complete properly and locks the UI. This was fixed in iOS 9.3. See [radar 21961293](http://www.openradar.me/21961293) for more information.

## License

SideMenu is available under the MIT license. See the LICENSE file for more info.
