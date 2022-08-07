# IO流

# 1、File类

![image-20210912104353982](https://github.com/floretteJ/JavaNotes/tree/main/imgs/image-20210912104353982.png)

## 1.1 常用构造器

**在内存中创建，硬盘上不存在**

![image-20210912101455855](https://github.com/floretteJ/JavaNotes/tree/main/)/imgs/image-20210912101455855.png)

![image-20210912102144539](D:/Typora/imgs/image-20210912102144539.png)

![image-20210912102123342](D:/Typora/imgs/image-20210912102123342.png)

## 1.2 常用方法

![image-20210912102252915](D:/Typora/imgs/image-20210912102252915.png)

![image-20210912103159101](D:/Typora/imgs/image-20210912103159101.png)

![image-20210912103248088](D:/Typora/imgs/image-20210912103248088.png)

**真正硬盘中的创建**

![image-20210912103545641](D:/Typora/imgs/image-20210912103545641.png)

![image-20210912104148603](D:/Typora/imgs/image-20210912104148603.png)



# 2、IO流

## 2.1 IO流原理及其分类

![image-20210912105857349](D:/Typora/imgs/image-20210912105857349.png)

![image-20210912110017982](D:/Typora/imgs/image-20210912110017982.png)

![image-20210912110348565](D:/Typora/imgs/image-20210912110348565.png)

![image-20210912110612013](D:/Typora/imgs/image-20210912110612013.png)

## 2.2 FileReader

![image-20210912121138812](D:/Typora/imgs/image-20210912121138812.png)

![image-20210912122217553](D:/Typora/imgs/image-20210912122217553.png)

![image-20210912121812823](D:/Typora/imgs/image-20210912121812823.png)

![image-20210912123600651](D:/Typora/imgs/image-20210912123600651.png)

![image-20210912124303238](D:/Typora/imgs/image-20210912124303238.png) 

## 2.3  FileWriter

![image-20210912125024616](D:/Typora/imgs/image-20210912125024616.png)

![image-20210912125052693](D:/Typora/imgs/image-20210912125052693.png)

![image-20210912125418281](D:/Typora/imgs/image-20210912125418281.png)

## 2.4 FileInputStream和FileOutputStream

![image-20210912130532727](D:/Typora/imgs/image-20210912130532727.png)

**使用InputStream处理 文本文件会出现中文乱码问题**

**因为这是在内存上看，如果是复制文本文件则不会有问题**

![image-20210912130213066](D:/Typora/imgs/image-20210912130213066.png)

![image-20210912130814920](D:/Typora/imgs/image-20210912130814920.png)

## 2.5 BufferedInputStream和BufferedOutputStream

![image-20210912142751894](D:/Typora/imgs/image-20210912142751894.png)

![image-20210912142449366](D:/Typora/imgs/image-20210912142449366.png)

![image-20210912142832965](D:/Typora/imgs/image-20210912142832965.png)

## 2.6 缓冲流 ：BufferedReader和BufferedWriter

![image-20210912143340719](D:/Typora/imgs/image-20210912143340719.png)

![image-20210912143715298](D:/Typora/imgs/image-20210912143715298.png)

![image-20210912143915233](D:/Typora/imgs/image-20210912143915233.png)

![image-20210912144519126](D:/Typora/imgs/image-20210912144519126.png)

## 2.7 转换流：InputStreamReader和OutputStreamWriter

![image-20210912145130889](D:/Typora/imgs/image-20210912145130889.png)

![image-20210912145412534](D:/Typora/imgs/image-20210912145412534.png)

![image-20210912145723529](D:/Typora/imgs/image-20210912145723529.png)

![image-20210912150057616](D:/Typora/imgs/image-20210912150057616.png)

![image-20210912150631977](D:/Typora/imgs/image-20210912150631977.png)

## 2.8  字符编码集

![image-20210912152039158](D:/Typora/imgs/image-20210912152039158.png)

![image-20210912152141069](D:/Typora/imgs/image-20210912152141069.png)

![image-20210912153030963](D:/Typora/imgs/image-20210912153030963.png)

![image-20210912153148914](D:/Typora/imgs/image-20210912153148914.png)

## 2.9 标准输入输出流：System.in和System.out

![image-20210912153824317](D:/Typora/imgs/image-20210912153824317.png)

![image-20210912154133925](D:/Typora/imgs/image-20210912154133925.png)

![image-20210912154410208](D:/Typora/imgs/image-20210912154410208.png)

## 2.10 打印流：PrintStream和PrintWriter

![image-20210912155039917](D:/Typora/imgs/image-20210912155039917.png)

![image-20210912155548510](D:/Typora/imgs/image-20210912155548510.png)

## 2.11 数据流：DataInputStream和DataOutputStream

![image-20210912155643012](D:/Typora/imgs/image-20210912155643012.png)

![image-20210912160020274](D:/Typora/imgs/image-20210912160020274.png)

![image-20210912160413203](D:/Typora/imgs/image-20210912160413203.png)

## 2.12 对象流：ObjectInputStream和OjbectOutputSteam

![image-20210912160955189](D:/Typora/imgs/image-20210912160955189.png)

![image-20210912161331258](D:/Typora/imgs/image-20210912161331258.png)

![image-20210912161844181](D:/Typora/imgs/image-20210912161844181.png)

![image-20210912162321531](D:/Typora/imgs/image-20210912162321531.png)

![image-20210912163347414](D:/Typora/imgs/image-20210912163347414.png)

![image-20210912163100812](D:/Typora/imgs/image-20210912163100812.png)

## 2.13 随机存取文件流：RandomAccessFile

![image-20210912163748527](D:/Typora/imgs/image-20210912163748527.png)

![image-20210912164145503](D:/Typora/imgs/image-20210912164145503.png)

![image-20210912165447619](D:/Typora/imgs/image-20210912165447619.png)

![image-20210912164335462](D:/Typora/imgs/image-20210912164335462.png)

![image-20210912164756393](D:/Typora/imgs/image-20210912164756393.png)

![image-20210912165350423](D:/Typora/imgs/image-20210912165350423.png)

## 2.14 NIO.2的常用类

![image-20210912170023143](D:/Typora/imgs/image-20210912170023143.png)

![image-20210912170424386](D:/Typora/imgs/image-20210912170424386.png)

![image-20210912170451241](D:/Typora/imgs/image-20210912170451241.png)

![image-20210912170502143](D:/Typora/imgs/image-20210912170502143.png)

![image-20210912170519581](D:/Typora/imgs/image-20210912170519581.png)

![image-20210912170537540](D:/Typora/imgs/image-20210912170537540.png)
