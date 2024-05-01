# ⚙️ Creation and edit bots

{% embed url="https://youtu.be/7jfVoK4MFk8" %}

#### Long/Short&#x20;

Type of trading strategy. In `Long` mode, the bot places buy orders from top to bottom as the price decreases. As the price falls, the bot buys at cheaper and cheaper prices. When the price reverses, the bot sets a take profit order with a specified % of `profit`. Then, the lap will be closed and it starts again. In `Short` mode, on the contrary, orders go up in ascending order as prices rise and gradually sell so that it can buy back all amounts later at a lower cost to earn profits.

#### Bot name

Unique name for your bot not exceeding 20 characters.

#### Market API

To work with an exchange on behalf of you, your bot uses an API key that needs to be created in your account settings on that exchange. After creating an API connection, select Market API for your created API key. [How to Create API?](https://www.binance.com/en/support/faq/how-to-create-api-360002502072)

#### Pair

The trading pair in which your bot will trade.

#### Limit, %

The limit of funds allocated by you for trading on an exchange by this bot should have enough funds available in your account balance too because these should cover all orders set under `Orders` section above minimum order limits allowed by exchanges based on selected pairs like $10 for most pairs traded via Binance platform. **Important!** For spot markets during Short mode operation deposit (`limit`) must be active and correspondingly available within your balance held in Bitcoin or any other relevant cryptocurrency depending upon selected pair such as BTC/BUSD where deposit (`limit`) must be made through BTC only.

#### Reinvest, %

> 0-100%

The percentage of profit that will be reinvested into the limit bot, thus ensuring capitalisation of profits and accelerating the bot's income. However, it should be noted that a portion of the profits goes towards paying exchange fees and when 100% is specified, there may not be enough deposit for another lap.

#### Profit, %

The percentage of profit that the bot includes when setting a take profit order (profit from each lap). High profit increases earnings but also lengthens round times and makes closing laps more difficult. Optimal values are between 0.4%-0.8%.

#### Coverage, %

The price range starting from the current price that the bot must cover with an ordered grid. To choose optimal coverage values, it is convenient to use charts to assess how well-grid size matches typical price movements for pairs.

#### Offset, %

The first order's deviation from current prices used to improve entry efficiency by allowing execution of first orders with small "reserves" in case prices move in reverse.

#### Reset, %

Percentage change in price after which bots must pull grids back to current prices if prices move in other directions.

#### Sleep&#x20;

Sleep timer (seconds). Pause seconds following executing take-profit orders before beginning new lap as protection against entering markets too quickly after strong price movements.

#### Indicators

Starting bots using technical indicators helps evaluate market situations while excluding overbought or oversold moments on markets; bots use indicators to select advantageous market entry points; every lap starts waiting until all set-up indicator conditions are fulfilled; Indicators can be viewed on charts.

#### Orders

> Maximum 40

The number of `orders` in the grid. The overall deposit of the bot (`limit`) is divided by the number of orders. The more orders, the smoother the averaging and higher chance for take profit order execution. However, it is necessary to control that the minimum order (`min order`) does not fall below what is allowed. For most pairs on Binance exchange, this value is $10.

{% hint style="info" %}
**Deposit Loss** - estimate of deposit loss in % if all grid orders are executed.

**Last TP** - at what distance in % from the first order will be a take profit order after executing all grid orders. For example, if cover is 10%, and Last TP is 5%, this means that with these settings, the bot will catch a rebound of no less than 50% after a price drop of 10%.

**Min Order** - minimum order size in the grid. It's important to monitor that it doesn't go below what's allowed on an exchange as per their rules table for Binance where min order for most pairs should be $10.
{% endhint %}

#### Factor, %

Multiplier used to calculate orders. To achieve more effective averaging each subsequent order in a grid must be larger than its predecessor by some percentage called `Factor` %. If factor equals 20%, then every next position would be bigger than previous one by 20%. At zero percent all positions are equal-sized across entire range covered by grid `Orders` parameter limit regardless how many there were set up initially or subsequently added over time period specified.

#### ⚙️ Custom Factor, manual order size adjustment

On our platform, you can manually set the size of each order. To do this, simply adjust the % of the corresponding order, with the total sum of all orders remaining at 100%. When manually assigning orders, a `Custom` label will appear in the `Factor` field.

#### ARC, %

> Greater than 1%, or less than -1%

In the standard version ARC=1 and orders are equidistant from each other, but this can be changed by setting your own `ARC` value. A value greater than 1 brings initial grid orders closer together and stretches out later ones. A value less than -1 does the opposite.

#### ⚙️ Custom ARC, manual distance between orders adjustment

On our platform, you can manually set the distance between orders. To do this simply adjust the offset in % for each order. When manually assigning orders a `Custom` label will appear in the `ARC` field.

#### Notification settings

You can configure notifications to be sent via Telegram or email for various bot events. Chatbot [@MatrixIoBot](https://t.me/MatrixIoBot)

#### Management settings

Functionality will be added in future versions

#### ☁️  Presets&#x20;

For each configuration block you can save typical parameter sets and then load them later on.
