
## Fin Formulas
Income , Expense , Asset , Liability 
Income - Expense = Cash Flow
Assets - Debts = Net Worth
 
**Net Worth**
NW = Age * Pretax Income / 10 
 
Tax 
Tax Planning = ELSS + NPS + PPF
Post Office Investment = FD + SCSS 
 
CAGR
((5000/1000))^(1/10))-1
How to calculate average/compound annual growth rate in Excel?
Int Rate and Tax 
Int Rate - (Int Rate * Tax rate)
= 10 - 10 * 30% = 10 - 10 * 0.3 = 7
 
# How much we need 
= a* (1+r) ^ n   |  = 1200000 * ( 1+7% ) ^ 15 = 33 10 838 
7 % inflation , 15 yr child education , Current Val 12l
 
# How much to invest 
= PMT(rate , nper , PV , FV) 
= PMT( 12%/12 , 15.12 , 0 , 33 10 838)
 
# How much to invest in stock 
100 -  Current Age of = % in Equity
@30 - 70% , @60- 40%
 
 
 
# Rule of Thumb
2x 72 / 9 % = 8 years ( 72 / r% ) 
3x 114/ 3 % = 38 years ( 114 / r% ) 
4x  144  / 12 % = 12 years ( 144 / r% ) 
 
XIRR
 
XIRR (B14:B15,A14:a15)
 
01-Jan-2010
-10000
01-Jan-2012
12000

 
1. Compound Interest 
Formula: A = P * (1+r/t) ^ (nt)
Total amount you will receive after 10 years will be  = 1,00,000(1+0.1) ^10 = 2,59,374.25
 
2. Post Tax Return
Formula = Interest rate - (Interest rate*tax rate)  = 10-(10*30%) = 7
 
3. Inflation
Formula: Future amount = Present amount * (1+inflation rate) ^number of years
= 10,000* (1+5%) ^10 = 16,289
 
4. Purchasing Power
Formula: Future Value = Present value/(1+inflation rate)^number of years
   =10,000/ (1+5%) ^10 = 6,139
 
5. Effective Annual Rate 
Formula: Effective Annual Rate = (1+(r/n))^n)-1*100
If an investment is made at 9 per cent annual rate and compounding is done quarterly, the effective annual rate will be (1+(0.09/4)^4) -1*100  = 9.3 per cent
 
6. Rule of 72 
If you are assuming a 12 per cent return on your investment, the number of years in which the money will double is = 72/Interest rate= 72/12 = 6 years 
 
7. Compounded Annual Growth Rate (CAGR)
indicate the return on an investment over a period. It is also the best tool to compare returns of two different asset classes - for instance gold/equity or equity/real estate. 
Formula:  CAGR=((FV/PV)^(1/n)) - 1
Suppose that an investment of Rs 1,000 grows to Rs 5,000 in 10 years.
CAGR is ((5,000/1,000)^(1/10)) - 1 , This comes to 17.4 per cent, 
((20,000/10,000) ^(1/2)) - 1, the CAGR comes to 41.42 per cent.
 
8. Loan EMI 
Formula: EMI= (A*R)*(1+R) ^N/ ((1+R) ^N)-1)
Where A = Loan amount ,  R = Interest rate N= Duration
Suppose you have taken a loan of Rs 10 lakh at 11 per cent annual interest for 15 years. 1
1 per cent per annum translates into 11/1200 = 0.00916 per month
Tenure = 15*12 = 180 months
EMI = (1000000 x 0.00916) x
((1+.00916) ^180) / ([(1+.00916) ^180] - 1)  = = Rs 11,361 
 
9. Future Value of SIP 
Formula: S = R((1+i)^n-1/i) (1+i)
S = Future value of investment ,   R = Regular monthly investment  , i = Interest rate assumed /12
n = Duration (number of months or number of years *12) investing Rs 1,000 each month for the next 10 years and expect a return of 15 per cent. 
 
Monthly over next 10 years = 12*10 = 120 months
Interest: 15% per annum - 15/12 = 1.25% = 0.0125
S = 1,000 * [{(1+ 0.0125) ^120 - 1}/0.0125] *  (1+ 0.0125)  = The outcome is Rs 2,78,657, which is the future value of the SIP.
 
10. Liquidity Ratio
Formula:Liquidity Ratio = Total liquid assets\Total current debt
The value of this ratio should ideally be above one. 
 
Some points to note
1. NPV is an absolute number
2. IRR is expressed in % terms
3. NPV calculates additional wealth
4. IRR reflects investment performance as well as cash flows
5. Use of IRR facilitates comparison
6. NPV and IRR both are discounted cash flow models
7. Since NPV is a direct measure of increase in wealth, NPV is preferred over IRR in case of conflict in mutually exclusive investments (where we have to select only one investment). In case of a scenario like: A’s NPV is high & B’s IRR is high, always go with the higher NPV option.

Summary of formulae used
PV formula is PV= FV/ (1+r) ^n; In Excel =PV (rate, nper, pmt, fv, type)
PV of ordinary annuity (PVA) = PMT * 1-(1+i)^-n/i
In Excel = PMT (RATE, NPER, PV, FV, Type)
Payback period = Initial investment amount/value ÷ Cash flow per year
The formula of Compounding is FV = PV (1+r/100) ^n
HPR=(EV-BV/BV) *100
Inflation adjusted returns = [(1+ r) / (1+P)}-1]*100, where r is nominal
return and P is inflation rate
Tax Adjusted returns TR = NR * (1-tax rate), where TR: tax adjusted
return and NR: nominal return
IRR= NPV= FV/ (1+r) ^3
Total return = (EV - BV)/ BV *100
Sharpe Ratio (S) = (r (Portfolio return) – rf (Risk free rate)) / portfolio volatility (v)
Treynor Ratio (S) = (r (Portfolio return) – rf (Risk free rate)) / portfolio beta (b)
Jensen Ratio (S) = R (actual portfolio return) – SML (expected return)
SML= Rf+ ß (Rm- Rf), where Rf is risk free return, ß is portfolio beta , and Rm is market return.


