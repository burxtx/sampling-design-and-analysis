## 名词解释D
1. 多阶段抽样  
    假设总体由N 个初级单元组成，每个初级单元又由若干个二级（次级）单元组成，先在总体中按一定方法抽取n 个初级单元，对每个抽中的初级单元再抽取若干二级单元进行调查，这种抽样方法称为二阶段抽样(two-stage sampling)（也称二阶抽样、二级抽样），如果每个二级单元又由更小的三级单元组成，那么在第二阶段抽样后，若在每个被抽中的二级单元中再进行三级单元的抽样，则是三阶段抽样（三阶抽样）。同样的道理，还可以定义更高阶段抽样。对于二阶段以上的抽样，称为多阶段抽样。
    特点：
    - 构造抽样框相对容易，使得大范围抽样变为可能
    - 样本单元分布相对集中，具有较强的可操作性
    - 不同阶段中抽样方法可以灵活，有利于抽样效率的提高
    - 可用于“散料”的抽样

2. 二阶段抽样  
    假设总体由N 个初级单元组成，每个初级单元又由若干个二级（次级）单元组成，先在总体中按一定方法抽取n 个初级单元，对每个抽中的初级单元再抽取若干二级单元进行调查，这种抽样方法称为二阶段抽样(two-stage sampling)（也称二阶抽样、二级抽样）

3. 自加权样本  
    在自加权抽样设计方案中，每个样本单元的设计权数都是相同的，即每个单元最终入样的概率是相等的。在各种抽样方法下，如果总体中每一个最基本单元被抽中的概率相等，这种抽样设计就称为自加权设计，这样的样本就称为自加权(self-weighting)样本

4. 入样概率
    

5. 包含概率


6. 汉森-赫维茨估计量  
    令$Z_i=\cfrac{M_i}{\Sigma{M_i}}$为第i个单元（群）入样概率  
    $\Sigma{M_i}=M$  
    均值估计量为：  
    $$\color{red}\hat{\bar{Y}}_{pps}=\cfrac{1}{n}\sum_{i=1}^n\bar{Y}_i$$
    均值估计量的方差为：  
    $$\color{red}V(\hat{\bar{Y}}_{pps})=\cfrac{1}{n}\cfrac{\sum_{i=1}^n(\bar{Y}_i-\hat{\bar{Y}}_{pps})^2}{n-1}$$
    总量的估计量为：  
    $$\color{red}\hat{Y}_{pps}=\cfrac{1}{n}\sum_{i=1}^n\cfrac{Y_i}{Z_i}=\cfrac{\Sigma{M_i}}{n}\Sigma{\bar{Y}_i}=\cfrac{M}{n}\Sigma{\cfrac{Y_i}{M_i}}$$
    总量估计量的方差：  
    $$\color{red}V(\hat{Y}_{pps})=\cfrac{1}{n(n-1)}{\sum_{i=1}^n}(\cfrac{y_i}{z_i}-\hat{Y}_{pps})^2$$

7. 二重抽样  
    先从总体中随机抽取一个样本量较大的样本，对其进行简单调查以获取有关总体的结构或者辅助信息，为下一步抽样提供条件；然后再从中随机抽取一个样本量较小的样本对总体研究的目标量进行估计，称为二重抽样。
    作用：
    - 进行样本筛选
    - 进行事后分层，抽选好的样本，是的样本结构与总体结构一致
    - 获得辅助信息的估计，提高估计效率
    - 用于对无回答的调整
  
8. 抽样中的权数


9. 样本量  
    从总体中抽取若干单元的集合的数量叫样本量，用n表示

10. 随机化回答  
    是针对敏感问题或者高度隐私问题的调查，采用的一种特殊方法。这种抽样调查基于概率理论，通过设计一套或若干套的特殊问答卡片，由受访者随机抽取卡片回答问题，然后再收集答卷，通过样本数据对目标总体进行推断。  
    技术特征：  
    - 随机化回答方式
    - 对受访者起到保密作用
    - 同时可以对目标参数进行推断

11. 逆抽样方法  
    捕获再捕获法有时会遇到第二次捕获的样本中没有标记单元，即r=0的特殊情况，或者预估的第二次捕获样本量比实际需要的大很多。针对这种情况霍尔丹提出一种逆抽样方法：
    逆抽样法的实施流程为：先获取数量为n1 的样本并在样本上进行标记，然后将这些样本放回总体，在已标记的样本充分融入总体后，进行第二次抽样。在这一阶段中，事先确定一个整数r(r>1)，然后进行逐个抽样，直到抽到r 个具有标记特征的单元为止。设抽到r 个具有标记特征的单元时实
    际抽取的样本量为n，根据第二次捕获时总体分布结构与第一次捕获时的结构相同的原理推算出：  
    N的估计为  
    $$\color{red}\hat{N}=\frac{n_1n}{r}$$
    方差估计为
    $$\color{red}v(\hat{N})=\frac{n^2n(n-r)}{r^2(r+1)}$$

12. 沃纳模型  
    沃纳模型是沃纳(Warner)于1965 年首先提出的一种随机化回答模型。该模型是为了解决社会经济现象中敏感性问题而采用的一种随机化回答技术。
    模型设计的基本思想是：  
    为了调查某个敏感问题或者高度隐私问题，同时列出两个存在相关关系的问题制成卡片（一个问题是具有某种特征，记为卡片A；另一个问题是不具有某种特征，记为卡片B），卡片A所占比例为P，卡片B所占比例为1-P。被调查者随机抽取卡片（调查人员不知道抽取结果）进行回答，答案只能是“是”或“不是”  

    弱点：  
    A,B卡片均为敏感问题  
    P不能等于1/2

13. 西蒙斯模型  
    针对沃纳模型的弱点提出的一种改进。  
    模型设计的基本思想是：为了调查某个敏感问题或者高度隐私问题，同时列出两个无关的问题制成卡片（一个问题是具有某种特征，记为卡片A；另一个问题是无关问题，记为卡片B），卡片A所占比例为P，卡片B所占比例为1-P。

14. 多阶段抽样
    
15. 辅助变量 


