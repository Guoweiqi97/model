# model
本模型采用改进的SEIR病毒传染模型，想法来源：https://zhuanlan.zhihu.com/p/104268573?night=1
模型大致流程：![image](https://user-images.githubusercontent.com/38526596/109908297-fd593d00-7cde-11eb-9475-c56450addf36.png)
通过建立微分方程组，通过matlab求解微分方程组的数值解!
微分方程组如下：
[image](https://user-images.githubusercontent.com/38526596/109907784-faaa1800-7cdd-11eb-9979-2fc64d09f5ef.png)
修改后的迭代表达式为：![image](https://user-images.githubusercontent.com/38526596/109908150-b4a18400-7cde-11eb-8592-ed3f905be95a.png)
表达式中相应的参数表示为：![image](https://user-images.githubusercontent.com/38526596/109908343-1104a380-7cdf-11eb-85c9-f3ca46cce1f3.png)


通过改变感染人数和接触者感染概率得出相应的图像：
![r=20,b=b1=0 03](https://user-images.githubusercontent.com/38526596/109908572-7e183900-7cdf-11eb-9a29-805a792bfdbb.jpg)
![r1=5,b=0 03](https://user-images.githubusercontent.com/38526596/109908580-807a9300-7cdf-11eb-8c57-a439703ef273.jpg)
![r1=r2=5](https://user-images.githubusercontent.com/38526596/109908587-83758380-7cdf-11eb-8163-40a3ef4b6fd3.jpg)
![b=0 01](https://user-images.githubusercontent.com/38526596/109908595-87a1a100-7cdf-11eb-9a90-0a160ac7b4cd.jpg)
![b=0 003](https://user-images.githubusercontent.com/38526596/109908603-8b352800-7cdf-11eb-85cd-381337451b7e.jpg)
从中可以看出减少接触人数对疫情防控起到至关重要的作用，而佩戴口罩可以降低感染率，对于疫情防控也非常的关键。该模型未考虑的死亡率，个人认为可以再设置一个变量来表示死亡率，感染的病人一方面会康复也会有可能死亡，从而建立出更加合理的模型。


