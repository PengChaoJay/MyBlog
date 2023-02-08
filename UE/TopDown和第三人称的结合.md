# UE topdown 和 第三人称结合
## 需求是要求具有两套输入方式
 1. 具有第三人称的输入模式，即wasd控制移动
 2. 具有topdown的输入方式，鼠标点选位置，玩家移动过去
## 实现方式
  1. 总体
  ![](https://github.com/PengChaoJay/MyBlog/blob/main/UE/Image/1675844730466.png)
  2. 鼠标点选位置，自动寻路
  ![](https://github.com/PengChaoJay/MyBlog/blob/main/UE/Image/1675844636931.png)
  3. 得到的各条路是以vector的形式存在的，依次遍历得到各个位置，作为add movement input的位置
  ![](https://github.com/PengChaoJay/MyBlog/blob/main/UE/Image/1675844715882.png)
  4. 检测玩家wasd是否输入，进行中断自动寻路的行为
  ![](https://github.com/PengChaoJay/MyBlog/blob/main/UE/Image/1675844585619.png)
        
  
