# General principle to implement different strategies:

## Understand what is payoff

Max return最大收益

Max lost最大亏损

Break even

Expired curve到期收益曲线 横轴是到期日标的价格，纵轴是最终盈亏，画出不同标的价格下策略赚或亏多少。

## Hand written strategy spec

legs
├── option_type
├── strike行权价
├── expiry到期日
└── quantity

Write backtest

Entry

Exit

Positioning sizing

Transaction cost

Expiration

Draw the pnl result

P&L

Drawdown

Hedge effectiveness

Premium cost

01  Long Call
      ↓
02  Long Put
      ↓
03  Covered Call
      ↓
04  Cash-Secured Put
      ↓
05  Protective Put
      ↓
06  Bull/Bear Vertical Spread
      ↓
07  Put Spread
      ↓
08  Collar
      ↓
09  Straddle
      ↓
10  Strangle
      ↓
11  Calendar / Diagonal
      ↓
12  Iron Condor / Butterfly

Covered Call
= Long ETF + Short Call

Protective Put
= Long ETF + Long Put

Collar
= Long ETF + Long Put + Short Call

Put Spread
= Long Put + Short Put
