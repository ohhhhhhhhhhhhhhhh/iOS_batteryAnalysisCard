# iOS_batteryAnalysisCard
 记录上一次电量到目前电量的时间间隔，统计分析平均掉电时间，查看最高电量到现在的时间。

### 电池用量记录组件/battery.scriptable

组件功能：记录上一格电量直到目前电量所花费的时间，根据iOS电量消耗特点，\[99.5%, 100.5%)的电量区间均记录为100%，因此实际记录的电量时间间隔为2分钟。

新加入了统计每分钟平均掉电量的功能，以及上一次记录的最高电量和最高电量至目前的时间间隔。

根据iOS小组件的刷新机制，小组将的自动刷新由iOS统一管理，大约5分钟刷新一次（系统设置电量图为18分钟记录1次），如果需要高频记录，可以点击组件，然后'run script'手动执行，并且将小组件放置在经常刷新到的页面，会增加刷新频率。如果配合快捷指令/自动化执行，可以更加高频记录。

#### 注意，目前设定接入充电器之后自动清除缓存。

清除缓存或第一次使用可能会找不到缓存文件，可能出现数据不准确的情况，耐心等待记录或者手动刷新几次就好了。


### 睡眠待机电量分析组件/analysis.js

基本功能：配合快捷指令/自动化，晚上开启睡眠模式时，或可手动点击睡眠开始，让检测组件记录当前电量。第二天睡眠模式自动关闭时，读取记录计算睡眠时长、掉电量等，然后在某一条件下通知推送。

暂未开发

#### 使用说明

App Store下载安装软件'scriptable'：

![1](https://user-images.githubusercontent.com/66932433/147191575-8771ba6b-daa9-4973-b9c4-e766faf18c64.jpg)

然后下载.scriptable文件直接导入软件，
组件预览图：

![2](https://user-images.githubusercontent.com/66932433/147191672-0f2b1337-7eda-4bb6-ba92-3a07839675be.jpg)
