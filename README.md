
前端纳米学位街机游戏克隆项目
===============================

# 项目要求
## 功能
- [x] 游戏功能正常，运行无误
- [x] 玩家无法移动到屏幕外
- [x] enemy横穿屏幕
- [x] player撞enemy后，player回到原点
- [x] 计时功能
- [ ] 玩家获胜后，出现动画
## 代码要求
- [x] player继承Enemy
- [x] 重写父类方法
- [x] 使用prototype chain和this关键字

## 文件说明
1. `app.js`说明
* 创建`Enemy` 的伪类,并实例化alEnemies实例化数组，需要多少个Enemies就实例化多少个；
* 创建继承自`Enemy`的子类`player`，重新父类`Enemy`的`updata`方法，并增加属性`Player.prototype.handleInput`方法;
2. engine.js 说明
* 使用DOM创建canvas画布；
* 函数`init`为回调函数，在`init`中调用`main`函数，游戏在这里一直刷新画面和检测游戏的状态；
3. `resources.js`说明
* 提供设置回调功能函数 `onReady`，图片先完成加载，便于绘制；
* 图片相关加载函数
4. index.html说明
* 外部引入脚本文件；
* 注意加载js文件的顺序


## 项目思路
- 根据Enemy 类，创建 player子类；
- 实例化 1个player 和 3个enemy；
- 重写player的updata方法，并实现4个方向键控制player的动作；
- 避免player超出边界
- 根据enemies的x和y的值同player的x和y值做比较，判断是否相撞；
- 实现计时功能


