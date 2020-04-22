# aim
- 框架要会用，webgl要深入研究下
# web3D
- 记录3D学习过程中的知识点
## threejs

- 初学的时候尽量不关注算法，主要了解顶点数据处理的过程，GPU渲染管线的基本功能单元。实际的工作中如果不是开发3D引擎可能不会使用原生WebGL API，但是学习了这些之后，对于three.js的深度开发学习很有好处，如果你了解你WebGL知识，可以联系绘制函数drawArrays()来理解渲染器的渲染操作方法render()。

### 场景
- scene--》 THree.screen
#### 光照
##### 颜色

- 环境光
- 点光源
- 平行光

#### 网络模型 mesh
##### 几何体 geometry
- 形状
- 尺寸
##### 材质 material
---所有的材质，都是对webgl着色器的封装--
- 颜色
- 贴图
- 透明度
### 相机
#### 位置
#### 视线方向
#### 投影方式
- 透射投影
- 正射投影


### 渲染器 renderer
##### 渲染器创建 webglRender 
##### 开始渲染 .render(scene, camera)
##### domElement属性 --- canvas对象
- requestAnimationFrame用于旋转图形，这个是浏览器自带的便于均匀的旋转
- 鼠标跟随旋转，与requestAnimationFrame方法不能同时存在

        function render() {
          renderer.render(scene,camera);//执行渲染操作
        }
        render();
        var controls = new THREE.OrbitControls(camera,renderer.domElement);//创建控件对象
        controls.addEventListener('change', render);//监听鼠标、键盘事件


## webGl

## js
###  react-three-fiber hooks fiber threejs
### [类型化数组](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Typed_arrays) 
- 对于canvas数据处理很有用 
- [Float32Array](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Float32Array)
- 
