---
description: Здесь разбираем самые частые ошибки, которые происходят во время торговли.
---

# Тексты ошибок и что делать

<details>

<summary>Insufficient balance / not enough balance</summary>

Может возникать при размещении ордера. Необходимо проверить:

* хватает ли монет на балансе для размещения ордера;
* присвоен ли боту корректный API ключ от счета, на котором есть средства;
* средства должны быть на торговом счете ("Spot", "Unified Trading" - может называться по разному);
* если выбрана шорт-торговля, то депозит бота считается в коинах, а не в USDT (USDC и тд), надо обратить внимание на количество монет на балансе.

</details>

<details>

<summary>Unmatched IP, please check your API key's bound IP addresses.</summary>

Такая ошибка может возникнуть, если для IP адреса включен белый список адресов. Необходимо, чтобы у API ключа биржи было "No IP Restrictions".

</details>

<details>

<summary>API key not found</summary>

Эта ошибка может возникнуть при запуске бота, который был куплен на Маркете.

Частая причина: боту не назначен API ключ.

* Необходимо зайти в редактирование бота.
* Назначить ему API ключ.
* Сохранить бота.
* Сбросить ошибку бота (кнопка остановки).

И можно запускать бота снова. Если проблема не решилась, можно попробовать склонировать бота.

</details>

<details>

<summary>Invalid API-key, IP, or permissions for action</summary>

API ключу не заданы необходимые разрешения или выбран режим "Read Only". [Необходимо воспользоваться инструкцией](../dobavlenie-api-klyuchei-birzhi/) по созданию и настройке API ключей.

</details>
