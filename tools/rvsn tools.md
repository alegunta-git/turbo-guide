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



## ddg
* !a books  , !a iPhone 15 cases (Amazon USA) ,   !ain  ( Amazon india) , !acro rss
* !b hadoop Bing search , !bang (bangs),  !blogspot  Blogspot , !bbc bbc
* !books the ascent of money ( amz books )
* !e ebay , !etsy , !expedia ,  !fb facebook , !fk  Flipkart ,
* !g ostechnix , Google search , !gi flowers , Google Image , !gn  Google News 
* !gfaqs Ace Attorney , !goodreads Good Reads ,  !gh github
* !howtogeek windows 10 ,  !ig Instagram , !imdb imdb 
* !jobs software engineer  indeed 
* !kindle the ascent of money , !ka algebra  Khan Academy
* !li linkedin  ,  !makeuseof Windows 10 
* !mitocw algebra  MIT , !medium medium  ,  !nf  netflix 
* !ox grammar (oxford dictionary) , !p Pinterest  , !q quora
* !r news , Sub Reddit !sr ostechnix , !sr wallpapers , !slideshare  Slideshare , 
* !so stackoverflow ,  !sx tuple object is not callable ,  !sx java pointers  stackexchange 
* !t amazing thesaurus,  !ta trip advisor  , !tw Twitter  , !toi Times of india  ,!ted  , !twp , The washington Post 
* !u chipmunking , !udemy  , 
* !w linux  , !w pizza ,  Wikipedia Search ,  !wa solve 8x + 6 = 15x -8 Wolfram Alpha 
* !yelp , !yt dennis ritchie  , !yt cat videos ,  Youtube 
* best hero in mission impossible !g !w !imdb , !hno hackernoon , !techradar 
* google Map : !gmap Delhi , !m orlando  , Google Scholar !gsc  
* news ios 15 , password 8 , 5 para lorem  

## 101 blog titles
* beginners/Intermediate/Expert guide
* best advice / worst advice  , recommendations
* buyers guide / alternatives for / considerations before../ which is better mac or pc
* cheat sheet on / checklist for / top 10 
* 100 most popular cross-platform free software , List of Resources for
* 101 basics/courses ,Fundamentals  Know 
* do you need / should you invest in / history of / 
* hacks for / anatomy of  / practical guide / how i made
* how to right way / how to in wrong way / best way / How to __ in X Steps
* how to solve biggest problem in / habits of / ideas for / mistakes in 
* how to troubleshoot / reasons marketing campaign is not working 
* inspirational quotes , predictions about future of  ,  trends about , new in ...
* key benefits , pros and cons , questions to ask
* quick tips / fast facts / Hacks for 
* things we learned from (conf , seminars , workshops) , lessons learned , magic formula
* timeline on , statistics on 
* videos to watch / podcasts to listen / blogs to read

## G Search
**Dan IRE Tipsheet 2016**
* wikipedia , references , talk page , CATEGORY Wikipedia entries.
* images -> “electric motor” motorcycle diagram ,
* youtube videos 
* define term , ["childhood * obesity"] , cold * treatment 
* domain glossary , domain dictionary 
* domain diagram , domain infographic
* blogs , forums ,conference ,social nw , fb ,tw , association 
* QA sites Stack Exchange , reddit site search 
* g books (toc) , best writers domain  ,  
* g scholar ,ms research , papers , gov reports 
* [filetype:pdf domain] , Search for syllabi [site:.edu “machine intelligence” ] 
* [domain tutorial/seminar/training/lesson/lecture]
* g shopping . amz shopping

**keywords**
* Keyword + "top 10 resources"/"top resources" , "top 10 sites" , "top 10 articles" , 
* Keyword + "top 10 tools" "favorite resources" "recommended sites" 
* Keyword + "whitepapers" "videos"  "podcasts"  "research" 
* "list of + Keyword + sites" ,  Keyword + site:.edu , Keyword + site:.info 
* Keyword + "intitle:resources" "news"/"industry news" 
* Keyword + filetype:doc/docx/xls/ppt/pdf 
* Keyword + inurl:links/resources 
* **windows cheatsheet** ,video easy recipes , life quotes

## SDLC 
**BSA**
* wireframe tutorial , java ui , customer registration form 
* requirement  risks  , agile types of projects ,  jad / alpha testing / ab testing 
* meta data/web service example , mainframe systems screen
* payroll processing features , Payroll processing systems (vb/java/documentation) , Top 10 payroll processing systems 
* mobile banking , mobile banking products , oss
* healthcare regulations in us
* anti fraud system for banks ,  ,credit appraisal
* anti money laundering ,aml system requirements , aml functionality , aml transaction monitoring , aml comliance

**Dev SME**
* Java tutorial (not learn Java) , Try Java course , YouTube videos , courseera , 
* Cyber security jobs LinkedIn -> Check JD -> Search ethical hacking course udemy , check out syllabus 
* Intitle: cross site scripting , Indexof hacking books , Computer networking pdf , Cross site scripting pdf owasp 
* Python decorators site: stackoverflow.com
* Oauth , jwt,json attack [site:hackingarticles.in](http://site:hackingarticles.in/) , medium.com
* frontend conferences location:DE

**Site**
* site:Stackoverflow.com errors in stencil.js , site:fireship.io react hooks , 
* related:github.com , site:livecodestream.dev machine learning

**Src code** 	
* linux command line history examples - Google Search , bash examples OR programs - Google Search
* filetype:ppt algorithms 
* hello world program filetype:py
* filetype:py regression site:github.com
* vuejs cheat sheet filetype:pdf

**Tutorials**	
* **javascript course for beginners udemy**
* react hooks after 2020 , most starred github project after:2018 before:2019
* vim editor * and replace examples ( “vim editor find|search )
* Angular or React , data binding syntax -angularjs
* "css center a div" , how to do * in python  , #100daysofcode
* "ember.js tutorials" ,  Define inheritance in oops
* frontend conferences location:DE
* "guide to install php5 from source" - Google Search (~tutorial searches for keywords: guide, manual, reference)
* nagios ~tutorial  (or)  debian installation ~tutorial  
* “How to install drivers in Ubuntu?” instead of “Troubleshoot driver problems Ubuntu.”
* intitle:learn regular expression regex 
* inurl:unspalsh.com "keyboard" , allurl:javascript patterns

**JS and Hashtags**
* #jobs    #recruitment   #hiring   #careers  #itpm
* site:linkedin.com "founder we're hiring"
* site:docs.google.com/spreadsheets intitle:startups
* top companies to work for in 2022  

**Xray search queries**
* "software engineer"  (location) (intitle:"resume for" OR intitle:"resume of")
* resume tips intext:summary , abc jobs site:glassdoor.com
* developer profile summary examples linkedin 

**Interview Questions**
* site:glassdoor.com Java Developer interview questions 
* oracle sql queries OR Examples for interviews

## Google Search
**Google**
* Google Tab search : ferrets | ferrets pictures | ferrests videos | ferrets news
* single result - title , url , snippet , links into site
* sagittarria : web images videos news shopping 
* oranges - refer to related searches
* learn SERP page , suggestions as you type
* sagittaria , suggestions as you type
* resume - images , people ask , **click PDF at top**
* resume - web , images , related searches
* automatic import licenses ( people also ask) title URL link
* reviews "space.com" , **Lateral Browsing : Click command on links**
* Search for communities; find conference; read proceedings

**SERP pages**
* Local Search Results , Images , News , Videos , Events , Podcasts , Recipes
* Web Results : Organic Results , Featured Snippets , Sitelinks  , Search by Photos , Voice
* Related Searches , People Also Ask ,  , People Also Search For , Knowledge Graph ,Questions and Answers
* Ads : Google Ads (Paid) , G Shopping  , Apps 
* Travel: Guided Tours , Travel guide , Popular Destinations , Flight Info, Hotels ,Holiday Packages  ,Route Planner , Map
* Knowledge Panel :  Container , Reviews , Streaming
* Other results : Movies , Twitter , Sport Results , Stocks & Exchange Rates , Jobs

**Define**
* define remittance / hdmi / pwned / gis
* high technology industries ,
* milk carton recycling pa

**Domain / Database**
* domain glossary ,"cold recovery" , cold glossary , cold database
* fish/education/wildflower/medicine database

**How to queries**
* outlook tips , outlook tricks 
* “I have a flat tire” -> “repair a flat tire.” , “My head hurts” > “headache relief.”

**Maths/Coversion**
* 978+456 ,   978-456 ,  978*456 ,  978/456  , 
* 50% of 100  , 2^10  ,  sqrt(1521)  , 11% of 256
* tip calculator , tip for $500 , mortgage calculator
* kg in pound , usd in inr , 5.8 feet in m ,2 USD in Euros
* convert 5:30 AM GMT to IST”   “convert 1m to cm” , 
* 32C in F , 45 celsius in Fahrenheit , 400 yards in miles
* 9AM in Mountain View , time in London

**General Knowledge**
* circumference of the earth , diameter of earth
* r_sun m_sun ln9 log 9 . m_earth ,r_jupiter ,gravitational constant
* speed of sound , gravitational constant location of india
* population of japan capital of Mongolia
* what is the longest riiver , how long is the ganges river in km ,
* how many countries are there
* how many cat breeds are there - carousel
* "average length" elephant
* Find Text web page Ctrl F

**Google Images**
* introduction to accounting book , machine intelligence diagram
* parts of web page , Anatomy of a Landing Page , cichlid evolution
* domain infographic ( gdpr intitle:infographic OR inurl:infographic)
* domain diagram ( planetary gear diagram , "electric motor" motorcycle diagram)
* bicycle parts ,bicycle diagram , sailing tutorial ,ship sails diagram
* Sales funnel png , customer relationship management ,  machine intelligence diagram 
* cat gifs , "wild animals" , Education icon 
* pizza  intitle:infographic inurl:infographic , gdpr intitle:infographic OR inurl:infographic 
* gi : blue wildflowers henry coe image collection/album
* tesla - face , tesla coil – images , Tesla , Type : Face , Photo , clip art
* football field - green color - images ( filter : blue color) ,

**Videos**
* cats - click tabs for videos images , options more menu
* how to make a pizza , how do i replace my bike chain
* how to repair flat tyre , how to paint a room
* Cichlid evolution - check images / yt videos

**Filetype**
* california condor filetype:pdf
* the lewis and clark expedition filetype:kml
* filetype:ppt high school geometry tutorial
* filetype:py regression
* filetype:py regression [site:github.com]
* filetype:pdf : search cheat sheet , tax forms , technology trend report 2018 ,  consulting case interview ,
* filetype:xls : checkbook , excel budget template , "super bowl winners" 
* marketing ebook filetype:pdf [site:neilpatel.com]
* list of birds filetype:dat OR filetype:csv site:.edu

**SITE SEARCH**  
* site:kinsta.com "google search operators"  
* site:gov tax forms | immigration statistics.
* site:org OR site:edu "single-payer healthcare" 
* site:quora.com  study tips  , site:org college admissions , site:nytimes.com college admissions 
* site:lifehacker.com keyboard shortcuts 
* site:stackoverflow.com polymorphism 
* site:makeuseof.com  productivity tips , python  , "laptop for students" 
* site:microsoft.com windows security , site:apple.com iphone 4 scratches
* bikes [site:.in] ,  einstein [site:.edu] , "fairy tales" [site:www.appuseries.com]
* marketing + site:meetup.com  , blogging + site:quora.com
* pizza site:tiktok.com OR site:vimeo.com OR Site:youtube.com

**Operators**
* “tesla coil” OR “jacobs ladder”
* Custom Search Engine	, Keyword : zss , URL with %S query : site:zapier.com/blog 
* related:amazon.com 
* business plan 2008..2011 , seo news 2021..2022 , business plan 000000..000000 
* ohio car buyer statistics 2019 ( NOT : statistics )
* “digital marketing news"   "search Marketing guides"  ,  "power user guide"  , "direct sales" training
* "winter jackers for women" , dance classes +jazz , science books +children
* digital marketing OR content marketing  , (baseball OR soccer) athletes
* intitle:self help books , intitle index of mp3
* allintitle: best thai food in chicago ,healthy snacks , science projects
* inurl:resources , ranking websites , startups , allinURL:seo competitor research

## Domain Search
**News**
* top stories <Place> , Latest news  , headlines today 
* shopping : hawaii , flights ,
* Google News : Time range , fugu laws , timerange , japan news , presidents 1800.1900 , creative  writing

**movies and tv shows**
* movies near me , star wars release date
* titanic casts | budget | characters | director
* Lyrics , songs by creed , “avatar songs” , 

**Health**
* “headache relief”  ,  list of essential oils for colds  ,  
* nutrition orange  , calories banana ,  cheeseburger vs spaghetti 

**recipes**
* naan recipes site:.in

**books**
* books by Tom clancy , favorite * book 
* new york times best sellers , Amazon Recommendations
* Book Reviews : Refer to Good reads , Browse Amazon reviews , 

**ideas**
* bathroom redesign ideas  , "circular knitting needles"
* photos professionally printed on canvas , “solar powered air conditioner,”  

**Shopping**
* google pixel 3 review , apple source :times of india , macbook pro store:amazon.com 
* laptop rs30000..40000 ,intitle:2022 laptops for students  
* lenovo g62 + review + site:wordpress.com (ratings , price , comparison)
* ifb customer service number , (best | worst) office suite

**Tutorial**
* quadratic equation tutorial , sailing tutorial
* Google talks OR lectures , model airplanes how-to
* bay area resource for teachers ,  howard university lectures.
* what is the area of a circle , solve rhombus
* “machine intelligence” overview filetype:ppt site:.stanford.edu
* “machine intelligence” overview filetype:ppt [site:.gov]

**youtube videos**
* Youtube : Filters(PL/Viewcount) , Playlists , Shorts 
* #youtubetipsandtricks 
* 1940s passenger trains ,paper tricks 
* movies trailers ,parks and recreation episodes 
* latest songs , “avatar songs” , songs by creed , 
* google hacks , this year ,short / python programming , short / math tricks , long  , 
* startup , channel | learn german , channel
* allintitle : "beautiful places" 

**Social media search**
* google search hacks reel , google search hacks instagram
* Pinterest : Infographics  , paris france , architecture , historical photos , art nouveau 
* Instagram :  site:instagram.com ,  #libraries  , #illuminatedmansuscript  #shorts + "instagram story ideas"
* Twitter  : Events, Threads , Top vs latest , Filters , Hashtags , Adv Search . Tech Support , Links , comments 
* shopify twitter , phone recall @twitter  ,  #throwbackthursday  #windows ,bananas@twitter  @jsavitt

**seo queries**
* Informational : how , what , who , where , why , guide , tutorial , resource , help , ideas , tips , learn , examples
* Navigational : brand names , name of proaduct , name of service 
* Investigation : best , top , pricing , review , attribute of product , comparison 
* txn/shopping : buy , coupon , order , [city] type of store , purchase , cheap , price 
* Financial : Spending, budget, balance sheets,  ratios, filing,
* Demography : Census,population, estimates, projections, survey
* Public Opinion : Sampling, survey, public opinion, polling
* Statistics : abc population  , abc unemployment rate ,  search / Visualize Public Data 
* statistics , numbers , data set ,  fast facts , time series analysis

**Trip planner**
* paris destination guide filetype:pdf , itineraries, weather reports
* Add "destination" or "vacation" (such as "Europe" or "Bangkok") ,  
* "best family vacations" , things to do in london ,  top things to do in london 
* airfare and hotel price  comparisons ,vacation package "usa"  discount or deal -cruise
* new york map  ,  newyork  population , newyork weather , newyork sunrise
* chicago attractions  , Chicago events , Chicago hotels ,
* distance from Seattle to Taipei (distance , trains , flights)
* restaurants near me  , food joints <pin code> , italian restaurant near abc 
* hello in abc lang , festivals <year>




## G Suite
**Chrome**
* Address Bar : Use Icons on Menu Bar for copy paste
* Manage Search Engine(Custom Search Engine) to launch web apps ( yt , gc ,gn), Edit Search Engines
* Back , Forward, Reload , Save as, Print , Cast , Translate to English , View Page source (Ctrl U) , Inspect
* Undo , Cut , Copy, Copy URL ,  Paste , Paste and Go , Delete , Select All
* Open link (New tab , new win , incog win) , Send link to devices , Save link as , Copy link address , Inspect (CSI)
* Open image in new tab , Save image as , Copy img , Copy img address , Create QR Code , search img w/ G Lens
* Tabs : New Tab , New Window , Incognito Window  |  Pin , Mute Site , Close , Close tabs to right
* Right Click Tab ( New Tab to the right , Add tab to reading list , new group , Move tab to new window )
* Duplicate ( Alt+D Alt+Enter  in quick succession )
* Right click : Copy link to highlight , Search Google for , print , inspect
* Open All (NW,IW) , Rename , Add Page , Add Folder ,Bookmark Manager , Show Apps , Show Bookmarks bar
* Find , Zoom :Make Text Smaller , larger , Full Screen
* History , Downloads , Cast  : Looking for devices
* Bookmarks ( Bookmark Current Tab , All Tabs , Show Bookmarks bar )
* Bookmark Manager( Import Bookmarks and Settings , Mobile bookmarks)
* More Tools / Print /Print custom Pages( HL imp points , print custom range , jpg to pdf , merge pdf )
* Settings : Autofill , Privacy & Security , Appearance ,SearchEngine , Default Browser , OnStartup, Lang, Downloads
* Settings : Accessibility , System , Reset and Clean-up , WebStore , Extensions
* Guest profile , password Manager , Dev tools
  
**G News**
* save Stories , how news works , personalize news , 
* change settings , notifications
* local news , news widget , digital subscriptions np/content,

**G Finance**
* create portfolio , custom watch list , rename/delete , playground p/f
* 2 step verification , currency , add shares/mf to p/f , add index , remove investment
* see p/f balance , browse news p/f , view returns , highlights , compare p/f to assets

**G Keep (notes)**
* c compose note , i compose list
* Chrome extn ,settings , create and edit note , make list , take img notes , save a drawing
* organize notes : label , color , pin notes , archive notes , version history , set up reminders
* search notes , share notes , lists drawings , send keep note to another app , export data

**G Calendar**
* New calendar , View day/week/month , 
* Print cal ,Search cal , keyboard sc , gc offline
* Share cal , subscribe , transfer events , see availability , 
* switch accounts , color labels track entries
* create events gc/gm , respond event invitations , manage invitations , del event
* add attachments , rooms , video conf , 
* create appointment schedule , email verification appt
* gcal appointment slots , event privacy settings , 
* cal settings , gcal notification , working hours
* gcl in diff time zone , lang setting , screen reader , how spend time mtg
* sync apple cal , import events to gcal , gprd side/side , repeating tasks

**G Drive(Storage)**
* Ctrl + C, Ctrl + Shift + V move files
* open files or folders in a new tab using Ctrl+Enter, 
* so that you can easily view multiple files at once
* o  open file | n rename , c  create menu | shift + p presentation | shift + f   new folder
* GD files offline , buy more storage , manage files , find/recover file , 
* accessibility , dark theme
* drive toolbar buttons , drive desktop , upload files and folders , download file , view and open files
* store and play video , save web content , convert pdf and photos to text , fill pdf forms
* find file , org files , delete and restore files , notifications , shortcut , move files , labels to files
* share files , limit sharing , transfer ownership , share docs visitors , add photos gd to g photos , duet ai , workspace labs

**GMail**
* s star msg , # del select mesg , c compose msg , l label msg, g + i    inbox  ,   g + s   starred
* sign in , security , privacy , username , read em , org em , find em , fwd em
* contact info , chat msg , export data , gm settings , signature , profile pic
* vacation reply , offline , labels to org em , layout , accessibility , events
* write em , attachments , img , send bulk em, smart compose , read receipt , branded em
* pin conversation , mark msg read , mute notification , spaces , duet ai

**G Docs**
* File : New , open , make a copy , share , email , download , rename , move to trash , version , offline , details , page setup , print
* Edit : Undo , redo , cut , copy , paste , paste w/o format , select all , delete , find and replace
* View : mode , show print layout , ruler , outline , eq toolbar , non print chars
* Insert : image , table , drawing , chart , hline , emoji , smart chips , dropdown , footnote , building blocks 
* dropdown , footnote , watermark , headers and footers , page no's , break , link , comment , bookmark , toc
* Format : text , para styles , align and indent , spacing , cols , bullets and numbering , headers and footers 
* page nos , page orientation ,clear formatting , borders and lines
* Tools : spelling , word count , review edits , cmp docs , citations , line no , explore , linked obj 
* dictionary , translate doc , voice typing, notification , preference, accessibility
* Extensions : Add on , app script
* Help : search menus , help , training , updates , privacy policy , terms of svc , kb sc

**G Photos**
* Search by people , places , HDR , default gallery , featured memories
* Print Store : Photo books , Photo/Canvas prints , pmt info , transfer photos (gd)
* Share photos & videos , Stop sharing an album , Show photos TV(Chromecast) , Label face group
* edit photos and videos , discover creations , collages , backup photos (Storage)
* edit photo albums , suggestion cards , archive , info surroundings , download photos

**G maps**
* Saved , nearby , visited , lists , search (map) ,navigation , filter search results (price , hours , info)
* Find & book online services (online classes/estimates/appointments/yoga classes) ,
* hide personal content , see nearby events , Create a list of places , offline maps
* Search on Google Maps built into your car (voice), street view , edit place , review , photo , dish
* scale bar , measure distance , use layers to find places , traffic , terrain , biking
* indoor maps , air quality , recommendations , show routes , req ride
* shortcut to freq visited places , train and bus departures

**Youtube menu**
- YT ads - Use brave browser
- Explore menu (Gaming, News, Music, Movies, Fashion & Beauty, Learning, Sports, Podcasts, and Shopping)
- trending , adv search (filters) , official cards , search glass , mic , explore yt ,
- Watch Videos ( find videos , change settings , diff devices )
- comment/subscribe , save/share playlist , purchase movies/tv shows) ,
- hashtags , watch later , captions ,slider
- playlists (long/short create , add/remove videos , save , edit , explore you tab) ,
- play/pause , next , prev , mute/unmute , vol slider , cc ,annotations ,
- playback speed , quality , theater mode , full screen
- dark theme , pic in pic , mini player , pinch to zoom , control video volume
- chapter/grabber , location setting , siri
- Accounts settings , supervised experience , yt premium ,
- billing , policies , ads monetization , loop videos
- Channel ( upload/edit videos , shorts , yt create , manage channel
- analytics , subtitles , captions , live stream

**YT Topics**
* Beauty ,  Fashion & Style Tips  ,  Financial independence
* Fitness Tips ,  H2 create Videos ,  Kitchen Hacks  ,  Life Hacks 
* Music instrument   Makeup ,  Pets&animals 
* Seminars ,  Sports  ,  Stocks  ,   Top X Lists ,  Travel Vlogging
* Dramedy , Food & Restaurant  , Game Shows  , Gardening 
* Health , Helpful Software & Apps  , Hindi cinema  Indian soap operas 
* Lifestyle Adv  , Motivational & Inspirational Videos  , Music 
* Mutual funds ,  Pakistani dramas , Recently uploaded  , Review 
* Sitcomes , Tech & Gadget  , Trailer and Movie Reactions 
* Trending , Web series   , World or Local News 

**Youtube Niche Ideas**
* City Tours  , Cooking Videos  , Comedy , DIY Crafts  , Dance tutorials
* Digital Marketing & Blogging  , Educational channel  , Fashion & Style Tips 
* Gaming Videos , Gardening Tips & Tricks , Haircare & Hairstyle Ideas 
* Kitchen Hacks  , Music instrument tutorials   , Pets & animals 
* Tech & Gadget Reviews  ,  Top X Lists  ,  Trailer and Movie Reactions 
* Yoga , Car & bike News/Reviews Book Review  , Drawing & sketching tutorials 
* Food & Restaurant Reviews , Helpful Software & Apps  , How to Create Videos 
* Life Hacks , Makeup & Beauty Health & Fitness Tips  , 
* Motivational & Inspirational Videos . Lifestyle Advice
* Sports  , Travel Vlogging  , Unboxing   ,  Viral Challenges  , World or Local News 

**Webseries**
* Action ,  Adventure  ,  Animated  ,  Anthology  ,   Asian 
* Childrens / Tweens ,   Crime , Horror fiction , Sci Fi 
* Documentary ,  Drama ,  Dystopian  ,  Experimental Fantasy 
* LGBT ,  Legal  ,  Literary  ,  Martial arts 
* Prison ,  Romance  ,,  Science  ,  Superhero 
* Thriller  ,  nonfiction  , Comedy  ,  Crime Drama  , Dark Fantasy
