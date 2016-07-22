* 要注意react-native的transform中没有提供类似web css3中的transform-origin(设置偏移的基准点)属性,
react-native中所有的偏移都是以元素的中心点为基准进行的, 无法更改
* 故这里为了达到最终效果, 采取了自行计算偏移的位置, 以达到更改偏移基准点的效果