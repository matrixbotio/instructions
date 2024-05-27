---
description: Рассмотрим как получить API ключ на бирже Bybit для торговле на Spot рынке.
---

# Создаем API ключ на Bybit

Если у тебя еще нет аккаунта на Bybit, [воспользуйся этой ссылкой](https://get.matrixbot.io/share-profit/bybit), чтобы создать аккаунт и снизить комиссию на 10%.

По умолчанию Bybit открывает "unified account" счета для своих клиентов, поэтому необходимо создать sub-account, в котором получить API ключ к Spot рынку. Дело в том, что API ключи к "unified account" и "spot" - считаются как ключи к разным рынкам.

1. [Создаем sub-account](https://www.bybit.com/app/user/sub-account) для торговых ботов. Необходимо выбрать "Standart Subaccount".

<figure><img src="../.gitbook/assets/bybit_1.jpg" alt=""><figcaption></figcaption></figure>

2. Далее выбери тип - "Standart account".

<figure><img src="../.gitbook/assets/bybit_2.jpg" alt=""><figcaption></figcaption></figure>

3. В созданном sub-account найди ссылку "API Management":

<figure><img src="../.gitbook/assets/bybit_3.jpg" alt=""><figcaption></figcaption></figure>

4. Создай API ключ для управления этим счетом. В качестве типа API ключа выбери "System-generated API Keys":

<figure><img src="../.gitbook/assets/bybit_4.jpg" alt=""><figcaption></figcaption></figure>

5. Выставь следующие разрешения ключу, чтобы бот мог запрашивать баланс, информацию об ордерах и производить торговлю:

<figure><img src="../.gitbook/assets/bybit_5.jpg" alt=""><figcaption></figcaption></figure>

6. Сохрани полученные публичный и приватный ключи. Добавь их к своему аккаунту в MatrixBot [в разделе API keys.](https://matrixbot.io/apikeys)

{% hint style="info" %}
API ключ на бирже имеет определенный срок действия. 30 или 90 дней, затем его надо продлять. Для этого достаточно зайти в список своих API ключей на бирже, нажать на "Edit IP acess" и сохранить ничего не меняя, тогда ключ продлит свое действие и его не придется менять в работающих ботах.
{% endhint %}

Готово! Можно запускать ботов!
