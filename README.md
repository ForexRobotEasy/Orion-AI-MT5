# Orion AI MT5

Orion AI MT5 is a multi-currency Expert Advisor that implements a new algorithm to enhance the performance and effectiveness of trading. This powerful tool is designed for forex traders and focuses on four major currency pairs using hourly chart candles to determine trading decisions. The algorithm utilizes a time-tested strategy and maintains an unrivaled risk-reward ratio, while avoiding dangerous money management methods like martingale.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-orion-ai-mt5-the-ultimate-forex-software-with-a-new-algorithm/). Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Specifications

- Multi-currency Expert Advisor
- Enhanced performance and effectiveness
- Powerful trading tool for forex traders
- Focus on four major currency pairs
- Use hourly chart candles for trading decisions
- Avoid dangerous money management methods
- Time-tested strategy with unrivaled risk-reward ratio

## Usage

To use this code, follow the steps below:

1. Include the necessary trading functions by adding the following line at the beginning of your code:

```cpp
#include <Trade\Trade.mqh>
```

2. Define the constant variables for the four major currency pairs by adding the following lines:

```cpp
const string SYMBOL_1 = 'EURUSD';
const string SYMBOL_2 = 'GBPUSD';
const string SYMBOL_3 = 'USDJPY';
const string SYMBOL_4 = 'AUDUSD';
```

3. Implement the `OnStart()` function to start the program. This function will loop through each currency pair, check hourly chart candles, and apply the time-tested strategy if conditions are met. The code for this function is provided below:

```cpp
void OnStart()
{
   // Loop through each currency pair
   for(int i=0; i<4; i++)
   {
      string symbol = GetSymbolByIndex(i);
      
      if(symbol == SYMBOL_1 || symbol == SYMBOL_2 || symbol == SYMBOL_3 || symbol == SYMBOL_4)
      {
         // Check hourly chart candles
         if(CheckHourlyCandles(symbol))
         {
            // Apply time-tested strategy
            ApplyStrategy(symbol);
         }
      }
   }
}
```

4. Implement the `CheckHourlyCandles()` function to check the hourly chart candles for a given symbol. This function should return `true` if the conditions are met, and `false` otherwise. Add your code to check the hourly chart candles inside this function.

5. Implement the `ApplyStrategy()` function to apply the time-tested strategy for a given symbol. Add your code to apply the strategy and maintain the unrivaled risk-reward ratio inside this function.

6. Implement the `GetSymbolByIndex()` function to get the symbol name by index. This function should return the symbol name as a string. Add your code to get the symbol name by index inside this function.

## Author

Forex Robot Easy Team

Website: [https://www.forexroboteasy.com](https://www.forexroboteasy.com)
