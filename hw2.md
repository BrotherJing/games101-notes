### 画三角形

遍历bounding box内每个像素，套公式算点是否在三角形内，插值计算每个点的z，更新zbuffer和绘制。

#### super-sampling实现anti-alias

循环体改成把点分成四份计算四次，最后求个平均再绘制。
