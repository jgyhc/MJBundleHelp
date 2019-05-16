# MJBundleHelp

[![CI Status](https://img.shields.io/travis/jgyhc/MJBundleHelp.svg?style=flat)](https://travis-ci.org/jgyhc/MJBundleHelp)
[![Version](https://img.shields.io/cocoapods/v/MJBundleHelp.svg?style=flat)](https://cocoapods.org/pods/MJBundleHelp)
[![License](https://img.shields.io/cocoapods/l/MJBundleHelp.svg?style=flat)](https://cocoapods.org/pods/MJBundleHelp)
[![Platform](https://img.shields.io/cocoapods/p/MJBundleHelp.svg?style=flat)](https://cocoapods.org/pods/MJBundleHelp)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

MJBundleHelp is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'MJBundleHelp'
```

## Author

jgyhc, jgyhc@foxmail.com.com

## License

MJBundleHelp is available under the MIT license. See the LICENSE file for more info.

pod集成的时候，方便获取bundle资源，把原来的imageNamed方法 替换成bundleKey: imageNamed:即可,`bundleKey`为当前组件的组件名，例如
`MSGoodsManagerKit`库里需要使用一个名叫`delete_icon`的图片：  
```
	self.imageView.image = [UIImage bundleKey:@"MSGoodsManagerKit" imageNamed:@"delete_icon"]；
```
这样可以全局搜索项目里的`imageNamed`方法，直接替换成`bundleKey:@"MSGoodsManagerKit" imageNamed`就好了
