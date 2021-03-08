### 透视投影矩阵

#### view matrix

输入视口坐标`eye_pos`。相机移到视口相当于所有物体反方向移到`{-eye_pos[0], -eye_pos[1], -eye_pos[2]}`。

#### model matrix

在作业中是将模型旋转给定的角度。

#### projection matrix

将一个frustum映射到1x1x1的cube。输入`eye_fov`, `aspect_ratio`, `zNear`, `zFar`，直接套公式。

### 绘制过程

绘制的过程就是计算mvp矩阵`projection * view * model`，对模型的每一个点进行矩阵变换。
