---
sidebar_position: 7
---

# 时轴

为字幕设置正确的出现时间和持续时间，使对白与画面同步。

## 参考规范

- 日文部分使用日文字体，中文部分使用中文字体
- 为对话设置层级，中文的层级大于日文
- 如果可以，对话部分使用有繁体版本的字体，否则使用 GBK 字体
- 在合适位置添加 Credits 信息
- 以 libass 渲染效果为准
- 观感（以下几点都需要视情况而定）
  - 一句话的持续时间不小于 60 ms
  - 相邻过近的时间轴应该使其连续，避免闪轴（参考：250ms）
  - 字幕在说话开始前出现，在说完后稍作停留（参考：向前余量 80 ~ 150ms 向后余量 250 ~ 350ms）
  - 如果时间轴前后有场景切换，紧贴场景切换（参考：句首 -250 ~ +50ms 句尾 -200 ~ +700ms）
  - 同屏出现多个对话，优先考虑调整边距
- 字幕设置（通常情况）
  - ScriptType: v4.00+
  - WrapStyle: 2
  - ScaledBorderAndShadow: yes
  - YCbCr Matrix: TV.709
  - PlayRes[XY] / LayoutRes[XY]: 源视频分辨率

另可参阅[喵萌奶茶屋的时轴规范](https://github.com/Nekomoekissaten-SUB/Nekomoekissaten-Subs/wiki/Recommendations-to-follow-for-ASS-production)。

## 学习资料

<!-- - 时轴：从入门到放弃（by Ming，2099 年，新建文件夹.jpg） -->
- [Aegisub教程:从入门到精通 序章:初识AEG](https://www.bilibili.com/video/BV19F411w7m5)（by 桜都字幕组，2022 年）
- [Timing Basics](https://unanimated.github.io/timing-basics.htm) / [Timing Without Using TPP](https://unanimated.github.io/timing-without-tpp.htm)（by unanimated，2014 年）

## 常用工具

- 文本编辑器
- 视频播放器（推荐使用 mpv）
- [Aegisub](https://github.com/TypesettingTools/Aegisub/)
