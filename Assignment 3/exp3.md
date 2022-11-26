# <center> 作业：高阶孤子的振荡

&emsp;&emsp;*利用分步傅里叶变换算法（或者RK4算法）计算高阶孤子在非线性光纤（满足非线性薛定谔方程）的传输，光纤参数自取，入射光脉冲满足色散长度为非线性长度的4倍，传输距离为高阶孤子演化的一个周期（假设该数值为 LP）。*
&emsp;&emsp;*计算传输长度为 0、 LP/4、 LP/2、3LP/4、以及 LP 时，光脉冲的时域、频域分布，以及啁啾情况；计算传输长度为 0 和 LP/2 时，色散长度和非线性长度；以上述结果为依据、解释高阶孤子周期性演化的原因*

##### 传输长度为 $0$ 时，光脉冲的时域、频域分布，以及啁啾情况：
![l0](distance0.png)

<div STYLE="page-break-after: always;"></div>

##### 传输长度为 $LP/4$ 时，光脉冲的时域、频域分布，以及啁啾情况：
![l1](distance18.png)
&emsp;&emsp;红色是输入信号，黑色是输出信号。此时色散长度大于非线性长度，因此非线性主导，即 SPM。可见，频谱在 SPM 作用下有所展宽，而且从啁啾图中可见，SPM的确是主导的，前沿红移后延蓝移，是正常啁啾。色散在这个阶段的作用要小于 SPM，但是它在正常啁啾的作用下将脉冲压缩。

##### 传输长度为 $LP/2$ 时，光脉冲的时域、频域分布，以及啁啾情况：
![l2](distance35.png)
&emsp;&emsp;在传播距离是 $LP/2$ 时，脉冲的光谱展宽已经比较大了，变化非常明显，中间有一个零点，这是 SPM 展宽的典型特征。这时候脉冲也在色散和正常啁啾的共同作用下压缩了很多，峰值功率大概是输入时的 4 倍。从啁啾的角度上讲，这时候的色散要翻盘了，从开始传播到现在一直是正常啁啾主导，到这个点的时候，色散已经把啁啾基本上补偿完毕，脉冲中心部分基本上没有瞬时频率的变化。此时通过计算得到色散长度小于非线性长度，也说明了继续传播后色散开始主导。

##### 传输长度为 $3LP/4$ 时，光脉冲的时域、频域分布，以及啁啾情况：
![l3](distance43.png)
&emsp;&emsp;传输距离超过 $LP/2$ 之后，从演化图可以看出，光脉冲的时域迅速展宽，而频域迅速压缩变窄。这个过程有些类似反常色散下的弱 SPM 效应。同样，截取两点来看，当传播距离为 $3LP/4$ 时，可以看到脉冲的频谱虽然比入射脉冲的频谱宽，但是和传输距离为 $LP/2$ 的时候相比，能量更往中心集中。在 $LP/2$ 的地方，频谱中心为零，能量更往外分布一些。所以相对而言，频谱是被压缩了。时域上，虽然比入射脉冲要窄很多，但是和 $LP/2$ 处相比，也是变宽了，明显的特点是峰值功率下降了一半，啁啾也重新出现，但是变成了反常啁啾，前沿蓝移后延红移。啁啾可以说明这段确实是色散主导，也就是说，脉冲演化和反常色散下的弱 SPM 类似：时域变宽，频谱压缩，啁啾反常。

##### 传输长度为 $LP$ 时，光脉冲的时域、频域分布，以及啁啾情况：
![l4](distance74.png)
&emsp;&emsp;传输距离达到 $LP$ 时，脉冲又一次没有了啁啾，这说明 SPM 一直在慢慢的累积正常色散，而且 SPM 的累积速度加快，超过了色散产生反常啁啾的速度。这时候脉冲在时域和频谱似乎都恢复到输入时候的形状，和输入相比，时域频域的分布变化都很小。

##### 传输长度为 0 和 LP/2 时，色散长度分别为：
$$L_{D1}=\frac{T_0^2}{\left | \beta_2 \right | }= \frac{1e-24}{2.168e-26}=46.12$$
$$L_{D2}=\frac{T_0^2}{\left | \beta_2 \right | }= \frac{1.231e-26}{2.168e-26}=0.568$$

##### 传输长度为 0 和 LP/2 时，非线性长度分别为：
$$L_{NL1}=\frac{1}{\gamma P_0}= \frac{1}{0.09\times 1}=11.11$$
$$L_{NL2}=\frac{1}{\gamma P_0}= \frac{1}{0.09\times 4.09}=2.715$$

&emsp;&emsp;高阶孤子在传输过程中，脉冲形状和频谱都将发生变化，但是高阶孤子会在传输一段距离后周期性地恢复原来的形状，这段距离称为孤子的周期，以上振荡过程就是高阶孤子周期性演化的原因。