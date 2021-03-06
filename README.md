
# SwiftMime

[![Version](https://img.shields.io/cocoapods/v/SwiftMime.svg?style=flat)](http://cocoadocs.org/docsets/SwiftMime)
[![Stories in Ready](https://badge.waffle.io/weekwood/SwiftMime.png?label=ready&title=Ready)](https://waffle.io/weekwood/SwiftMime)
[![Build Status](https://travis-ci.org/weekwood/SwiftMime.svg?branch=master)](https://travis-ci.org/weekwood/SwiftMime)

Comprehensive MIME type mapping API. Includes all 600+ types and 800+ extensions defined by the Apache project, plus additional types submitted by the node.js community.

inspired from [mime](https://github.com/broofa/node-mime)

## Usage

### Basic API

    SwiftMime.sharedManager.lookupExtension("text/html")
    SwiftMime.sharedManager.lookupType("pdf")

### define

  	SwiftMime.sharedManager.define([
  	"text/x-some-format": ["x-sf", "x-sft", "x-sfml"],
  	"application/x-my-type": ["x-mt", "x-mtt"]
  	])
	SwiftMime.sharedManager.lookupType("pdf")

## Installation

SwiftMime is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

    pod "SwiftMime"

## Author

di wu, di.wu@me.com

## License

SwiftMime is available under the MIT license. See the LICENSE file for more info.
