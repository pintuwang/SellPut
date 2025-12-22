SELL-PUT ANALYZER DECODER – QUICK REFERENCE
============================================

1.  WHAT THE DECODER DOES
-------------------------
For any entered short-put trade the page returns:
- Live market data (price, IV, Greeks)
- Risk metrics (prob OTM, breakeven, max loss)
- Income metrics (premium, daily $, annual %)
- Volatility context (IV percentile vs 1 yr, vol premium vs 30 d HV)
- Expected value (statistical edge)

All numbers update in real time; IV can be overridden if chain data fail.

2.  FIELD-BY-FIELD DECODER & ACTION GUIDE
-----------------------------------------
(≈ ranges for a 30-45 DTE US equity option)

FIELD               TYPICAL RANGE        WHAT IT TELLS YOU               LIKELY MARKET CONTEXT / ACTION
----------------------------------------------------------------------------------------------------------------
Position Delta      0.05 – 0.35          ≈ % chance of being ITM        Low = deep OTM, high cushion.  
                    0.35 – 0.50          ATM strike                     Roll or accept assignment plan.
                    > 0.50               ITM already                    Bear gap or rally; roll up/out.

% OTM               > 10 %               Comfortable cushion            Low-vol or far strike.
                    3 – 10 %             Moderate cushion               Normal ATM/OTM.
                    < 3 %                Razor-thin                     High vol or near expiry; roll early.

Premium             $0.30 – $1.00        “Normal” income              Low IV / far strike.
                    $1.00 – $3.00        Fat premium                  High IV or close strike; size smaller.
                    > $3.00              Crash-level                  Earnings/news; avoid or hedge.

Days to Exp         7 – 45               Theta-decay sweet spot       Manage at 21 DTE or 50 % profit.
                    > 45                 Income diluted annually      Roll or take profits early.

Annual Ret          8 – 25 %             Decent yield                 Low-vol bull market.
                    25 – 60 %            Very high                    High IV or deep ITM; tail-risk present.
                    > 60 %               Red-flag rich                Crisis pricing; size tiny or wait.

Expected Val        +$50 – +$200         Edge in your favour          IV > realised vol.
                    −$200 – 0             Fair/fat premium             Accept if you manage early.
                    < −$500              Statistically under-paid     Reduce size or wait for IV crush.

IV                  15 – 35 %            Low/normal                   Bull quiet market.
                    35 – 60 %            Elevated                     Earnings / uncertainty.
                    > 60 %               Crash-level                  Hedge, smaller size, or sell later.

IV Percentile       < 30 %               Cheap vs history             Buyback calls / wait for vol rise.
                    30 – 70 %            Fair                         Standard entry.
                    > 70 %               Expensive vs history         Good time to **sell**; plan rolls.

Vol Premium vs HV   < −20 %              IV < recent realised         Option cheap vs own vol – caution.
                    −20 % – +20 %        Fair                         Normal entry.
                    > +20 %              IV fat vs realised           Favourable seller edge; monitor collapse.

Risk Level          Low                  High win-rate, low $ risk    Size normally.
                    Medium               Balanced                     Watch earnings / technical levels.
                    High                 Low win-rate or large $ risk Reduce size or hedge.

3.  QUICK ACTION CHECKLIST
--------------------------
A.  **IV pct > 70 % + Vol Prem > +20 % → SELL small, plan roll/up-out.**  
B.  **Delta > 0.40 on earnings week → avoid or hedge.**  
C.  **Expected Val < −$500 → size ½ normal or wait.**  
D.  **Annual Ret > 60 % → tail-risk present; take 25–50 % profit early.**  
E.  **21 DTE or 50 % profit → close or roll to next cycle.**  

Keep this txt beside the analyser – one glance tells you if the market is paying you **fairly** for the risk you’re short.
