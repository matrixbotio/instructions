---
description: Here we will analyze the most common mistakes that occur during trading.
---

# Error texts and what to do

<details>

<summary>Insufficient balance / not enough balance</summary>

May occur when placing an order. It is necessary to check:

* are there enough coins on the balance to place an order;

- whether the bot has been assigned the correct API key from an account that has funds;

* funds must be in a trading account ("Spot", "Unified Trading" - may be called differently);

- if short trading is selected, the bot deposit is calculated in coins, not in USDT (USDC, etc.), you need to pay attention to the number of coins on the balance.

</details>

<details>

<summary>Unmatched IP, please check your API key's bound IP addresses.</summary>

This error may occur if the IP address has a whitelist enabled. The exchange API key must have "No IP Restrictions".

</details>

<details>

<summary>API key not found</summary>

This error may occur when running a bot that was purchased on the Market.

Common reason: the bot has not been assigned an API key.

* You need to go to the bot editing.
* Assign an API key to it.
* Save the bot.
* Reset the bot error (stop button).

And you can run the bot again. If the problem is not solved, you can try to clone the bot.

</details>

<details>

<summary>Invalid API-key, IP, or permissions for action</summary>

The API key does not have the required permissions or the "Read Only" mode is selected. You must [follow the instructions](../adding-exchange-api-keys/) for creating and configuring API keys.

</details>

<details>

<summary>Order value exceeded lower limit</summary>

Occurs when the minimum order size on the exchange has been updated and is now larger than the bot order. It is worth trying to change the bot settings to increase the size of the 1st grid order.

This can be done by:

* increasing the bot deposit,
* reducing the number of grid orders,
* decreasing the Factor value.

</details>
