【良く使用される名前】

- 使用目的が明確なもの -
import.css
print.css
reset.css

- 使用目的が明確でないもの -

style.css
default.css
base.css
module.css
global.css

【良く使用されるCSSコメント記述例】

/* Body
----------------------------------------------------*/

/* Link
----------------------------------------------------*/

/*----------------------------------------------------
	Common
----------------------------------------------------*/



@charset "utf-8";

/*------------------------------------------

	@ Style Name	/css/commmon/base.css

--------------------------------------------

		00. Reset
		01. html, body
		02. Frame
		03. Navigation
		04. Module
		05. Clearfix

------------------------------------------*/

/*------------------------------------------
 *	00. Reset
------------------------------------------*/



/*
Font-size list (base: 12px)
 83% = 10px
 91% = 11px        175% = 21px        258% = 31px
100% = 12px        183% = 22px        266% = 32px
108% = 13px        191% = 23px        275% = 33px
116% = 14px        200% = 24px        283% = 34px
125% = 15px        208% = 25px        291% = 35px
133% = 16px        216% = 26px        300% = 36px
141% = 17px        225% = 27px        308% = 37px
150% = 18px        233% = 28px        316% = 38px
158% = 19px        241% = 29px        325% = 39px
166% = 20px        250% = 30px        333% = 40px
*/



/*//////////////////////////////////////////////////////////////////////////////

base.css

--------------------------------------------------------------------------------
Resetting HTML elements styles
	0. universal
	1. html, body, a
	2. inline elements
	3. block elements
	4. table elements
	5. html5 elements
	6. fonts(YUI)
	
//////////////////////////////////////////////////////////////////////////////*/

/* -----------------------------------------------------------------------------
	0. universal
----------------------------------------------------------------------------- */














@charset "utf-8";
/* ===================================================================
fonts
 10px = 77%     11px = 85%     12px = 93%     13px = 100%
 14px = 108%    15px = 116%    16px = 123.1%  17px = 131%
 18px = 138.5%  19px = 146.5%  20px = 153.9%  21px = 161.6%
 22px = 167%    23px = 174%    24px = 182%    25px = 189%
 26px = 197%
=================================================================== */


/* Body
----------------------------------------------------*/

body {
	background: url(../images/share/bg_paper_01.jpg) repeat;
	font-size: 13px;
	line-height: 1.7;
	letter-spacing: 0.3px;
}

/* Link
----------------------------------------------------*/
a {color: #c01622;}
a:link {color: #c01622;}
a:visited {color: #c01622;}
a:hover {color: #ff0012;}
a:active {color: #c01622;}

/* CSS3
----------------------------------------------------*/
#selectors {
/* 角丸 */
	-webkit-border-radius: 10px;
	-moz-border-radius: 10px;
	border-radius: 10px;

/* 角丸個別 */
	-webkit-border-top-right-radius: 15px;
	-moz-border-radius-topright: 15px;
	border-top-right-radius: 15px;

/* ボックスに影 */
	-webkit-box-shadow: 1px 1px 3px #999;
	-moz-box-shadow: 1px 1px 3px #999;
	box-shadow: 1px 1px 3px #999;

/* テキストに影 */
	text-shadow: 1px 1px 0px #999;
}

/* 汎用
----------------------------------------------------*/

.cf { width:100%; }
.cf:after {
  content: ""; 
  display: block; 
  clear: both;
}

.imgR {
	float: right;
	margin: 0 0 10px 10px;
}

.imgL {
	float: left;
	margin: 0 10px 10px 0;
}

.tC,
.btn {
	text-align: center;
}

.tR,
.sign {
	text-align: right;
}

.keyword {
	text-indent: 100%;
    white-space: nowrap;
    overflow: hidden;
}

.eng {
	font-family: 'Raleway', sans-serif;
	font-size: 108%;
}

.exBox {
	border: solid 1px #222;
	padding: 10px 20px;
}

.mB {
	margin-bottom: 20px;
}

.mT {
	margin-top: 20px;
}

.cts_body {
	padding: 20px 60px;
	width: 880px;
}













@charset "utf-8" !important;

/* ----------------------------------------
 * æ±Žç”¨ã‚¤ãƒ¡ãƒ¼ã‚¸ãƒ•ãƒ­ãƒ¼ãƒˆ
 * ---------------------------------------- */

.imgfl{
	float:left !important;
	margin: 0px 30px 30px 0px !important;
}
.imgfr{
	float:right !important;
	margin: 0px 0px 30px 30px !important;
}

/* ----------------------------------------
 *   æ±Žç”¨float
 * ---------------------------------------- */

.fl { float: left !important;}
.fr { float: right !important;}


/* ----------------------------------------
 *   æ±Žç”¨ã‚¯ãƒªã‚¢
 * ---------------------------------------- */
.cb { clear: both !important;}

/* ----------------------------------------
 *   æ±Žç”¨width
 * ---------------------------------------- */
.w50 { width: 50px !important;}
.w60 { width: 60px !important;}
.w70 { width: 70px !important;}
.w80 { width: 80px !important;}
.w90 { width: 90px !important;}
.w100 { width: 100px !important;}
.w110 { width: 110px !important;}
.w120 { width: 120px !important;}
.w130 { width: 130px !important;}
.w140 { width: 140px !important;}
.w150 { width: 150px !important;}
.w200 { width: 200px !important;}
.w250 { width: 250px !important;}
.w300 { width: 300px !important;}
.w400 { width: 400px !important;}
.w500 { width: 500px !important;}
.w600 { width: 600px !important;}

/* ----------------------------------------
 *   æ±Žç”¨line-height
 * ---------------------------------------- */

.lh10 { line-height: 1.0 !important;}
.lh11 { line-height: 1.1 !important;}
.lh12 { line-height: 1.2 !important;}
.lh13 { line-height: 1.3 !important;}
.lh14 { line-height: 1.4 !important;}
.lh15 { line-height: 1.5 !important;}
.lh16 { line-height: 1.6 !important;}
.lh17 { line-height: 1.7 !important;}
.lh18 { line-height: 1.8 !important;}
.lh19 { line-height: 1.9 !important;}
.lh20 { line-height: 2.0 !important;}

/* ----------------------------------------
 *   æ±Žç”¨line-height
 * ---------------------------------------- */

.lh10 { line-height: 1.0 !important;}
.lh11 { line-height: 1.1 !important;}
.lh12 { line-height: 1.2 !important;}
.lh13 { line-height: 1.3 !important;}
.lh14 { line-height: 1.4 !important;}
.lh15 { line-height: 1.5 !important;}
.lh16 { line-height: 1.6 !important;}
.lh17 { line-height: 1.7 !important;}
.lh18 { line-height: 1.8 !important;}
.lh19 { line-height: 1.9 !important;}
.lh20 { line-height: 2.0 !important;}

/* ----------------------------------------
 *   æ±Žç”¨margin
 * ---------------------------------------- */

.m0 {margin: 0px !important;}
.mt0 {margin-top: 0px !important;}
.ml0 {margin-left: 0px !important;}
.mr0 {margin-right: 0px !important;}
.mb0 {margin-bottom: 0px !important;}

.m5 {margin: 5px !important;}
.mt5 {margin-top: 5px !important;}
.ml5 {margin-left: 5px !important;}
.mr5 {margin-right: 5px !important;}
.mb5 {margin-bottom: 5px !important;}

.m10 {margin: 10px !important;}
.mt10 {margin-top: 10px !important;}
.ml10 {margin-left: 10px !important;}
.mr10 {margin-right: 10px !important;}
.mb10 {margin-bottom: 10px !important;}

.m15 {margin: 15px !important;}
.mt15 {margin-top: 15px !important;}
.ml15 {margin-left: 15px !important;}
.mr15 {margin-right: 15px !important;}
.mb15 {margin-bottom: 15px !important;}

.m20 {margin: 20px !important;}
.mt20 {margin-top: 20px !important;}
.ml20 {margin-left: 20px !important;}
.mr20 {margin-right: 20px !important;}
.mb20 {margin-bottom: 20px !important;}

.m25 {margin: 25px !important;}
.mt25 {margin-top: 25px !important;}
.ml25 {margin-left: 25px !important;}
.mr25 {margin-right: 25px !important;}
.mb25 {margin-bottom: 25px !important;}

.m30 {margin: 30px !important;}
.mt30 {margin-top: 30px !important;}
.ml30 {margin-left: 30px !important;}
.mr30 {margin-right: 30px !important;}
.mb30 {margin-bottom: 30px !important;}

.m35 {margin: 35px !important;}
.mt35 {margin-top: 35px !important;}
.ml35 {margin-left: 35px !important;}
.mr35 {margin-right: 35px !important;}
.mb35 {margin-bottom: 35px !important;}

.m40 {margin: 40px !important;}
.mt40 {margin-top: 40px !important;}
.ml40 {margin-left: 40px !important;}
.mr40 {margin-right: 40px !important;}
.mb40 {margin-bottom: 40px !important;}

.m45 {margin: 45px !important;}
.mt45 {margin-top: 45px !important;}
.ml45 {margin-left: 45px !important;}
.mr45 {margin-right: 45px !important;}
.mb45 {margin-bottom: 45px !important;}

.m50 {margin: 50px !important;}
.mt50 {margin-top: 50px !important;}
.ml50 {margin-left: 50px !important;}
.mr50 {margin-right: 50px !important;}
.mb50 {margin-bottom: 50px !important;}

/* ----------------------------------------
 *   æ±Žç”¨padding
 * ---------------------------------------- */

.p5 {padding: 5px !important;}
.pt5 {padding-top: 5px !important;}
.pl5 {padding-left: 5px !important;}
.pr5 {padding-right: 5px !important;}
.pb5 {padding-bottom: 5px !important;}

.p10 {padding: 10px !important;}
.pt10 {padding-top: 10px !important;}
.pl10 {padding-left: 10px !important;}
.pr10 {padding-right: 10px !important;}
.pb10 {padding-bottom: 10px !important;}

.p15 {padding: 15px !important;}
.pt15 {padding-top: 15px !important;}
.pl15 {padding-left: 15px !important;}
.pr15 {padding-right: 15px !important;}
.pb15 {padding-bottom: 15px !important;}

.p20 {padding: 20px !important;}
.pt20 {padding-top: 20px !important;}
.pl20 {padding-left: 20px !important;}
.pr20 {padding-right: 20px !important;}
.pb20 {padding-bottom: 20px !important;}

.p25 {padding: 25px !important;}
.pt25 {padding-top: 25px !important;}
.pl25 {padding-left: 25px !important;}
.pr25 {padding-right: 25px !important;}
.pb25 {padding-bottom: 25px !important;}

.p30 {padding: 30px !important;}
.pt30 {padding-top: 30px !important;}
.pl30 {padding-left: 30px !important;}
.pr30 {padding-right: 30px !important;}
.pb30 {padding-bottom: 30px !important;}

.p35 {padding: 35px !important;}
.pt35 {padding-top: 35px !important;}
.pl35 {padding-left: 35px !important;}
.pr35 {padding-right: 35px !important;}
.pb35 {padding-bottom: 35px !important;}

.p40 {padding: 40px !important;}
.pt40 {padding-top: 40px !important;}
.pl40 {padding-left: 40px !important;}
.pr40 {padding-right: 40px !important;}
.pb40 {padding-bottom: 40px !important;}

.p45 {padding: 45px !important;}
.pt45 {padding-top: 45px !important;}
.pl45 {padding-left: 45px !important;}
.pr45 {padding-right: 45px !important;}
.pb45 {padding-bottom: 45px !important;}

.p50 {padding: 50px !important;}
.pt50 {padding-top: 50px !important;}
.pl50 {padding-left: 50px !important;}
.pr50 {padding-right: 50px !important;}
.pb50 {padding-bottom: 50px !important;}
