---
marp: true
paginate: true
# size: 4:3
# header: 'Header space'
# footer: 'Footer space'
title: 'ch03_位势高度与气压场'
# theme: nordic-beamer
theme: 'beamer'
---
<!-- page_number: true -->

<h1>位势高度与气压场</h1>

<br>

> 葛朝霞等，__气象学与气候学教程__，中国水利水电出版社（第2版）
>
> - 1.4. 大气静力学方程及其应用
>
> - 1.5.2 气压与气压场
> 
> - 4.1. 作用在气块上的力
> 
> - 4.4. 自由大气中的风
> 
> - 4.5 热成风

<br>

孔冬冬，__kongdongdong@cug.edu.cn__

办公室：环境学院416

中国地质大学大气科学系 · 武汉

---
<style scoped>
/* h2 { color: black;} */
</style>

<h2>QA</h2>

> 假设A、B两点，分别是冷空气和暖空气，地表气压相同

1. <span style='color:blue'>冷空气</span>、<span style='color:red'>暖空气</span>，哪个气压下降快？

2. 这意味着什么？

![bg right:65% 90%](images/ch03_位势高度与气压场/冷暖-气压下降快慢.png)  

---

# 1. 位势高度<span style='color:red'>（重点）</span>


定义：单位质量物体从海平面移动到$z$高度处所做的功$\Phi$，称为**重力位势**（简称位势$\Phi$）；__位势高度__$H=\Phi/g_0$，其中：
<br>

$$
\Phi = \sum_{0}^{z}{g_\phi dZ}
$$

- $g_0$: 重力加速度<span style='color:red'>__常数__</span>，$g_0=9.80665 J/kg$，<u>**不随**</u>纬度、垂直高度的变化而变化

- $g_\phi$: 物理学中的重力加速度，<u>**随**</u>纬度、垂直高度的变化而变化

<br>

---

## 1.1. 位势高度$H$与几何高度$Z$的差别

位势高度近似等于几何高度。**不同之处在于：**

- 位势高度$H=\Phi/g_0$，$g_0$为常数；
  
- 几何高度$Z=\Phi/g$，$g$随纬度、垂直高度的变化而变化。

> 位势高度不再考虑重力加速度随<u>**纬度**</u>与<u>**高度**</u>的变化。

<br>

**H和Z的换算**
$$
H = \frac{1}{g_0}\sum_{0}^{z}{g_\phi dZ}, ~~
g_0 dH = g_\phi dZ, ~~(g_\phi: 纬度\phi处的重力加速度，也写作g)
$$

从上式可以看出，位势高度$H$仅和$\phi$和$Z$相关，<span style='color:red'><u>和质量无关</u></span>。

<span style='color:red'>根据上面的定义，你能想象出位势高度和温度之间的关系吗？</span>

---

## 1.2. 位势高度的使用


- __等压面对应的位势高度、位势高度距平__：如500hPa位势高度、500hPa位势高度距平；
  
- **位势高度厚度**：如1000hPa-500hPa位势高度厚度

---

![bg right:60% 90%](images/ch03_位势高度与气压场/位势高度_网站地址.png)  

- 知乎，如何找天气图，<https://www.zhihu.com/question/63785418/answer/2687416982>

- tropicaltidbits，<https://www.tropicaltidbits.com/analysis/models/?model=ecmwf&region=ea&pkg=z500a>


---

# 2. 位势高度的应用

1. 气压高低
    > <u>*位势高度*</u>高（低）意味着同一平面上该点的气压也偏高（低）

2. 大气层平均虚温；
    > 根据压高公式，<u>*位势高度厚度*</u>与虚温$T_v$正相关

3. 风向（平行于等高线）；
    > 气压梯度力和科氏力的影响下，风向平行于<u>*等位势高度线*</u>；摩擦力影响下，逆时针偏转15°~30°

4. 环流形式与天气系统
    > 环流形式，如高低压系统（气旋、反气旋）、槽脊（槽前脊后阴雨）；
    > 天气系统，如副高、南亚高压、阻塞高压、切断低压、冷涡

5. 辐合辐散

---

## 2.1. 位势高度与气压高低

- 气压场：空间点气压组成的场。
  
- 等压面：3维空间中，气压相同的平面。
  
- 等高线：2维空间中，等压面上的等位势高度线。

![h:11.5cm](images/ch03_位势高度与气压场/Figure1_气压场示意图.png)  

<!-- ![bg right:50% 90%](images/ch03_位势高度与气压场/空间压强场.png)   -->

<!-- ![bg bottom:70%](images/ch03_位势高度与气压场/等压面与等高线关系.png)   -->

---

![](images/ch03_位势高度与气压场/Figure2_位势高度与气压01.png)  

---

![](images/ch03_位势高度与气压场/Figure2_位势高度与气压02.png)  

---

<h3>14 Nov, 2022</h3>

![w:26cm h:15cm](images/ch03_位势高度与气压场/位势高度距平-01.png)  

<https://www.tropicaltidbits.com/analysis/models/?model=ecmwf&region=ea&pkg=z500a&runtime=2021112112&fh=24>

---


## 2.2. 位势高度与大气层平均虚温


### 2.2.1. 理论基础

<h4>1. 液体的压力（高中）：</h4>


$$
P = \rho g h
$$

<h4>2. 理想气体状态方程</h4>

$$
\begin{align*}
pV &= nR^*T \\
p &= \rho R T \\
%  &= \rho R_d T_v \\
\end{align*}
$$

---

<!-- $$
T_v = T (1 + 0.378 \frac{e }{p})
$$ -->

![bg right:50% 90%](images/ch03_位势高度与气压场/大气静力平衡.png)  

<h4>3. 大气静力平衡</h4>

(1) **气压**
$p_1$ -> $p_2$：$p_2 = p_1 + \frac{\partial p}{\partial z} \delta z$
<br>

(2) **重力**

厚度为$\delta z$的小气柱受到的重力：$G = -\rho g \delta z$，方向垂直向下。

<br>

二者作用下，气体平衡状态时：

$$
-\rho g \delta z = \frac{\partial p}{\partial z} \delta z \\
\\
g = - \frac{1}{\rho} \frac{\partial p}{\partial z} \\
$$

微分形式：<span style='background-color:yellow'>$dp = - \rho g dz = - \rho g_0 dH$</span>

---

### 2.2.2. 位势高度厚度

> 为获得整层气柱中气压与高度之间的精确关系，采用积分进行求解

$$
\frac{dp}{dz} = - \rho g = -\frac{g~ p}{R_d T_v} \\
dp / p = -\frac{g~ dz}{R_d T_v}
$$

从$p_1$ -> $p_2$过程，对上式进行积分求解:

$$
\begin{align*}
\int_{p1}^{p2} dp / p &= \int_{z_1}^{z_2}-\frac{g dz}{R_d T_v} \\

ln\frac{p_2}{p_1} &= -\frac{g (z_2 - z_1)}{R_d \overline{T_v}} \\

\Delta z = z_2 - z_1 &= \frac{R_d \overline{T_v}}{g} ln\frac{p_1}{p_2}
\end{align*}
$$


---


把$g$换为$g_0$（$g dZ = g_0 dH$）即可得到：

$$
\Delta z = z_2 - z_1 = \frac{R_d \overline{T_v}}{g} ln\frac{p_1}{p_2} \\
\Delta H = H_2 - H_1 = \frac{R_d \overline{T_v}}{g_0} ln\frac{p_1}{p_2}
$$

> 此公式可以反映<span style='background-color:yellow'>位势高度厚度</span>的含义，$\Delta H$反映了$H_1$~$H_2$范围内气柱的平均虚温。

__1000hPa~500hPa位势高度厚度__

1. ≤5,100: 北极气团（ arctic air ）

2. ≥5,700: 热带气团（ tropical air ）

3. 5,400: 极地气团（ polar air ）与中纬度气团（ mid-latitude air ）的分界线；也是雨、雪的分界线。

<https://www.weather.gov/source/zhu/ZHU_Training_Page/Miscellaneous/Heights_Thicknesses/thickness_temperature.htm>

---

<h3>推论：</h3>

$$
\Delta H = H_2 - H_1 = \frac{R_d \overline{T_v}}{g_0} ln\frac{p_1}{p_2}
$$

- 位势高度距平偏高：大气层平均虚温$T_v$偏高
   <br>
  > 因此，通过看位势高度距平，可以得出空间上哪些地区温度偏高（<span style='color:red'><u>热浪</u></span>）、哪些地区温度偏低（<span style='color:blue'><u>寒潮</u></span>）。

---

<h3>22 Nov, 2021</h3>

![w:30cm h:13cm](images/ch03_位势高度与气压场/示例-位势高度厚度01.png)  

<https://charts.ecmwf.int/products/medium-thickness-mslp?base_time=202211130000&projection=opencharts_eastern_asia&valid_time=202211150600>

---

## 2.3. 位势高度与风向

- 不考虑摩擦力的情况下，地转风平行于等位势线；

- 考虑摩擦力的情况，风向逆时针偏转15°~30°。

---

### 2.3.1. 作用在气块上的力

#### 2.3.1.1. 气压梯度力 (pressure gradient force, PGF)

   > 由高压指向低压，等压线约密集，PGF越大。

$$
\begin{align*}
PGF &= - \frac{1}{\rho} \nabla p \\
    &= - \frac{1}{\rho} (
            \frac{\partial p}{\partial x} i +
            \frac{\partial p}{\partial y} j +
            \frac{\partial p}{\partial z} k)
\end{align*}
$$

- 水平方向的分量

$$
\begin{align*}
PGF_h &= - \frac{1}{\rho} \nabla_h p \\
    &= - \frac{1}{\rho} (
            \frac{\partial p}{\partial x} i +
            \frac{\partial p}{\partial y} j)
\end{align*}
$$

![bg right:38% 90%](images/ch03_位势高度与气压场/气压梯度力-01.png)  


---

#### 2.3.1.2. 科氏力 (Coriolis Force, CF)


![h:16cm](images/ch03_位势高度与气压场/科氏力-01.png)  

---

#### 2.3.1.3. 科氏力 (Coriolis Force, CF)
   > 由于地球自转，所形成的一种虚假的力。
   > 垂直于$v$，北半球向右；南半球向左。

$$
\begin{align*}
CF_h &= 2 \Omega v sin \phi \boldsymbol{i} - 2 \Omega u sin \phi \boldsymbol{j} \\
     &= 2 \Omega sin \phi(v \boldsymbol{i} - u \boldsymbol{j})\\
     &= -f \boldsymbol{k} × V_h, (f = 2 \Omega sin \phi)
\end{align*}
$$

- $\Omega$: 地球自转的角速度
- $\phi$: 纬度
- $V_h$: 水平方向风速

![bg right:50%](images/ch03_位势高度与气压场/科氏力.png)  

---

#### 2.3.1.4. 摩擦力


摩擦力的作用，使原本的风向，逆时针偏转15°~30°左右。(<u>章节 4.6</u>)

<br>

- 导致高低压中心发生辐散、辐合；

   > 没有摩擦力，台风可能就不会产生降水；

![bg right:50% 90%](images/ch03_位势高度与气压场/摩擦力-01.png)  

---

### 2.3.2. 风

#### 2.3.2.1. 地转风

水平<u>气压梯度力</u>PGF和<u>科氏力CF</u>二者受力均衡，平衡状态下所形成的风。

<br>

<span style='color:red'>__重点：__</span>

- 风向平行于等压线；
  
- 背风而立，__高压在右、低压在左__（主要是科氏力右偏所影响）。

![bg right:50% h:8cm](images/ch03_位势高度与气压场/地转风.png)  

---

<h4>地转风公式</h4>

- 气压梯度力

$$
\begin{align*}
PGF_h & = - \frac{1}{\rho} (
            \frac{\partial p}{\partial x} i +
            \frac{\partial p}{\partial y} j)
        = - \frac{1}{\rho} \nabla_h p
\end{align*}
$$

- 科氏力

$$
\begin{align*}
CF_h &= 2 \Omega v sin \phi \boldsymbol{i} - 2 \Omega u sin \phi \boldsymbol{j} \\
     &= 2 \Omega sin \phi(v \boldsymbol{i} - u \boldsymbol{j})\\
     &= -f (v \boldsymbol{i} - u \boldsymbol{j})
     = -f \boldsymbol{k} × V_h, (f = 2 \Omega sin \phi)
\end{align*}
$$

可以得到

$$
\begin{align*}
- \frac{1}{\rho} \frac{\partial p}{\partial x} + fu = 0 \\
- \frac{1}{\rho} \frac{\partial p}{\partial y} - fv = 0
\end{align*}
$$

即：$V_g = V_h = -\frac{1}{f \rho} \nabla_h p  ×  \boldsymbol{k}$

---

- z坐标中（$t, x, y, z$）

$$
V_g = -\frac{1}{f \rho} \nabla_h p  ×  \boldsymbol{k}
$$

- p坐标中（$t, x, y, p$）

$$
V_g = -\frac{g_0}{f} \nabla_p H  ×  \boldsymbol{k}
$$

> $H$: 位势高度

> 关于公式的解释，详见章节4.4, Eq. 4-33

采用位势高度的形式，更容易解释<span style='background-color:yellow'>__寒潮时的大风__</span>和<span style='background-color:yellow'>__高空急流__</span>  

---

#### 2.3.2.2. 梯度风

气体做圆周运动而形成的风。

<br>

**科氏力影响下：**

- 高压中心（反气旋）：顺时针转动

- 低压中心（气旋）：逆时针转动。

![bg right:55% h:12cm](images/ch03_位势高度与气压场/梯度风-01.png)  

<span style='color:red; background-color:yellow'>**注意：南半球旋转方向刚好相反！**</span>

---

#### 2.3.2.3. 风向的作用

- 气温：冷平流 or 暖平流
  
- 水汽：陆地来的风 or 海洋来的风，水汽增加 or 减小？

<br>

:::info:应用重点

- 已知等位势高度线，判断风向（从高压指向低压、右偏），高低压中心（顺时针、逆时针），对气温、水汽的影响；

- 已知风向，判断高低压中心。

:::


---

## 2.4. 天气系统与环流型

<!-- > 这里我们先主要讲<u>环流型</u> -->

<style scoped>
p { margin: 0.4em 0em 0.2em 0em }
</style>

__等压面：__ 气压相等的面；

__等高线：__ 位势高度相等的点的连线；
<hr>

__槽脊__：槽前脊后阴雨，反之高温、干旱

__高压中心（反气旋）__：高空辐合、低空辐散，干旱

__低压中心（气旋）__：高空辐散、低空辐合，阴雨

---

### 2.4.1. 槽脊

- <span style='color:blue'>__低压槽（槽线）__</span>
  
   等高线中曲率最大的点的连线，开口指向低压中心。

- <span style='color:red'>**高压脊（脊线）**</span>

  等高线中曲率最大的点的连线，开口指向高压中心。

![bg right:56% 100%](images/ch03_位势高度与气压场/槽脊定义.png)  

---

### 2.4.2. 高低压中心

![h:16cm](images/ch03_位势高度与气压场/高低压中心-特征.png)  

---

## 2.5. 辐合、辐散

- __辐合(convergence)__：物质积累。有如下类型：
  - 相对而行的风场；
  - 风速从快到慢；
  - 气旋；逆时针转动，摩擦力影响，风向逆时针偏转30°左右，物质向内积累

  > 物质积累，则中心气压变高，有向上运动的趋势，向上运动则产生对流，有利于成云致雨。

  <!-- 、向上运动（对流） -->

![](images/ch03_位势高度与气压场/辐合.png)  

---

- __辐散(divergence)__：物质丢失。有如下类型：
  - 相背而行的风场；
  - 风速从慢到快（物质丢失）
  - 反气旋；顺时针转动，摩擦力影响，风向逆时针偏转30°左右，物质向外流失
  
  > 物质丢失，则中心气压变低，有向下运动的趋势，空气向下运动不易降水

![](images/ch03_位势高度与气压场/辐散.png)  

  <!-- 、中心气压下降、向下运动 -->

---

### 2.5.1. 高空与地表的辐合、辐散

> <span style='color:red'>天之道，损有余而补不足</span>

- 地表辐合、高空辐散；
  
- 反之则，地表辐散、高空辐合。

![](images/ch03_位势高度与气压场/地表高空-辐合辐散-01.png)  

---

![h:19cm](images/ch03_位势高度与气压场/地表高空-辐合辐散-02.png)  

---

### 2.5.2. 槽脊的辐合、辐散

![w:15cm h:10cm](images/ch03_位势高度与气压场/槽脊-辐合辐散.png)  


<style scoped>
p { 
  margin: 0.4em 0em 0.4em 0em;
  font-size: 30px
}
</style>

- 高空槽前脊后：
  > 高空幅散、地表辐合，阴雨区。

- 高空槽后脊前：
  > 高空辐合、地表幅散，晴朗区。

![bg right:50% h:18cm w:14cm](images/ch03_位势高度与气压场/槽脊-辐合辐散02.png)  

---

<h4>原理：</h4>

![h:16cm](images/ch03_位势高度与气压场/槽前脊后原理.png)  

---

<h2>总结：位势高度的作用</h2>

1. 气压高低
    > <u>*位势高度*</u>高（低）意味着同一平面上该点的气压也偏高（低）

2. 大气层平均虚温；
    > 根据压高公式，<u>*位势高度厚度*</u>与虚温$T_v$正相关

3. 风向（平行于等高线）；
    > 气压梯度力和科氏力的影响下，风向平行于<u>*等位势高度线*</u>；摩擦力影响下，逆时针偏转15°~30°

4. 环流形式与天气系统
    > 环流形式，如高低压系统（气旋、反气旋）、槽脊（槽前脊后阴雨）；
    > 天气系统，如副高、南亚高压、阻塞高压、切断低压、冷涡

5. 辐合辐散

---

<h1>谢谢！欢迎沟通交流！</h1>

孔冬冬，**<kongdongdong@cug.edu.cn>**

办公室：环境学院416

中国地质大学大气科学系 · 武汉

<br>

:::block
课件地址见：<https://github.com/CUG-hydro/class2022_CUG_HydroMet>
:::
