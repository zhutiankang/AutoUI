# AutoUI
多屏幕适配
> res-new-Android Resource Folder

## 不常用：Screen Size:  values-small
1. small (small screens)
2. normal (normal screens)
3. large (large screens)
4. xlarge (extra-large screens)

## 常用：具体分辨率 优先级 sw > w > h(h基本无用)  同时多个都有，优先匹配多限定的文件夹
* sw720dp sw1080dp (最小宽度不分设备横竖屏，只找宽高最小的尺寸)
* w1280dp w1920dp
* values-sw720dp-w1280dp    720p 宽度>=1280 使用
* values-sw720dp-w1920dp    720p 宽度>=1920 使用
* values-sw720dp            如果上面两个都存在，宽度<1280 使用
* layout其他文件夹与values一样使用

## 常用命令：
* adb shell dumpsys window displays
* adb shell wm size reset
* adb shell wm size
* adb shell wm size 1280x720
* adb shell wm density

## 密度表
* res/drawable-mdpi/：中等密度（160dpi）
* res/drawable-hdpi/：高密度（240dpi）
* res/drawable-xhdpi/：超高密度（320dpi）
* res/drawable-xxhdpi/：超超高密度（480dpi）
* res/drawable-xxxhdpi/：超超超高密度（640dpi）

