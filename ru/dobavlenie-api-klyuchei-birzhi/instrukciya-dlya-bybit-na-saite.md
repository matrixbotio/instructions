---
description: Рассмотрим как получить API ключ на бирже Bybit для торговли.
---

# Инструкция для Bybit (на сайте)

Если у тебя еще нет аккаунта на Bybit, [воспользуйся этой ссылкой](https://get.matrixbot.io/share-profit/bybit), чтобы создать аккаунт и снизить комиссию на 10%.

Переходим к странице [API Management.](https://www.bybit.com/app/user/api-management)

Справа вверху страницы находим кнопку "Create New Key", нажимаем на нее.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-08-54.png" alt=""><figcaption></figcaption></figure>

Далее выбираем "System-generated API Keys":

<figure><img src="../.gitbook/assets/bybit_4.jpg" alt="" width="351"><figcaption></figcaption></figure>

Тип ключа "API Transaction". Имя для ключа можно придумать любое.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-11-05.png" alt="" width="375"><figcaption></figcaption></figure>

**Ниже в разрешениях ключа выбираем "Read-Write",** чтобы боты могли не только получать данные о балансе, но и могли размещать ордера.

**Выбираем "No IP restriction".** Так как на платформе IP меняется периодически.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-12-35.png" alt="" width="366"><figcaption></figcaption></figure>

Далее отмечаем разрешения ключу. Отмечаем галку у SPOT -> Trade.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-15-20.png" alt="" width="563"><figcaption></figcaption></figure>

И отмечаем галку Exchange -> Convert, Exchange History.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-15-50.png" alt="" width="563"><figcaption></figcaption></figure>

Готово, жмем кнопку "Submit", чтобы закончить создание API ключа.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-25-13.png" alt=""><figcaption></figcaption></figure>

Отображается окошко с данными API ключа. Записываем публичный и приватный ключи.

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-17-24(1).png" alt="" width="563"><figcaption></figcaption></figure>

Затем добавляем созданный ключ [в разделе API keys](https://matrixbot.io/apikeys) на сайте MatrixBot:

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-18-10(1).png" alt="" width="563"><figcaption></figcaption></figure>

Жмем "Connect", ключ будет проверен на необходимые доступы и добавится в аккаунт.

Проверить ключ можно кнопкой "Balance":

<figure><img src="../.gitbook/assets/Screenshot_2024-10-17_14-20-38(1).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
API ключ на бирже имеет определенный срок действия. 30 или 90 дней, затем его надо продлять.

Для этого достаточно зайти в список своих API ключей на бирже, нажать на "Edit IP access" и сохранить ничего не меняя, тогда ключ продлит свое действие и его не придется менять в работающих ботах.
{% endhint %}

Готово! Можно запускать ботов!
