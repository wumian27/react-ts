讲真我觉得 npm 是真的设计的很屎，不知道最开始为什么会设计成安装包默认不会添加到 dependencies，使用缓存这么容易想到的设计还是 yarn 首创的，锁定版本也是抄 yarn 的。
yarn 用起来舒服多了。但是 yarn 在 windows 经常有 hash 值对不上然后安装不了的 bug，搞得我很烦，看了一下 github 仓库，将近 2000 个 issues。
最近我重新试用了一下 cnpm，让我意外的是下载速度是真的快，同样的使用淘宝源，cnpm 比 yarn 还要快很多。但是我觉得 cnpm 安装之后，node_modules 看起来很乱，多了很多乱七八槽的依赖。
因为我有点洁癖，所以 yarn 和 cnpm 我站 yarn。其实 yarn 还有一个杀手级的特性 yarn workspace，用于管理 monorepos 的依赖，虽然这个项目不是 monorepos 结构，但是确实 说明一个问题 npm 在工程领域落后 yarn 太远了。


因为我们这个项目不打算发布到 npm，所以 private 设置为 true。

这个 main 入口对于我们这个模板项目来说没什么意义，直接删了。