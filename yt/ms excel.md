## MS Excel
**xls topics**
| Category | Examples                                                                                  |
|----------|-------------------------------------------------------------------------------------------|
| Maths    | Mod , Abs , Int , Subtotal , Sum , Sumproduct , Randbetween , Round , Roundup , Rounddown |
| Logical  | IF  , AND , OR , NOT , True , False , Cell , IsError , IsBlank , IsText , IsNumber        |
| Text     | Len , Text , Value , Find , Replace , Trim , Left , Mid , Right                           |
| Dates    | Today , Weekday , Workday ,  Datevalue , Eomonth , Edate , Days360 , year    ,  Month     |
| Lookup   | Lookup , HLookup , Vlookup , Choose , Match , Index , Offset , Indirect                   |
| Finance  | PV  FV RATE NPER  , NPV XNPV  IRR XIRR MIRR                                               |
| Finance  | PMT PPMT IPMT ISPMT CUMIPMT CUMPRINC                                             |
| Finance  | DB DDB VDB SLN SYD NOMINAL EFFECT FVSCHEDULE                                             |

Investment
* PMT , PPMT , PV, FV , RATE , NPER , NPV , XNPV, XIRR
* PMT   (10% , 3 , 1000)   -402.11
* PMT   (5%/12 , 60 , 50000)
* PPMT  ( 10% , 1 , 3 , 1000) -302.11 ppmt(10%,2,3,1000) -332
* pv ( 10% , 3 , 1 , -100) 3 nper , 1 ppmt , fv -100
* pv ( 5%/12 , 60 , 1000 ) 5 yrs
* npv( 5% , b4:b7 (values)) + b3 (rate)
* npv ( a1-2% , a2:a7) -5000 , 800 , 950 , 1080 1220 1550
* xnpv ( 5% , c4:c8 , d4:d8)  dates , values
* nper ( 10% , -200 , 1000) Is this for annual rate ???
* nper ( 4%/12 , -1000 , 50000)   monthly rate , pmt , loan
* nper ( 6%/4 , -12000 , 9000 , 5000 , 1)
* rate ( 6 , -200 , 1000 , 0.1) 6 - nper , 200 pmt , 1000 loan , 0.1 guess
* rate ( 60 , -1000 , 50000)   5 yrs * 60 , 1000 pmt , 50000 loan  * 12 * a2
* rate ( 24 , -800 , 0 , 20000 , 1)
* xirr( c4:c8 , d4:d8 , 0.1 )  c4c8 - investment , d4d8 - dates , -10000 , 200 , 400 , 01 Jan to Apr

Interest
* FV, IPMT,ISPMT, IRR , MIRR, NOMINAL,EFFECT , CUMIPMT,CUMPRINC ,FVSCHEDULE	
* fv ( 10% , 3 , 1 , -100 ) 3 nper , 1 pmt
* fv ( 5% / 12 , 60 , -10000)
* fv ( 10% / 4 , 16 , -2000 , 0 , 1 )
* IPMT  (5%/12 , 1, 60, 50000) , IPMT(5%/12 , 2, 60 , 50000)
* ISPMT ( 7.5%/12 , 8 TH MONTH , 2*12 2 YRS, 5000) * -20.833
* irr ( c3:c7 , 0.1) , -1000 , 3000 400 400 300
* mirr ( c3:c7 , 12% , 10% ) finrate reinvstmnt rate
* nominal(12%,12)
* effect(12%,12)
* effect(10%,4)
* CUMIPMT ( 5%/12 , 60 , 50000 , 1 , 12 , 0 ) * CUMIPMT ( 5%/12 , 60 , 50000 , 13,24 ,0)
* CUMPRINC ( 5%/12 , 60 , 50000 , 1 ,12 , 0)  13.24 , 25 TO 36
* fvschedule ( c1 , c2:c4)  100 principal , rate percent

Depreciation
* DB , DDB, SLN , SYD
* sln ( 10000 , 1000 , 5)
* syd ( 10000 , 1000 , 5 , 1 )
* ddb ( 10000 , 1000 , 5 ,1 )
* db ( 10000 , 5000 , 5,1 ,12)
* vdb ( 10000 , 5000 , 5*12 , 6,12 , 2 , true)

Logical
* AND , OR , IF, NOT , TRUE , FALSE
* and ( a1 > 0 , a1 < b1 )  , or ( a1 > 0 , a1 < b1) 
* if ( b1 = 0 , "div zero" , a1/b1) ,  if ( a1> = 0 , a1 , -a1) , if (iserror(1/a3) , 1 , 1/a3) ,  if ( len(a1)<>0 , 1,0 )
* not ( isblank (b1)) ,  True() ,  False()

Math
* ABS , EXP , FACT , GCD , LCM	 , MOD	 , POWER ,  PRODUCT , QUOTIENT ,SIGN , SQRT , SUM
* abs(-10) , exp(3) ,  gcd ( 1,5) ( 15,25)  ,  lcm(1,8,12) ,  mod ( 6, 4) ,  power ( 2 , 5) 
* product(3,6,2,8,5) , quotient(5,2)  , sign(9.5) ,  sqrt(25) ,  sum(a1:a5)(5,6,7,8)   ( b16,b18)
* fact(12) , factdouble(5)

Rounding 
* CEILING ,  COMBIN , EVEN , FLOOR , INT , MROUND , ODD , ROUND , ROUNDDOWN , ROUNDUP , TRUNC
* arabic("iv") , base (12,2) , combin(6,1) , decimal("100",2) , 
* even(23) , odd(22) , int ( 1009) , ceiling ( a2, 0.1)  , trunc(a1,2)
* mround(a2 , 0.5) , round(a1,1) -1 , -5  , rounddown(a1,1) , roundup( a2 , 2)

Operators
*  LN , LOG , LOG10 , PI ,ROMAN ,RAND , RANDBETWEEN , MDETERM ,MINVERSE ,MMULT ,MULTINOMIAL
* ln(100) , log10(100) , log(64,2)  ,  rand() * 100 ,  randbetween(10,20)

Text 
* CLEAN , CODE , CONCATENATE , EXACT , FIND ,LEFT,LEN,LOWER,MID, PROPER , REPLACE , REPT , RIGHT, SEARCH ,  SUBSTITUTE , T , TEXT , TRIM ,UPPER , VALUE
* char(65) , code(a1) 65  , code("2") , exact(a1,b1) ,  len (a1)  , clean( a2) ,  lower(a1) , upper(a1) , proper(a1) , 
* find("T", a1) , find("t", a2)  ,  find("i", a4 , 4)
* search("T", a1) ,  search("t", a2) ,  , search("i", a3) , search("i", a4,4)
* left ( a1 ) , left (a2,4) , left( a3 , find (" ") , a3-1) | mid(a1,7,1) ,  mid(a2,4,7) ,  mid(a3,3,1) |  right(a1) ,  right(a2,4) , right(a3, )
* concatenate(a2 , " " , b2) ,  replace(a1,7,3,"X") , substitute(a1,"a","X") ,  substitute(a4,"5","6") , substitute(a3,"John","Jane")
* trim( a3) , t(a1), rept("ha",9) 
* text ( a2, "dd/mmm/yyyy') ,  text ( a4, "mm dd yyy") ,  text ( a5, "hh:mm") ,  text ( a6, "0.00") ,  text ( a7, "0.0%") , text ( a9, "$#,####0")
* value("50") , numbervalue("1000") ,  numbervalue("5%")

Count
* AVERAGE , AVERAGEA COUNT COUNTA	COUNTBLANK COUNTIF COUNTIFS PERMUT QUARTILE  MAX MIN MODE PERCENTILE PERCENTRANK RANK LARGE	SMALL		
* average (a1:a5) ( 8,7,6,9) ,  averageif(a1:a14,"Wed",b1:b4,5) ,  averageifs(d2:d13, a2:a13,1,b2:b13,"month")
* permut(6,6) ,  mode( a1:a10) , 
* count( a1:a5) ,  counta(a1:a6) ,  countblank(a1:b5) ,  countif(a1:a9, "Wed", "<>wch",1,">01/10",20) ,  countifs(b2:b13,"male", d2:d13 , ">60%")
* max ( a1: a5) , min( a1: a5) , percentile(a1:a6 , 0.2) , percentrank ( a1:a9 , 6.5 , 7.5) ,  quartile ( a1:a7 , 0)   2  ,  
* rank( 5 , a1:a7 , 1) ,  rank( 9 , a1:a7 ) ,  large ( a1:a5 , 3) ,  small ( a1:a5 , 2)

Time
* TIME,NOW , Timelvalue , HOUR,Minute,SECOND
* now() ,  today() ,  time( 5 , 44 , 3 )  ,  timevalue("2:23 am")
* hour("12:45:10") ,  minute("12:45:10") , second("12:45:10")

Date
* DATE , DATEDIF , DATEVALUE , DAY , DAYNAME , DAYS360 , EDATE , EOMONTH , MONTH , MONTHNAME 
* NETWORKDAYS , NETWORKDAYS.INTL , TODAY , WEEKDAY , WEEKNUM , WORKDAY,YEAR, YEARFRAC
* date ( 2001, 1 , 2) ,  datedif(d1,d2,"d") ,  datevalue("01/01/2016")  ,  day(a2)   31-may-2020  ,  year(a2) ,  month(a2)
* edate(a1,1)  ( a2,-1) ,  eomonth(a1,9) , (a2,-12) , (a3,0) ,  days360(a1,a2) ,  networkdays(b1.b2 , b3:b5) with Hols ,  networkdays(b1.b2)
* today() ,  weekday(a2) ,  weeknum(a1) ,  workday(b1,25 ) ,  workday(b1,25 , b2:b4) with Hols ,  yearfrac(b1 , b2)

lookup , address
* Address,AREAS,CHOOSE,COLUMN,COLUMNS,HLOOKUP,HYPERLINK,INDEX,INDIRECT,LOOKUP,MATCH,OFFSET,ROW,ROWS,TRANSPOSE,VLOOKUP
* address(1,1) ,  address(1,1,3) ,  address (row() , col()) ,   areas(c1:e2) ,  areas((c1:e2 , b2:b5))
* transpose(a1:a6) ,  column(c6) ,  columns(b1:e5) ,  row() ,  rows()
* lookup ( f2 , a2:c7) ,  vlookup ( d2 , a:b , 2 , false ) - exact match ,  vlookup ( f2 , a2:c7 , 3 , true )  
* hlookup ( c6 ,  c1 : f3 , 3 , true ) ,  hlookup ( a10  , a2:f6 , 5 , false )
* choose ( a1 , "red" , "blue" , "green")  ,  index ( c1 : c5 , 5) ,  index ( c1 : d5 , 5 , 2 ) ,   sum ( index ( c1 : d5 , 5 , 0)) , offset ( a3,3,1)
* match ( 6 , a1:a6 , 1) ,  match ( "aaaa" , a1:a5 , 0) ,  match ( "?eee" , a1:a5 , 0) ,  match ( "*b" , a1:a5 , 0) , 

Information
* N,IFNA,ISNA,NA,SHEET,TYPE,CELL,INFO,ERROR.TYPE,IFERROR,ISERR,ISERROR,ISTEXT,ISNONTEXT,ISREF,ISBLANK,ISLOGICAL,ISEVEN,ISODD,ISFORMULA,ISNUMBER
* cell ("address" , a1) ,  cell ("col" , a1) ,  error.type(a1)
* isblank(a1) ,  iserror(559) , iserror("text") ,  iseven(0) (2) ,  isodd(0) (1)
* isformula(a1) ,  islogical(true) , islogical(false) , islogical(text) ,  isna(536) ("text") (#n/a)
* isnontext() ,  isnumber(1) , isnumber("text")  ,  isref(b)  ,  sheet() ,  type(2) , N(10) ,  NA()

Regression
* INTERCEPT , SLOPE , STEYX
* intercept( g2:g7 , f2:f7 ) known y , known x
* slope( g2:g7 , f2:f7 ) known y , known x
* steyx( g2:g7 , f2:f7 ) known y , known x

Trends
* FORECAST , GROWTH ,TREND , LINEST ,LOGEST
* forecast ( 7 , g2:g7 , f2:f7)  known x's , known y's    y * a + bx 
* {growth(b2:b5, a2:a5 , a8:a10)}
* {Trend(b2:b5 , a2 : a5 , a8 : a10)}
* linest(b2:b10 , a2:a10 , true , true) 
* logest(b2:b10 , a2:a10 , true , true) 

Transformation 
* CORREL ,  FISHER , FISHERINV ,  PEARSON , RSQ , STANDARDIZE

Variance
* VAR, VARP ,  VARA , VARPA
* var( b3:b100 , d3:d100 , f3:f100) ,  var.p( - do -)
* vara( a1:a4) , varp( a1:a4)

Deviation
* MEDIAN , GEOMEAN , HARMEAN, TRIMMEAN, CONFIDENCE , STDEV , STDEVA,STDEVP,STDEVPA , COVAR , DEVSQ
* confidence.norm ( 0.05 , 0.07 , 100) ,  covar ( a2:a9 , b2:b9) ,  devsq ( a1:a6 )
* geomean( a1:a5) ,  harmean( a1:a5) ,  median( a1:a7 , 12)
* stdev ( b2:b100 , d3:d100  , f3:f100) ,  stdev.p (-do- ) ,  stdeva (a1:a4) ,  trimmean(a1:a10, 15%)

Summation
* sumif(a2:a9 , "Feb" , c2:c9 , "North") ,  sumifs ( a2:d13 , a2:a13 , 1 , b2:b13 , " ")
* subtotal( 1, c2:c10)  ,  subtotal( 9, c2:c10) ,  sumproduct ( a2:a4 , b2:b4)
* sumsq(a2:a5) 5^2 + 2 ^ 2 + 1 ^ 2 + 3^2 
* sumx2my2(a2:a4,b2:b4) ,  sumx2py2(a2:a4,b2:b4) ,  seriessum(5,1,1,{1,1,11,})

Conversion
* convert(20.2, "mi","yd") , bind2dec("10") ,  erf(0,1.5) ,  acos(-1) ,  asin(-1)
* degrees(acos(1/sqrt(2)),  degrees(1) ,  radians(50) , pi()

Probability
* BETAINV,BETADIST,BINOMDIST,CHIDIST,CHIINV,CRITBINOM,EXPONDIST,FDIST,FINV,FREQUENCY,FTEST,GAMMADIST,GAMMAINV,GAMMALN,
* HYPGEOMDIST,LOGINV,LOGNORMDIST,NEGBINOMDIST,NORMDIST,NORMINV,NORMSDIST,NORMSINV,POISSON,PROB,SKEW,TDIST,TINV,TTEST,WEIBULL,ZTEST
* beta.inv( 0.2 , 4 , 5 , 0, 1 )  ,  betadist( 0.4 , 4 , 5 , true , 0 , 1 ) 
* binom.dist( 50 , 100 , 0.5 , false) ,  binom.inv ( 100 , 0.5 , 20% ) ,  binomdist( 10 , 100 , 0.5 , false)
* chidist ( 0.5 , 1 ) ,  chiinv( 2.5 , 1 ) ,  chitest(0.5 ,1 ) 
* correl( a2:a21 , b2:b21) ,   critbinom ( 100 , 0.5 , 20%) ,  
* expon.dist ( 0.5 , 1 , false) ,  f.dist ( 1, 2 , 5 , false) ,  f.test ( a2:a21 , b2:b21) ,  
* finv ( 0.9 , 2 ,5 )  ,  fisher ( 0.9) ,   fisherinv( -0.2)
* gamma ( 0.1) ,  gamma.dist ( 6 ,3 , 2 , false) ,   gamma.inv ( 0.5 ,3 , 2 ) ,  kurt ( a1:a5) ,  loginv ( 0.3 , 2 , 0.2) 
* negbinomdist ( 6 , 12 , 0.5 ) ,  negbinomdist(6,12,0.5,false) 
* norm.inv( 0.6 , 5 , 2) ,  norm.s.dist ( 0.5 , false) ,  norm.s.inv ( 0.25) ,  normdist ( 50 , 40 , 20 , false)
* poisson ( 20 , 25 , false) ,  prob ( a2:a9 , b2:b9 , 3.5) ,  rsq ( a2:a9 , b2:b9) ,  skew ( a1:a15) ,  standard ( 5.5 , 5 , 2)
* t.dist ( 1, 10 , 1) ,  t.dist ( 1, 10 , true) ,  t.dist.2t( 1,10) ,  t.dist.rt ( 1,10) 
* t.inv ( 0.25 , 10) ,  t.test ( a1:a12 , b1:b12 , 2, 1 ) ,  weibull( 1,3,1,false) 
* z.test ( a1:a12 , 5) , (frequency(a2:a11, b2:b9)}



## MS Excel
* xls : Arrange All Windows , Quick access toolbar pin it ,
* Excel : Formulas 100, xls macros , 101 tips/tricks , pivot ,charts , Tips , Data Analysis
* Excel : Finance Modelling, Statistics , Graphs ,Dashboard , Quality , Stats
* [copy text to xls](https://www.youtube.com/watch?v=7UVbaBuUWEA&list=PLmMyXRtEtJEaMk5au5y8p8avI5kJuQPHS&index=38&pp=gAQBiAQB)
* md to xls : https://www.youtube.com/watch?v=iIyNSbPElf4&list=WL&index=9&pp=gAQBiAQB
* fin literacy : https://www.youtube.com/watch?v=vJabNEwZIuc&list=WL&index=2&pp=gAQBiAQB
* data from web to xls : https://youtu.be/tmuvIt_ITLw?si=LSYityc4e74VMJFw



  
**Excel Formulas**
* [Google sheets fn list](https://support.google.com/docs/table/25273?hl=en-GB&ref_topic=1361471)
* [CAGR Ablebits](https://www.ablebits.com/office-addins-blog/calculate-cagr-excel-formulas/)
* [Excel Easy: #1 Excel tutorial on the net](https://www.excel-easy.com/)
* [xls easy fn](https://www.excel-easy.com/functions.html)
* [tax guru xls fx](https://taxguru.in/finance/excel-formulas-shortcuts-bank-reconciliation-emi-calculation-pivot-tables.html)
* [xls fn](https://www.excelfunctions.net/excel-functions-list.html)
* [xls function](https://excelx.com/formulas-functions/)
* [Excel Formula List - Which formulas you must learn - 100+ examples](https://chandoo.org/wp/excel-formula-list/)
* [xlsJet 350](https://exceljet.net/functions)
* [500 Excel Formula Examples | Exceljet](https://exceljet.net/formulas)
* [xls Stats fn](https://real-statistics.com/excel-capabilities/built-in-statistical-functions/)
* [xls Stats fn2](https://bettersolutions.com/excel/functions/statistical-category.htm) 

tips
* [yt Top 30 tips](https://www.youtube.com/watch?v=Hj4PVFYhqhQ&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=2)
* [xls tips](https://www.teachexcel.com/excel-tutorial/#9)
* [xls tips300](https://excelchamps.com/guides/tips/)
* [Top 100 Excel Tips and TRICKS (Basic + Advanced) (Free PDF)](https://excelchamps.com/blog/tips/)

vba
* [yt xls vba loops](https://www.youtube.com/watch?v=QOxhRSCfHaw&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=3)
* [18 ready-to-use VBA Codes that will save your day](https://yonkov.github.io/post/18-ready-to-use-vba-codes-that-will-save-your-day/)

I banking
* [yt xls Investment Banking](https://www.youtube.com/watch?v=VpY-v9Gn6YA&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=23)
* [bks FinModeling](https://corporatefinanceinstitute.com/resources/financial-modeling/best-financial-modeling-books/)

**Data Analysis**
* [Custom Excel number format](https://www.ablebits.com/office-addins-blog/custom-excel-number-format/)
* [Group Pivot Table](https://www.excel-easy.com/examples/group-pivot-table-items.html)
* [Create Two-Variable Data Table in Excel (Step by Step Examples)](https://www.wallstreetmojo.com/two-variable-data-table-in-excel/)
* [3 ways duplicate](https://spreadsheetplanet.com/duplicate-sheet-in-excel/)
* [download data](https://www.spreadsheetsports.com/free-tools/how-to-download-sport-data-into-a-spreadsheet/)


**yt xls tips**
* [yt xls](https://www.youtube.com/watch?v=9iQj0Lix7UM)
* [yt Percentage increase and decrease](https://www.youtube.com/watch?edufilter=NULL&v=HlX3O9vDzlc)
* [yt Percent GST](https://www.youtube.com/watch?v=eYlrebch0oU&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=36)
* [yt Financial Functions - YouTube](https://www.youtube.com/watch?edufilter=NULL&v=-6ERqkxlcFY)
* [yt How To Calculate CAGR, IRR & XIRR on Excel Spreadsheet? - YouTube](https://www.youtube.com/watch?edufilter=NULL&v=JD0ootg9JOE)
* [yt Excel add ins : How to Make your own Excel Add-ins - YouTube](https://www.youtube.com/watch?edufilter=NULL&v=t9MFnBpDHfA)
* [yt text to col](https://www.youtube.com/shorts/sKLEBqSZlTE)
* [yt Excel select data](https://www.youtube.com/watch?v=GBPLRthTsGc&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=15)
* [yt Excel Autofill](https://www.youtube.com/watch?v=zQOafMG3Iq4&list=PLmMyXRtEtJEY9N3G_nEAobi5b2nusbnPg&index=8)
* [yt Advanced Find & Replace](https://www.youtube.com/watch?v=ZDuM2oQAiLw&list=PLmMyXRtEtJEY9N3G_nEAobi5b2nusbnPg&index=9)
* [yt clean data](https://www.youtube.com/watch?v=x78JR7XHTro&list=PLmMyXRtEtJEY9N3G_nEAobi5b2nusbnPg&index=10)
* [yt Copy Text from Browser to Excel](https://www.youtube.com/watch?v=7UVbaBuUWEA&list=PLmMyXRtEtJEbe9jHvxCL08o6pHnKWJRQ3&index=9)
* [yt Excel Autofill](https://www.youtube.com/watch?v=zQOafMG3Iq4&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=2)
* [yt Advanced Find & Replace](https://www.youtube.com/watch?v=ZDuM2oQAiLw&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=11)
* [yt ⏱Do in 10sec Combine Multiple Workbook](https://www.youtube.com/watch?v=wIFXqd0m4VY&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=16)
* [yt Download Data from the Web](https://www.youtube.com/watch?v=RCcEUpRNsXg&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=21)
v

**Finance Modeling**
* [How to Build a Financial Model in Excel - Full Tutorial for Beginners - YouTube](https://www.youtube.com/watch?edufilter=NULL&v=-ivpFNCU4CY)
* [How to Build a Basic Financial Model in Excel - YouTube](https://www.youtube.com/watch?edufilter=NULL&v=Wws6T9uPVfA)
* [Financial Modeling Tut - Quantitative Portfolio Management ](https://www.youtube.com/playlist?list=PL6YwPExkSESoghM_-FoS0VVI7elc4dLVB)
* [Financial Modeling CMU](https://www.cmu.edu/swartz-center-for-entrepreneurship/assets/connects-spring-2018/Financial%20Modeling%20-%20CMU%20-%20Compton%202-2-18.pdf)
* [Financial Modelling Best Practices - YouTube](https://www.youtube.com/watch?v=lvVfN6uFrrM&list=PLmMyXRtEtJEY9N3G_nEAobi5b2nusbnPg&index=15)
* [Financial Modeling The Top 10 Skills](https://corporatefinanceinstitute.com/resources/knowledge/modeling/financial-modeling-skills/)
* [Top 5 Excel Features for Financial Modellers - YouTube](https://www.youtube.com/watch?v=HGlYRbxpVJU&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=12)
* [Core Financial Modeling Part 1 - YouTube](https://www.youtube.com/watch?v=BXP0i1TIvrg&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=13)
* [Advanced Financial Modeling In Excel - Essentials of Excel Skills in Building a Financial Model - YouTube](https://www.youtube.com/watch?v=IW8Jp4-8q-Y&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=22)
* [The great Excel-based project plan template explained - tacticalprojectmanager.com - YouTube](https://www.youtube.com/watch?v=gyySngGuWqQ&list=PLmMyXRtEtJEYEbVO5Freg35Xl6HzMm63z&index=32)
  

**Statistics**
* [wsj 2 Var Data ](https://www.wallstreetmojo.com/two-variable-data-table-in-excel/)
* [Scatter plot](https://www.excel-easy.com/examples/scatter-plot.html)
* [How To Make Normal Distribution Graph in Excel? (With Examples)](https://www.educba.com/normal-distribution-graph-in-excel/?source=leftnav)
* [Scatter Chart in Excel (Examples) | How To Create Scatter Chart in Excel?](https://www.educba.com/scatter-chart-in-excel/?source=leftnav)
* [Bell Curve in Excel | How To Make Bell Curve in Excel?](https://www.educba.com/bell-curve-in-excel/?source=leftnav)
* [Bubble Chart in Excel (Examples) | How to Create Bubble Chart?](https://www.educba.com/bubble-chart-in-excel/)
* [Control Charts in Excel | How to Create Control Charts in Excel?](https://www.educba.com/control-charts-in-excel/)
* [Understanding the normal distribution - statistics help - YouTube](https://www.youtube.com/watch?v=mtH1fmUVkfE&list=PLmMyXRtEtJEZ4Mt2eOzcARIIqjF4DrwEO&index=9)
* [Interpretation of control charts SPC 7QC Tool - YouTube](https://www.youtube.com/watch?v=jBO-W8cKqLw)
* [Create a Basic Control Chart - YouTube](https://www.youtube.com/watch?v=os17KYZAnd0)
* [Create Control Charts (X-Bar & R Chart) in Excel - YouTube](https://www.youtube.com/watch?v=krowVMzxecI)
* [Interpretation of control charts SPC 7QC Tool - YouTube](https://www.youtube.com/watch?v=jBO-W8cKqLw)
* [What is RStudio and Why Should You Download It? | R Tutorial 1.1 | MarinStatsLectures - YouTube](https://www.youtube.com/watch?v=riONFzJdXcs&list=PLmMyXRtEtJEZ4Mt2eOzcARIIqjF4DrwEO&index=7)
* [The Five Number Summary, Boxplots, and Outliers (1.6) - YouTube](https://www.youtube.com/watch?v=tpToLyZibKM&list=PLmMyXRtEtJEZ4Mt2eOzcARIIqjF4DrwEO&index=5)
* [Statistics 101: Population vs Sample Data - YouTube](https://www.youtube.com/watch?v=8X2xfwBP4uo&list=PLmMyXRtEtJEZ4Mt2eOzcARIIqjF4DrwEO&index=1)
