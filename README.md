# 文字动态图生成工具

这是一个用于生成文字动态图的工具，灵感来自于一个 Go 项目（项目地址没找到...）。

### 安装
``` bash
$ pip install lolly
```

### 用法
点击图片可预览完整动图效果

``` bash
$ lolly --help

Usage: lolly [OPTIONS] WORDS

  WORDS: The words you want to display in a gif image

Options:
  -w, --width INTEGER      Image width (default 400)
  -h, --height INTEGER     Image height (default 400)
  -b, --bg-color TEXT      Background color (default 'white')
  -s, --font-size INTEGER  Font size (default 50)
  -c, --font-color TEXT    Font color (default 'red')
  -t, --font-type TEXT     Font type (default 'Microsoft YaHei')
  -d, --duration INTEGER   Animation duration (default 400)
  -p, --path TEXT          Output path (default 'out.gif')
  --help                   Show this message and exit.
```

### 示例
```bash
$ lolly "talk is cheap show me your picture"
```
![out](https://user-images.githubusercontent.com/19553554/38259494-c02d24a8-3797-11e8-8336-c8bb8395a305.gif)

```bash
$ lolly "python is the best language in the world" -b "yellow" -c "green"
```
![out](https://user-images.githubusercontent.com/19553554/38259611-0e8c20a4-3798-11e8-8089-abadeeec6751.gif)

```bash
$ lolly "love you more than I can say" -b "pink" -c "blue" -d 350
```
![out](https://user-images.githubusercontent.com/19553554/38259727-4f9a9e36-3798-11e8-93f0-3b19bb63e983.gif)

```bash
$ lolly "陈 独 秀 同 志 请 坐 下" -s 80 -b "#eee"
```
![out](https://user-images.githubusercontent.com/19553554/38259860-b25926f0-3798-11e8-9653-d01390d60346.gif)


### License
MIT [©chenjiandongx](https://github.com/chenjiandongx)
