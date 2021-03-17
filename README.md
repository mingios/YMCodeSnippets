# YMCodeSnippets
iOS 开发中 常用的代码段

部分代码块来自 [https://github.com/QMUI/QMUI_iOS_CodeSnippets]()

## 使用方式
Xcode 的 Code Snippets 文件存放于 `~/Library/Developer/Xcode/UserData/CodeSnippets` 目录，只要直接把 `*.codesnippets` 文件放到这个目录下（若没有则自己创建），重启 Xcode 即可生效。
```
cd ~/Library/Developer/Xcode/UserData/CodeSnippets
git clone https://github.com/mingios/YMCodeSnippets.git ./
```
重启后，在Xcode 中查看，使用快捷键 `cmd + shift + L`

## 快捷键汇总
*NSObject*
- `pa` - 定义一个 `assign` 的 property
- `par` - 定义一个 `assign, readonly` 的 property
- `pc` - 定义一个 `copy` 的 property
- `pcr` - 定义一个 `copy, readonly` 的 property
- `ps` - 定义一个 `strong` 的property
- `psr` - 定义一个 `strong, readonly` 的property
- `pw` - 定义一个 `weak` 的property
- `pwr` - 定义一个 `weak, readonly` 的property
- `propertySwizzleAssign` - 用 `swizzle` 的方式定义一个 `assign` 的property
- `propertySwizzleCopy` - 用 `swizzle` 的方式定义一个 `copy` 的property
- `propertySwizzleStrong` - 用 `swizzle` 的方式定义一个 `strong` 的property
- `propertySwizzleWeak` - 用 `swizzle` 的方式定义一个 `weak` 的property
- `load_once` - 创建一个带 `dispatch_once` 的 `+load` 方法
*Block*
- `blockParameterInMethod` - 声明一个用于 OC 方法参数的 block
- `blockParameterInFunction` - 声明一个用于 C 函数参数的 block
- `blockproperty` - 声明一个用于 property 的 block
- `blocktypedef` - 用 `typedef` 定义一个 block
- `blockvar` - 定义一个作为局部变量的 block

*Method & Function*
- `fnv` - 定义一个返回值为 `void` 的方法
- `fnv:` - 定义一个返回值为 `void` 且带参数的方法
- `fnblock` - 定义一个返回值类型为 block 的方法
- `fnv_handleEvent` - 定义一个用于 `UIControl` 事件回调的方法
- `fnv_longPress` - 定义一个用于 `UILongPressGestureRecognizer` 的回调方法（你就不用每次都去拼写那个很长的手势名字了）
- `fnv_pan` - 定义一个用于 `UIPanGestureRecognizer` 的回调方法
- `fnv_tap` - 定义一个用于 `UITapGestureRecognizer` 的回调方法

*UITableView*
- `initWithStyle` - 展开 `initWithStyle:` 方法
- `initWithStyleForCell` - 展开 `UITableViewCell initWithStyle:reuseIdentifier:` 方法
- `tableViewDelegate` - 展开常用的几个 `UITableViewDelegate` 方法
- `numberOfSectionsInTableView` - 展开 `numberOfSectionsInTableView:`方法
- `numberOfRowsInSection` - 展开 `tableView:numberOfRowsInSection:` 方法
- `cellForRowAtIndexPath` - 展开 `tableView:cellForRowAtIndexPath:` 方法
- `heightForRowAtIndexPath` - 展开 `tableView:heightForRowAtIndexPath:` 方法
- `didSelectRowAtIndexPath` - 展开 `tableView:didSelectRowAtIndexPath:` 方法
- `tableView_scrollNever` - UITableView Scroll Never

*UICollectionView*
- `collectionViewDelegate` - 展开常用的几个`UICollectionViewDelegate` 方法
- `numberOfSectionsInCollectionView` - 展开 `numberOfSectionsInCollectionView:`
- `numberOfItemsInSection` - 展开 `collectionView:numberOfItemsInSection:`
- `cellForItemAtIndexPath` - 展开 `collectionView:cellForItemAtIndexPath:`
- `sizeForItemAtIndexPath` - 展开 `collectionView:layout:sizeForItemAtIndexPath:` 方法
- `didSelectItemAtIndexPath` - 展开 `collectionView:didSelectItemAtIndexPath:` 方法
- `didDeselectItemAtIndexPath` - 展开 `collectionView:didDeselectItemAtIndexPath:` 方法


*UIView*
- `addtarget` - 调用 `UIControl addTarget:action:forEvents:` 方法
- `setImageForButton` - 为 `UIButton` 设置图片
- `setTitleColorForButton` - 为 `UIButton` 设置文字颜色
- `setTitleForButton` - 为 `UIButton` 设置文字

*UIViewController*
- `initWithNib` - 展开 `initWithNibName:bundle:` 方法
`didInitializeWithStyle:` 方法
- `viewDidLoad` - 展开 `viewDidLoad` 方法
- `viewWillAppear` - 展开 `viewWillAppear:` 方法
- `viewDidAppear` - 展开 `viewDidAppear:` 方法
- `viewWillDisappear` - 展开 `viewWillDisappear:` 方法
- `viewDidDisappear` - 展开 `viewDidDisappear:` 方法


*Other*
- `pragma` - 展开一个用于 Xcode 导航的 `#pragma mark -` 宏
- `log` - 展开 `NSLog(@"xxx")`
- `osif` - 展开一个 @available(iOS xxx, \*) 的 if 判断
- `__weakSelf` - 定义一个 `weak` 的 `self` 指针
- `__strongSelf` - 将 `weakSelf` 指针改为 `strong` 的 `self` 指针
