舰船战力溢出修复v1.1
游戏版本: v3.8.*
————————————————————
xT的战力溢出修复mod
重新计算后战斗力与原版基本相等
单舰战斗力在8.5G前不会变成1(但2.1G-4.3G等情况会显示负数)
在前面的图片是原版，后面的是重算后的
————————————————————
我已经推导出来了战斗力计算公式，发在了wiki中Defines#Ship#MILITARY_POWER_EXPONENT 后面: stellaris.paradoxwikis.com/Defines#Ship
具体讲解在tieba.baidu.com/p/8029004849
————————————————————
PS:就算战力变1了，更高还可以再溢出回来
defines文件里还有一套单舰战力上限2.1G的参数；一套上限215G的(已经达到了压缩上限)，战力过低可能会变成75281；
一套2.1G的(从215G的改指数压到2.1G)，战力越大相对原版减小越多，战力过低可能会变成23173
还有52G的和52G->2.1G的
注意!!!: 215G版本有最小战力要求, 约100, 使用之后小泡泡、初始护卫舰战斗力会变成75281
因此新增了一套上限52G的
关于写这个mod的原因: 其他战力溢出修复mod(我找到的)其一：数值通常相对原版变化较大；其二：较大程度改动了EXP，导致战力数值的参考作用下降；其三：由上两个问题导致战力相关的事件/外交受到影响
其实我还想改一下外交权重的算法(不是改系数)，使得后期，特别是mod环境下，军事/经济/科技外交权重不至于差得离谱




Ship power overflow repair v1.1 (Machine translation, I hope you could understand it)
Game version: v3.8.*
————————————————————
The power recalculated is basically equal to the original version
Single ship power will not become 1 before 8.5G (but 2.1G-4.3G display negative numbers)
The picture in the front is the original, and the one after it is the recalculated version
————————————————————
Military Power Calculation Formula : wiki#Defines#Ship#MILITARY_POWER_EXPONENT
(derived and published by me)
Learn more about it: tieba.baidu.com/p/8029004849
————————————————————
PS
Even if the power becomes 1, the higher one can still be spilled back 
The defines file also contains set of parameters with a maximum combat power of 2.1G for a single ship; 
A set with upper limit 215G (the upper limit of compression has been reached), if the power is too low, it may become 75281; 
A set with upper limit 2.1G (from 215G to 2.1G), the more powerful it is, the more it decreases compared with the original version. If the power is too low, it may become 23173
And 52G and 52G->2.1G