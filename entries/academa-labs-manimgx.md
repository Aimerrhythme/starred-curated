# academa-labs/manimgx

## 简介

兼容 Manim CE API 的 3D 数学动画引擎，Rust + wgpu 渲染，速度更快，自带字体、公式排版和视频编码，还能在浏览器里跑，并为 AI agent 提供分镜检查命令。

## 适用场景

- 适合：做讲解动画，如傅里叶级数、相量旋转、三相旋转磁场、矩阵变换；让 AI agent 自动生成教学短视频。
- 不适合：依赖 Manim CE 第三方插件的老项目（兼容范围未核实）；需要 Python 3.13 以下环境。

## 快速用法

对照上游 README（2026-11-04 版本），需 Python 3.13+：

```bash
pip install manimgx
```

```python
import manimgx as m

class Hello3D(m.ThreeDScene):
    def construct(self) -> None:
        self.set_camera_orientation(phi=65 * m.DEGREES, theta=-45 * m.DEGREES)
        cube = m.Cube(side_length=3, fill_opacity=0.3, stroke_width=2)
        self.play(m.Create(cube), run_time=2)
```

渲染为 MP4 的命令见上游 Quickstart（未核实具体参数）。

## 推荐理由

近期 Star 激增（10 月创建，入库时约 2.5 千 Star，MIT）。无需本机装 LaTeX，比原版 Manim 更容易在课件流水线里落地，适合电气课程的动画演示。

## 入库日期

2026-11-04

## 源链接

https://github.com/academa-labs/manimgx

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
