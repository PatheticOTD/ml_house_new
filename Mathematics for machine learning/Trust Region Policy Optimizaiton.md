#on_policy #model_free

Рассмотрим MDP, определенного кортежем (S A P r p_0  $\gamma$) где S - states set, A - finite acitons set, P: SxAxS - [[Transition probability distribution]]

В reinforcement learning, если просто на каждом шаге делать градиентный апдейт политики (policy gradient), можно получить **резкие скачки стратегии** → это ломает обучение и приводит к нестабильности.

**Trust Region Policy Optimization** (TRPO) вводит _ограничение_ на изменение политики между итерациями, чтобы гарантировать **монотонный рост вознаграждения** и избежать "разрушительных" апдейтов.