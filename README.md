# Group6_FinalProject_v0
完整项目工程的地址：https://github.com/sysu-computer-graphics-team/CG-FinalProject/
##  项目运行
```
git clone https://github.com/sysu-computer-graphics-team/Group6_FinalProject_v0
进入bin文件夹，再进入exe文件夹
运行 OpenGLFinalProject.exe
```

##  文件目录
```
- bin 存放资源以及可执行程序
  --- Resources 存放项目所需要资源
      --- objects  存放项目的模型
      --- shaders  存放项目的着色器
      --- textures 存放项目的纹理
      --- fonts    存放项目的字体
  --- Resources 存放项目可执行文件
- doc 存放演示视频
- src 存放项目代码以及库
  --- Resourcess   上传了Shader的代码
  --- Includes     存放项目需要的外部头文件
  --- Src          存放项目代码
```

##  代码介绍
```
- program.cpp         程序的入口,负责初始化窗口
- game.h              初始化场景中的物体，控制各个物体的渲染
  -- game.cpp
- shader.h            着色器类
  -- shader.cpp
- texture.h           纹理类
  -- texture.cpp
- resource_manager.h  负责资源调度，避免同个shader、texture、ModelObject多次声明
  -- resource_manager.cpp
- custom_object.h     将物体的基本属性封装，减少冗余
  -- custom_object.cpp
  -- border.h         继承自custom_object,对应场景中的边界
  -- lamp.h           继承自custom_object,对应场景中的台灯
  -- plane.h          继承自custom_object,对应场景中的平面
- camera.h            摄像机
- mesh.h              网格
  -- model.h          模型
- ModelObject.h       封装好的模型类，负责模型的导入
- mytext.h            文字类，用于文字渲染
- scene.h             场景类，用于渲染迷宫
- skybox.h            天空盒类
```

##  项目完成度
已实现如下功能：
- 相机漫游
- 基础的光照和着色
- 纹理映射
- 阴影映射
- 模型的导入与网格
- 天空盒
- 文字渲染
- 爆破效果
- 物理效果
- 粒子系统
