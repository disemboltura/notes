numpy属性
---------

>  ndim : 维度

>  shape : 行数和列数

>  size : 元素个数


numpy array 创建
----------------
> array : 创建数组

>     `a = np.array([2,3,4])`

> dtype : 创建时指定数据类型

>     `a = np.array([2,3,4,5], dtype=np.int)`

>     `a = np.array([2,3,4,5], dtype=np.float32)`

> zeros : 创建的数据全为 0

>     `a = np.zeros( (3,4) ,dtype = np.int ) # 创建3行,4列, 数据类型为int ,数据全为 0 `

> empty : 创建的数据全接近 0

>     `a = np.empty( (3,4) )` # 创建3行,4列，数据都接近于 0

> arange : 按指定范围来创建数据

>     `a = np.arange(10,20 , 2)  #创建范围在10到20之间的数据 步长为2 (间隔为2)`

> linespace: 指定间隔内，返回间隔均匀的数据

>     `a = np.linespace( 1 , 10 , 20)  #开端是 1, 结束是10 ，分割成20个数据 `


使用reshape 改变数据形状:
-----------------------
>     `a = np.arange(20,dtype=np.int).reshape(3,4)  #变成3行4列 `


