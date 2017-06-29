# my_erasure_coding
+ 该方法采用二进制矩阵进行纠删码的编解码
+ 提供n+m<=16的编解码方式，2<=n<=12，2<=m<=4
+ 使用方法只需要构造数据节点的状态信息，调用ec_get_recover_table_by_ec_status接口可以得到数据块解码的拓扑
+ 二进制矩阵避免RS编码的乘法查表运算，所有编码全部是关联数据块的异或运算，理解简单