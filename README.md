# 傅里叶分析
## 傅里叶级数
1. 讲义为谌秋辉老师的手写稿，看第三次讲义之前看上面的那个初识傅里叶级数，里面包括入门的傅里叶级数，希望你先从基的正交（先当作是基，基的完备性需要证明三角级数在L2空间稠密或者其他的推论比如说正交补为0，因为相关的推论，证明太多了，泛函内积里面有）学习；然后从数分，泛函两个不同时代的角度来求出系数，初步探讨收敛条件而且系数必有衰减性。  
2. 再从现代分析学的视角证明L2范数下均方收敛（积分收敛，几乎处处收敛），在另外一份名为傅里叶级数依L2范数均方收敛里面。  
3. 再去看第三次讲义，探讨傅里叶级数逐点收敛的不同条件，Dini条件和Jordan条件。Dini条件是从经典分析学来看待问题，其中，狄利克雷核，勒贝格黎曼引理为我们最重要的工具。  
4. Jordan条件是从现代分析学，有界变差来看待问题，积分第二中值定理是我们最重要的工具。  
5. 我们数分上说的，L1可积，分段光滑，分段连续这个充分条件只是Dini条件的一种情况；lip条件也是Dini条件的一种情况；（狄利克雷条件）L1可积，分段单调，分段连续这个充分条件只是Jordan条件的一种情况  
## 傅里叶变换
1. 傅里叶级数从泛函上理解是找一组正交基（三角级数）来刻画周期函数和定义域无限的非周期函数，故要研究各种范数下的收敛条件；  
2. 傅里叶变换是来刻画定义域无限的非周期函数，把他看作是周期函数，周期从负无穷到正无穷，周期取极限，求和取极限，变成积分。而做傅里叶变换再做傅里叶逆变换是否能等于原函数（包括积分是否收敛（本质上傅里叶变换和逆变换就是积分）），就是我们这个周期无穷的假设是否成立，需要傅里叶反演定理来证明  
3. 还要学习傅里叶变换的性质，还有和卷积的性质。其中导数的傅里叶变换要用到分部积分，这里可引入紧支撑（也可以从泛函空间引入） 
4. 但是傅立叶变换要存在，积分要想收敛，必要条件是函数绝对可积（L1）但是这样的函数太少了，起码我们绝大部分初等函数不在L1,比如说x,sinx,cosx,e^x傅里叶变换都不收敛，要想解决这样的问题有三种办法  
## 窗口(短时)傅里叶变换,小波变换
第一种就是分成一段段区间分别做傅里叶变换。将时域分成若干个短时间段，每个时间段乘以一个窗函数，然后对每个窗口内的信号进行傅里叶变换。窗口傅里叶变换一定程度上克服了傅里叶变换的缺点，但是仍然有时间窗宽度不随频率变化的问题。小波变换解决了这个问题，但把傅里叶的三角基函数都变成小波基。  
## 广义函数
第二种就是作用到性质很好的测试函数上，如果效果相同就是说明傅里叶变换弱收敛于一个函数，这是广义函数的思想。能保留整个时域但是太过复杂  
## 拉普拉斯变换
第三种就是乘一个衰减权函数再做傅里叶变换，这就是拉普拉斯变换的思想，用衰减性很好的负指数函数，但是要想利用其衰减性，就必须只要一半的时域。拉普拉斯变换求解简单，而且能处理大部分初等函数，让积分收敛，但是也丢失一半的时域  
## 应用
其次再计算一些积分的时候，复变函数的围道积分，留数定理能帮我们很好的解决很多问题。而傅里叶变换，拉普拉斯变换在解决偏微分方程，常微分方程组，常微分方程，积分都有他的优势。
