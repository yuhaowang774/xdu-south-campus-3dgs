# 西安电子科技大学南校区 3DGS 模型

西安电子科技大学南校区（Xidian University South Campus）的 3D Gaussian Splatting 重建模型，提供完整版与裁切版两个 SOG v2 文件，可直接在浏览器中查看。

![西安电子科技大学南校区 3DGS 重建预览](assets/preview.jpg)

> [!IMPORTANT]
> 本项目为个人学习与研究用途的非官方发布，与西安电子科技大学官方无关，不代表学校立场。采集、发布与使用请遵守相关法律法规。

## 下载

| 版本 | Splats | 大小 | 说明 | 下载 |
| --- | ---: | ---: | --- | --- |
| 完整版 | 8,195,476 | 116 MB | 保留完整场景范围 | [xdu-south-campus-full-8.2m.sog](https://github.com/yuhaowang774/xdu-south-campus-3dgs/releases/download/v1.0.0/xdu-south-campus-full-8.2m.sog) |
| 裁切版 | 7,958,807 | 114 MB | 裁切至核心场景，包围盒更紧凑，推荐预览 | [xdu-south-campus-cropped-8.0m.sog](https://github.com/yuhaowang774/xdu-south-campus-3dgs/releases/download/v1.0.0/xdu-south-campus-cropped-8.0m.sog) |

SHA-256 校验和见 [SHA256SUMS](SHA256SUMS)。

### 模型详情

| 项目 | 完整版 | 裁切版 |
| --- | --- | --- |
| 文件大小 | 120,967,587 字节 | 119,294,631 字节 |
| 坐标范围（模型单位） | x 6.984 / y 2.280 / z 5.988 | x 2.607 / y 0.584 / z 2.537 |
| 球谐阶数 | 3 | 3 |
| SOG 生成器 | splat-transform v3.0.0 | splat-transform v3.9.0 |

坐标范围为 SOG 元数据中的包围盒尺寸，模型使用归一化坐标，不代表米制尺寸，也未附带地理坐标或真实比例尺。

## 查看方式

1. 打开 [SuperSplat 在线编辑器](https://superspl.at/editor)。
2. 将 `.sog` 文件拖入页面，或通过 File → Import 导入。
3. 建议先试裁切版，加载更快。

也可以在知天下平台在线查看：[西安电子科技大学南校区作品页](https://3d.explorerglobal.cn/model/zl3043jl)。

SOG 是 PlayCanvas SuperSplat 使用的压缩高斯泼溅格式（v2），支持该格式的 PlayCanvas 应用均可加载。

## 训练信息

- 训练平台：知天下
- 知天下作品页：https://3d.explorerglobal.cn/model/zl3043jl
- 采集规模、影像分辨率、训练迭代次数、曝光/色彩处理等参数：待补充

## 适用场景

- 校园场景的三维浏览与展示
- 计算机图形学、三维重建相关的研究与教学演示
- 支持 SOG 格式的 Web 应用集成

不适用于测绘、导航、工程测量等需要精确几何、地理坐标或真实比例尺的任务。

## 已知限制

- 未附带地理参考、真实比例尺与坐标基准
- 反光、透明材质、植被和细薄结构可能出现伪影
- 动态物体可能被固化或产生拖影
- 未进行几何精度与量测精度评估
- 裁切版仅保留核心场景范围，周边区域不完整

## 隐私与合规

- 采集与公开发布应获得校园管理方许可
- 发布前需检查画面中的清晰人脸、车牌等个人信息，必要时进行处理
- 公开高精度三维模型可能涉及测绘地理信息管理要求，请勿公开精确坐标或比例尺

## 许可

- 仓库内文档与脚本：[MIT](LICENSE)
- 模型权重：[CC BY-NC 4.0](LICENSE-MODEL)（署名—非商业性使用）

模型权重可以共享、改编，但必须署名、注明是否修改，且不得用于商业目的。完整法律文本见 [LICENSE-MODEL](LICENSE-MODEL)。

建议署名：

> “西安电子科技大学南校区 3DGS 模型” by yuhaowang774, licensed under CC BY-NC 4.0.
> Source: https://github.com/yuhaowang774/xdu-south-campus-3dgs

商业使用需另行联系版权持有人授权。CC BY-NC 4.0 不是 OSI 认可的开源软件许可，属于“开放权重、非商业使用”许可。

## 引用

如果本模型对你的工作有帮助，引用信息见 [CITATION.cff](CITATION.cff)。

## 致谢

- 训练平台：知天下
- SOG 格式与查看器：[PlayCanvas SuperSplat](https://github.com/playcanvas/supersplat)
