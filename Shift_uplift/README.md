# ШИФТ Курс "Аплифт". 
# Предсказать, кому отправить СМС, чтобы склонить к покупке.

Есть данные о том, кто из клиентов именно тот, кто без СМС не купит, а с СМС - купит!  
Предстоит из всех test-клиентов указать вероятность того, что клиент купит только при коммуникации (не купит без нее).  
Оценка модели будет делаться по метрике Gini:

**Gini = 2 * AUC - 1**, где AUC - это ROC AUC.

Для построения модели, участникам предоставляется обучающий набор клиентов train.csv с информацией о наличии коммуникации (treatment_flg) и совершение покупки (purchased).

Необходимо для каждого клиента из тестовой выборки test.csv предсказать target, который равен 1, если после коммуникации покупка совершена и если без коммуникации покупка не совершена, 0 в других случаях.
[Описание конкурса](https://www.kaggle.com/competitions/uplift-shift-23/overview)
