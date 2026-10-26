## Дополнение к ячейке «Свойства оценки»

### Асимптотическая нормальность

Поскольку для любого $n$ верно $\sqrt n(\widehat\theta-\theta)\sim\mathcal N(0;1)$, то

$$
\boxed{\sqrt n(\widehat\theta-\theta)\xrightarrow{d}\mathcal N(0;1)}
$$

То есть оценка также асимптотически нормальная

---

## Асимптотическая эффективность

Логарифм плотности равен

$$
\ln f_\theta(x)=\ln\frac{3x^2}{\sqrt{2\pi}}-\frac{(\theta-x^3)^2}{2}
$$

Найдём производную по $\theta$

$$
\frac{\partial}{\partial\theta}\ln f_\theta(x)=x^3-\theta
$$

Информация Фишера одного наблюдения

$$
I(\theta)=\mathbb E\left[\left(X^3-\theta\right)^2\right]=\operatorname{Var}(X^3)=1
$$

Для независимой выборки объёма $n$ информация Фишера складывается

$$
I_n(\theta)=nI(\theta)=n
$$

По неравенству Рао-Крамера дисперсия любой несмещённой оценки параметра $\theta$ не меньше

$$
\operatorname{Var}(\widehat\theta)\geq\frac{1}{I_n(\theta)}=\frac1n
$$

Ранее мы получили

$$
\operatorname{Var}(\widehat\theta)=\frac1n
$$

Таким образом, оценка достигает нижней границы Рао-Крамера и является эффективной при любом $n$, а значит и асимптотически эффективной
