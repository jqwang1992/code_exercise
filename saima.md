<b>1、数组定义的时候初始化</b><br>
　char(int) str[10] = {0}; //该句相当于字符串制空<br>
<b>2、上下取整</b><br>
　double ceil(double x); //向上取整<br>
　double floor(double x); //向下取整<br>
<b>3、long类型</b><br>
　sizeof(long) = 4(x86), sizeof(long long) = 8(x86_64);<br>
　<br>
<b>4、字符与整数的互相转换问题</b><br>
　首先看个例子：<br>
	
	int a = 3;
	char c = '1';
	printf("change int a to char:%c\n", (char)a);//输出ascii码为3的符号
	printf("change char c to int:%d\n", (int)c);//输出49

	//可以看出上面的输出并不是我们想要的结果，所以正确的转换应该如下：
	printf("change int to char:%c\n", char(a + 48));
	printf("change char to int:%d\n", (int)c - 48);

　<br>