1.main.cpp 是源代码
运行环境:Code::Blocks IDE 16.1.0.0 , c++11标准下


2.main.exe 是可执行文件，为 win7下生成，
输入文件 data.txt
输出文件 out.txt

3.输入格式：

【注：默认约束条件对应序号：1经过点数的限制 2必经点 3必经边 4路径长度】
有序关系			//输入例如 3 2 1 4表示3>2>1>4
重要性程度之比			//依次输入r2,r3,r4   (r2=w1/w2)
必经的节点个数  必经路径数	//输入
开始节点  结束节点 链路代价 
//每输入一条边后换行
//......
必经点的点数 		//输入
必经过的节点 		
//每输入一个点后换行
//......
必经之路的数目 		//输入
开始点 结束点 		
// 每输入两点后换行
//......
不能经过的路径的数目//输入
开始点 结束点 		
// 每输入两点后换行
//......


4.输出格式：
**********Pass All Must constraints********** //通过所有必经点与必经边
********No constraints**********//忽略所有限制条件，最短路径
********Only less equal max Pass Num Constraints********//经过的点数不超过最大值
**********Pass All Must Edges constraints**********//经过所有必经点边
**********Pass All Must Vertexes constraints**********//经过所有必经点
**********Pass Weight constraints**********//根据权重系数，总体偏离限制条件程度最小
**********other reference paths*********//其余所有路径

其中定义：passVertex（经过点的数目，包括起始点与终点）；distance （路径花费）；
pass must edges（必须经过边的集合） ；pass must Vertexes（必须经过点的集合）；
路径表示为“0 => 57 => 345 => 402” 数字为每点的标记，0为起点。


5.样例放在testdata文件夹下，
分别有输入data1.txt，data2.txt，data3.txt，data4.txt
分别对应输出out1.txt,out2.txt,out3.txt,out4.txt

data1.txt
总点数：500；可游历点的最大点数：100；经点的点数： 7；必经之路的数目：2 ；不能经过的边的数目：1 
序关系 3 2 1 4；相邻指标的重要性之比 ：1.8 1.2 1.6；用时：20.197s 

data2.txt
初赛赛题（蚂蚁游历储藏间）
总点数：18；可游历点的最大点数：9；必经点的点数：2；必经之路的数目：2 ；不能经过的边的数目：1；
序关系 3 1 2 4；相邻指标的重要性之比 ：1.4 1.2 1.6；用时：0.055s

data3.txt
总点数：800 ；可游历点的最大点数：100；必经点的点数： 51；	必经之路的数目：14 ；不能经过的边的数目：8
序关系 3 4 1 2；相邻指标的重要性之比 ：1.4 1.2 1.6；用时：0.001s

data4.txt
总点数：160  ；可游历点的最大点数：50；必经点的点数： 25；必经之路的数目：9 ；不能经过的边的数目：5；
序关系 3 4 1 2；相邻指标的重要性之比 ：1.4 1.2 1.6；用时：0.001s




