# min_stack

实现一个栈的push,pop,top，以及取最小值的函数。

key idea:
定义两个栈s1,s2 将最小值存入s2中，则取最小值时只需s2.top即可。

每次push时，都需要与s2.top比较一下，若小于s2的值，则放入s2(注意：若同样的最小值有很多个，均需要存入)
每次pop时，如果s1.top==s2.top，s2的值也需要被弹出。
