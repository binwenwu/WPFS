**中文** | [English](./README.md)

> 本页为项目**前端代码**仓库，**后端代码**[请前往](https://github.com/binwenwu/WPFS-BOOT)

## 简介

>新时代国家政策要求推进`“智慧风电”`建设。目前风电预测领域面临的困难主要有预测准确率欠佳，产业数字化不足等。《“十四五”现代能源体系规划》提出，要加快能源产业数字化智能化升级，推进“智慧风电”建设。提高风电功率预测的准确性，为电网调度提供科学支撑，对我国能源产业有重要的价值。
>
>WPFboost作品由武汉大学结束乐队开发完成，旨在构建一个`“数智一体”`的风电预测平台，以解决以上问题。

## 总体框架

有赖于项目前期积累的多源异构时空大数据和算法模型，团队基于“数智一体”搭建了一个风电集群、风电场站、单风机三级架构应用平台，在涵盖了风电预测的方方面面的同时，还巧妙地融合了**物联网**、**数字孪生**、**人工智能**等先进技术。

![image-20240331172536574](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331172536574.png)

具体而言，项目以全时空分辨率大型分布式数据库以及团队自行创新融合的算法`Complementary Time series Fusion Networks（CTFN）`为基础，在数字化与智能化方面引入多模态大语言模型机器人，打造了**数据上传与预处理、训练预测、数字孪生场站、风电场监测大屏、风机异常监控以及AR风电**等功能模块。

## 模型算法

团队提出了一个融合天气预报数据的预测算法，对二十个风机统一建模，扩充数据集。然后将天气预报数据扩展后输入到编码器和解码器中。考虑到针对不同风机模型预测效果不同，团队通过预测误差来决定模型的选择，如LightGBM与深度学习的模型集成方案。最后模型算法也取得了全国前列的好成绩（**score: 0.75274**）。

![image-20240331172804499](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331172804499.png)

## 创新特色

- 依托于武汉大学超算中心，实现了高速模型推理，实现快速预测；
- 多尺度多场景数字孪生，在大尺度上对高山风场、海滨风场以及荒原风场等多场景进行了数字孪生，在中尺度上实现了单风电场的监测大屏，在小尺度上实现了单风机的异常监控；
- 全过程的预测结果可视化贯穿了整个项目，提供一个全面的解决方案使风电预测从始至终落实在平台中；
- 物联网数据实时连接，可接入传感器实时数据，实现数据一连接，多屏齐变化；
- AI赋能实体经济，支持语音输入，实现了多模态大语言模型的人工智能内容生成。

## 软件成果

​	团队设计了“6+1”个功能模块：数据上传与预处理、训练预测、数字孪生场站、风电场监测大屏、风机异常监控以及AR风电，和较为独立的LLM机器人。这些模块涵盖了从数据处理到预测，从数字孪生到AR展示的全方位功能，为风电预测提供了一个全面的解决方案。

> 团队对所有页面都做了多终端响应式设计；
>
> 数据上传和预处理，团队提供了4x4共16种预处理组合方法对上传数据进行预处理，并展示丰富的可视化图表，提供了工作空间，便于用户回顾历史记录；

- **多终端**

![image-20240331173142289](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173142289.png)

- **数据上传与预处理**

![image-20240331173205307](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173205307.png)

- **训练预测**

![image-20240331173252686](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173252686.png)

- **数字场站**

![image-20240331173304257](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173304257.png)

- **监测大屏**

![image-20240331173318637](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173318637.png)

- **异常监控**

![image-20240331173328034](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173328034.png)

- **AR**

![image-20240331173358016](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173358016.png)

- **多模态问答机器人**

![image-20240331173416524](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173416524.png)

## 安装和使用

- 获取项目代码

```BASH
git clone https://github.com/binwenwu/WPFS.git
```

- 安装依赖

```BASH
cd WPFS

npm install
```

- 本地运行

```BASH
npm run serve
```

- 打包

```bash
npm run build
```

## 浏览器支持

建议使用`Chrome 80+`浏览器进行本地开发

支持现代浏览器，不包括IE

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt=" Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt=" Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                         not support                          |                       last 2 versions                        |                       last 2 versions                        |                       last 2 versions                        |                       last 2 versions                        |

## 维护人员

[@Binwen Wu](https://github.com/binwenwu)

## 许可证

[MIT © Tankenqi-2023](./LICENSE)
