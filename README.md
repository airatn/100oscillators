# Model of wave propagation in a system of 100 identical interconnected bodies with loose ends
Предметом исследования является, многокомпонентная, переходная по простоте, модель распространения волн в системе из 100 взаимосвязанных тел. Такого рода процессы мы можем наблюдать в многочисленных физических явлениях таких как водяные, звуковые, сейсмические или электромагнитные волны. Основное свойство данных систем, это перенос энергии без переноса вещества, так как при распространении волны частицы среды не двигаются вместе с волной, а колеблются около своих положений равновесия.

Поперечная волна - это форма волны, в которой частицы среды колеблются относительно своего среднего положения, перпендикулярного направлению движения волны - на рисунке показаны стрелками. Среда состоит из [тел связанных только с соседними узлами пружинами](https://en.wikipedia.org/wiki/Damping)  - упругими объектами, накапливающих механическую энергию.

<img src="https://drive.google.com/uc?export=view&id=1V4N2aD6LOos3hWvFA3T09kTQWGxnWALb" width="900">

Данная модель, для случаев незакрепленных концов описывается следующей системой дифференциальных уравнений:


$$\begin{cases}
  \ddot y_1\cdot m_1+c_1\cdot\dot y_1+k_1\cdot \left(y_1-y_2\right)=0\\
  \ddot y_2\cdot m_2+c_2\cdot\dot y_2+k_1\cdot \left(y_2-y_1\right)+k_2\cdot\left(y_2-y_3\right)=0\\
  ...\\
  \ddot y_{99}\cdot m_99+c_99\cdot\dot y_99+k_99\cdot \left(y_99-y_98\right)+k_100\cdot\left(y_99-y_100\right)=0\\
  \ddot y_100\cdot m_100+c_100\cdot\dot y_100+k_100\cdot \left(y_100-y_99\right)=0
\end{cases}$$
