# GrootSwift

[![Join the chat at https://acm-uiuc.slack.com/messages/C6XGZD212/](https://img.shields.io/badge/slack-groot-724D71.svg)](https://acm-uiuc.slack.com/messages/C6XGZD212/)


Pod for easily adding Groot integration to your iOS App or Swift Project


## Requirements

- iOS 10.0+ / macOS 10.10+ / tvOS 9.0+ / watchOS 2.0+
- Xcode 8.0+
- Swift 3.0+


## Installation

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

> CocoaPods 1.0.0+ is required to build GrootSwift.

To integrate GrootSwift into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
platform :ios, '10.0'
use_frameworks!

target '<Your Target Name>' do
    pod 'GrootSwift', '~> 0.3.1'
end
```

Then, run the following command:

```bash
$ pod install
```


## Usage

### Example Merch Service Request

```swift
import GrootSwift

MerchService.getItems(success: { (json) in
    // Handle Success (Background thread)
}) { (error) in
    // Handle Failure (Background thread)
}.perform(withAuthorization: nil)
```


## License

This project is licensed under the University of Illinois/NCSA Open Source License. For a full copy of this license take a look at the LICENSE file.

When contributing new files to this project, preappend the following header to the file as a comment:

```
Copyright © 2017, ACM@UIUC

This file is part of the Merch Project.

The Merch Project is open source software, released under the University of Illinois/NCSA Open Source License.
You should have received a copy of this license in a file with the distribution.
```
