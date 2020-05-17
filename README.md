UnityEditorExtension
这个工程目前包含了以下功能:
### 展示了GUI.skin.customStyles下所有的GUIStyle  

![图片](https://note.youdao.com/yws/public/resource/adfbabb5a71e5f49edece05c2c90dc98/xmlnote/28AB26BC34C94C28B2C4E0DBBC12FF66/5558)  
点击**Tools/GUIStyleViewer**中的Styles  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200517165024599.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2o3NTY5MTUzNzA=,size_16,color_FFFFFF,t_70#pic_center)
对于每一种**GUIStyle**绘制了active和inactive两种情况。  
代码差别如下:  
```
GUILayout.Toggle( false, inactiveText, thisStyle, GUILayout.Width( width / 2 ) );
GUILayout.Toggle( true, activeText, thisStyle, GUILayout.Width( width / 2 ) );
```
对于一些Button相关的样式，两种情况绘制的结果是不一样的。
***
### 展示了Unity自带的Texture2D  
点击**Tools/GUIStyleViewer**中的Icons     
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200517233945541.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2o3NTY5MTUzNzA=,size_16,color_FFFFFF,t_70#pic_center)
源码来自[Show Built In Resources](http://wiki.unity3d.com/index.php/Show_Built_In_Resources)
进行了以下修改:
- 修复了绘制非Texture2D类型的Texture会报错
- 改进搜索框样式
***
关于作者:
- **水曜日鸡**，简称**水鸡**，ACG宅。曾参与索尼中国之星项目研发，具有2D联网多人动作游戏开发经验。

CSDN博客：[https://blog.csdn.net/j756915370](https://blog.csdn.net/j756915370)  
知乎专栏：[https://zhuanlan.zhihu.com/c_1241442143220363264](https://zhuanlan.zhihu.com/c_1241442143220363264)  
Q群：891809847
