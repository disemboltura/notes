numpy
========
numpy主要功能：
> ndarray , 高效的多位数组, 具有快速的面向数组的运算操作和灵活的广播能力

> 快速操作整个数组的数学函数

> 读写硬盘以及内存映射文件的工具

> 线性代数, 随机数生成, 和傅里叶变换等

> 
    
ndarray
==========
    ndarray是一个多位数组,数组中的元素必须是同一个类型的数据,  每个ndarray都有一个 shape, dtype 属性, 分别表明数组的维度以及数组元素的类型.
    
创建ndarray
------------

1.array函数创建ndarray


    data = [1,2,3,5] 
    arr1 = np.array(data)

-----------
2. zeros, ones 创建元素为 0 ,1 的元素

    arr2 = np.zeros(10)
    
    arr3 = np.zeros(3,2)

----------

3. empty 创建空的数组

    arr4 = np.empty(2,3)


axis = 0 表示列轴
-------------
axis = 1 表示行轴
-------------
创建ndarray的函数列表:
------------------
* array
* asarray
* arange
* ones
* ones_like
* zeros
* zeros_like
* empty
* empty_like
* full
* full_like
* eye , identity


ndarray数据类型:
-------------
* int8, uint8
* int16, uint16
* int32, uint32
* int64, uint64
* float16
* float32
* float64
* float128
* complex64
* complex128
* complex256
* bool
* object            python object type, can be any python object
* string_           fixed-length ascii type
* unicode_          fixed-length unicode type

------------
     arr5 = np.array([2,3,5,12,10],dtype=uint32)
     
     
ndarray索引
----------
    ndarray 索引和列表等操作是一样的，通过下标来索引对应的元素.
    

