**English** | [中文](./README.zh-CN.md)

> This page is the **front-end code** repository for the project, and the **back-end code** [please go to](https://github.com/binwenwu/WPFS-BOOT )

## Profile

> The national policy in the new era requires the promotion of the construction of `"smart wind power"`. The current difficulties in the field of wind power prediction mainly include poor prediction accuracy and insufficient digitalization of the industry. The 14th Five Year Plan for Modern Energy System proposes to accelerate the digital and intelligent upgrading of the energy industry and promote the construction of "smart wind power". Improving the accuracy of wind power prediction and providing scientific support for power grid scheduling is of great value to China's energy industry.
>
> The WPFboost work was developed by the Wuhan University End Band, aiming to build a `"digital intelligent"` wind power prediction platform to solve the above problems.

## Overall framework

Relying on the multi-source heterogeneous spatiotemporal big data and algorithm models accumulated in the early stage of the project, the team has built a three-level architecture application platform based on "digital intelligence integration" for wind power clusters, wind farm stations, and single wind turbines. While covering all aspects of wind power prediction, it also cleverly integrates advanced technologies such as the `Internet of Things`, `digital twins`, and `artificial intelligence`.

![image-20240331172536574](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331172536574.png)

Specifically, the project is based on a large-scale distributed database with full temporal and spatial resolution, as well as the team's innovative and integrated algorithm, the `Comprehensive Time series Fusion Networks (CTFN)`. In terms of digitization and intelligence, a multimodal large language model robot is introduced to create functional modules such as **data upload and preprocessing, training prediction, digital twin stations, wind farm monitoring screens, wind turbine anomaly monitoring, and AR wind power.**

## Model algorithm

The team proposed a prediction algorithm that integrates weather forecast data, models twenty wind turbines uniformly, and expands the dataset. Then expand the weather forecast data and input it into the encoder and decoder. Considering that the prediction performance varies for different wind turbine models, the team determines the model selection based on prediction errors, such as the model integration scheme of LightGBM and deep learning. Finally, the model algorithm also achieved good results among the top in the country (**score: 0.75274**).

![image-20240331172804499](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331172804499.png)

## Innovative features

- Relying on the Supercomputing Center of Wuhan University, we have achieved high-speed model inference and fast prediction;
- Multi scale and multi scene digital twinning has been carried out on multiple scenes such as high-altitude wind fields, coastal wind fields, and wilderness wind fields at a large scale. A monitoring screen for a single wind farm has been achieved at a medium scale, and abnormal monitoring for a single wind turbine has been achieved at a small scale;
- The visualization of the prediction results throughout the entire project provides a comprehensive solution to integrate wind power prediction into the platform from start to finish;
- Real time connection of IoT data, which can access real-time data from sensors, achieving data connection and multi screen simultaneous changes;
- AI empowers the real economy, supports voice input, and achieves artificial intelligence content generation for multimodal large language models.

## Software achievements

​	The team designed 6+1 functional modules: data upload and preprocessing, training prediction, digital twin station, wind farm monitoring screen, wind turbine anomaly monitoring, AR wind power, and a relatively independent LLM robot. These modules cover a comprehensive range of functions from data processing to prediction, from digital twins to AR display, providing a comprehensive solution for wind power prediction.

> The team has implemented multi terminal responsive design for all pages;
>
> The team provides a total of 16 4x4 preprocessing combination methods for data uploading and preprocessing, and displays rich visual charts, providing a workspace for users to review historical records;

- **Multiple terminals**

![image-20240331173142289](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173142289.png)

- **Data upload and preprocessing**

![image-20240331173205307](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173205307.png)

- **Training prediction**

![image-20240331173252686](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173252686.png)

- **Digital Field Station**

![image-20240331173304257](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173304257.png)

- **Monitoring large screen**

![image-20240331173318637](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173318637.png)

- **Abnormal monitoring**

![image-20240331173328034](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173328034.png)

- **AR**

![image-20240331173358016](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173358016.png)

- **Multimodal Q&A robot**

![image-20240331173416524](https://cdn.jsdelivr.net/gh/binwenwu/picgo_demo/img/image-20240331173416524.png)

## Installation and Use

- Get project code

```BASH
git clone https://github.com/binwenwu/WPFS.git
```

- Installation dependencies

```BASH
cd WPFS

npm install
```

- Local operation

```BASH
npm run serve
```

- pack

```bash
npm run build
```

## Browser support

The `Chrome 80+` browser is recommended for local development

Support modern browsers, doesn't include IE

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt=" Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt=" Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                         not support                          |                       last 2 versions                        |                       last 2 versions                        |                       last 2 versions                        |                       last 2 versions                        |

## Maintainer

[@Binwen Wu](https://github.com/binwenwu)

## License

[MIT © Tankenqi-2023](./LICENSE)
