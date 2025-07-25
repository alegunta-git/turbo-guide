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


## Web design
**web Patterns**
* **GETTING INPUT**
* Flagging / Reporting , Tagging , Inline (Conversational) Forms , Input Hints , Natural Language Inputs
* Forgiving Formats , Inline Validation , Wizards / Stepped Forms , Completeness Meters , Action Context
* Keyboard Shortcuts , Drag-and-Drop Actions , Default Values & Autocomplete , 
* Immediate Immersion (or “Lazy Signups”) , Social Login , Notifications , 
* Discoverable Controls, Expandable Inputs , Undo
* **NAVIGATION**
* Jump to Section , Single-Page Web Apps , Recommendations , Related Content , 
* Next Steps , History / Recently Viewed , Featured Content , 
* Infinite Scroll , Walkthroughs & Coach Marks
* Overflow Menus , Morphing Controls , “Sticky” Fixed Navigation , Vertical Navigation ,
* Popovers , Slideouts, Sidebars & Drawers , Links to Everything
* **DATA & CONTENT MANAGEMENT**
* Favorites & Bookmarks , Stats / Dashboards , Contextually-Aware Content , Hover Controls
* Context Menus , WYSIWYG , Autosave , Lightbox Photo Slideshows , Full-Screen Modes
* Interactive Content Layers , Maps As Backgrounds , Group Friends & Content , Grids , Cards
* Hidden Information , Empty States , Direct Manipulation of Content & Data , Draggable Objects
* **SOCIAL**
* Achievements & Badges , Auto-Sharing , Activity Feeds , Friend Lists , Follow
* Vote to Promote , Pay To Promote , Direct Messaging , Like , Find & Invite Friends

**Web Design**
* IA blue print site ,  top level navigation ( tabs , menu bar , links , buttons ) 
* sketches / mock ups focus on functionality 
* text scannable( intro , header - section , bold and italics , short paras easier to read than text , bullet points to give facts ) 
* visual metaphor for page elements ( main navigation , sub navigation , sidebar ,  white space , content , footer )
* user persona , story boards , keep your site organized with IA ( Card sorting )
* grid , golden ration , 2/3 , 1/3 (1.66 ratio )
* color wheel , base color , typography , fonts , css style sheets for media 
* web copy , text present in inverted pyramid ( main heading , sub heading , provide gist , add detail afterward , user can skip low level details)
* web accessibility ( screen reader , audio. , alt text ) 

**Web Design Deliverables**
* Detailed description of site content
* Wireframes and prototypes demonstrating site architecture
* validated through user research and usability testing
* Taxonomies representing categories and tags
* Text, edited and proofread
* Graphic design specifications for all page types
* Header and footer graphics, logos, buttons, backgrounds
* Detailed page comps or finished examples of key pages
* Site graphic standards ,  master page grid templates completed 
* Finished html template pages , SEO
* cms templates , content structures , JavaScript scripts , Database tables 


**HTML**
* Web2.0 : Search , Links , Author , Tags , Signals
* Links:,href , name , target
* Text : Formatting , Section , List(ol,ul,dt) , Block(div,hr,p) , inline(span,a,img)
* Img:src,url,alt,align,ht,wt
* Tables:border,cell padg ,tr,td,th,colspan | Frames | Style(bgcolor,text color,fonts,size,txt algin)
* Forms(Form,action,method,input,name,value,size,text area, select , options)

**Developing User Interfaces for Microsoft Windows-Microsoft Press (1999)**
- The Windows Interface Guidelines for Software Design
- Microsoft Manual of Style for Technical Publications
- About Face: The Essentials of User Interface Design
- Donald A. Norman's The Design of Everyday Things
- Macintosh Human Interface Guidelines
- Easy to learn , configurability , beginning vs advanced users ,Information at Your Fingertips.
- Users Perform Tasks, Not Features


## UX
UI Patterns
| Type            | UI elements                                                                          |
|-----------------|--------------------------------------------------------------------------------------|
| Navigational    | Address bar , bread crumb , hyperlink ,  Navigation bar , Pager , Tree view          |
| Container       | Accordion , Disclosure widget , Frame , Field , Menu Bar ,                           |
|                 | Panel , Popover , Ribbon , Tab , Toolbar , Window , Work space                       |
| Command Input   | Button , Hamburger button , Context menu ,  Drop Down list , Menu                    |
| Data i/p o/p    | Checkbox , Color Picker , Combo box , Date picker ,  Grid view ,                     |
|                 | List box , List builder Radio , Scroll bar , Search box , Slider , Spinner , Textbox |
| Informational   | Icon , Info bar , Label , Loading screen ,  Progress Indicator ,                     |
|                 |  Progress bar Splash screen , Throbber , Sidebar , Status Bar , Toast , Tool tip     |
| Special Windows | Alert Dialog box , Dialog box , File dialog , Inspector window ,                     |
|                 | Modal Window , Palette window                                                        |
| Others          | File viewer , Layout manager ,  Look and feel , Mouse over , WIMP                    |


eCommerce Site UI Controls
* About page , Accepted payment methods , 
* Added to basket , Alternatives to buying
* Badges , Basic form usability
* Basket – products , Basket – shipping cost , Buy button
* Carousels, Category descriptions
* Checkout (1a. Basket , 1b. Product customization) -> 2 Delivery information -> 3 Billing information -> 4 Payment details
* Checkout navigation , Contact methods , Content pages , Country & currency
* Credibility messages , Cross-selling
* Delivery information , Details
* Do you need a product finder? , Do your users understand your product names?
* Editorial content , Extra content
* Filters – mobile , Filters – desktop
* Guest checkout , Images , Landing , Layout , Listings
* Mailing list sign-up , Main heading , Main image
* Maps , Mobile form usability , Names
* Order collection , Order confirmation , Order summary
* Payment gateways , Price , Primary actions
* Product , Product video , Promo code field , Promotions
* Quick view , Ratings , Related products , Repeated links
* Reviews , Search fields , Should you use ‘add to basket’ links?
* Site navigation , Smart defaults , Social buttons , Social media feeds , Social proof
* Stock levels , Thumbnail images , Title field , USP , Variant options
* Variations , Video , Wallets

