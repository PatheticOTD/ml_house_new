Фундаментальная часть RL, так как является единственным источником фидбэка для агента. 
Кумулятивная награда на каждом шагу t  может быть записана как: 
![[Pasted image 20250612175328.png]]
что эквивалентно записи: $$
R(\tau) = \sum\limits_{k = 0}^{\inf}{r_{t+k+1}}
$$
Но в реальности каждую награду регулируют следующим образом:
1. Задают значение скидки $\gamma$ от 0 до 1. Обычно от 0.95 до 0.99. Чем больше гамма, тем меньше скидка. Это позволяет агенту больше беспокоиться о труднодоступных наградах. Но с другой стороны, чем меньше гамма, тем больше скидка, а значит агент больше внимания будет уделять легким наградам.
2. Затем каждая награда будет  получит свою скидку на каждом шагу: ![[Pasted image 20250612180352.png]]