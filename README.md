# Lope · 无头版 SmallDog V67（URDF + mesh）

本目录是 Lope 的无头仿真模型 **`v67_sim_r5_headless`** URDF 与 mesh 包。关节限位、惯量、连杆结构和几何与 `headless-v67` 上的原文件一致，只调整了目录位置。

## 文件

| 内容 | 路径 |
| --- | --- |
| URDF | [urdf/smalldog_v67.urdf](urdf/smalldog_v67.urdf) |
| mesh | [meshes/](meshes/) |

`meshes/` 里的每个文件都被这份 URDF 引用，共 35 个。URDF 中的路径写成相对 `urdf/` 的 `../meshes/...`，请保持这两个目录的相对位置。

## 使用

用 URDF 查看器打开本目录，并选择 `urdf/smalldog_v67.urdf`。例如在 [Robot Viewer](https://viewer.robotsfan.com/) 中导入包含 `urdf/` 和 `meshes/` 的文件夹。

默认站姿（弧度）不是全零：四个髋关节为 0；右侧 thigh = -0.6715534335840251、calf = 1.1；左侧 thigh = 0.6715534335840251、calf = -1.1。小腿 0 rad 不在本模型限位内。

模型来源见 [THIRD_PARTY.md](THIRD_PARTY.md)。
