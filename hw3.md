### Shading

套公式插值计算每个点的颜色，法线，纹理坐标，调用不同shading函数获得最终的颜色，绘制。

#### normal shader

直接把法线的xyz三个值作为rgb颜色。

#### phong shader

遍历所有光源，套公式计算环境光，漫反射，镜面反射，求和。

#### texture shader

和phong完全一样，只是固有颜色变成通过uv坐标从texture取颜色。

#### bump shader

套公式对法线做扰动，直接把法线的值作为颜色。

#### displacement shader

套公式对法线做扰动，算完后用phong shading算颜色。
