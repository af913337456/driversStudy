# readme

## 每个子工程的解释

* mem_test_1 : 使用vmalloc进行内存分配
* mem_test_2 : 使用kmalloc分配带有物理地址的dma内存

## 工程简单介绍

* 在打开字符设备节点后， 进行的操作
  * 应用层写入字符串， 驱动中将会把接收的字符串打印出来， 并将字符串记录到分配的内存中
  * 应用层读取数据， 驱动中将内存中的字符串返回给应用层