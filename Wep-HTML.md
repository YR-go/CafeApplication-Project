# Web

# ⚫ Web Page (HTML)
#　<header>에 Firebase 와 연동 scirpt 삽입
<code>
<!DOCTYPE HTML>
<html>
  <head>
    <title>NFC Order</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="assets/css/main.css" />
    <script src="https://www.gstatic.com/firebasejs/7.14.5/firebase-app.js"></script>
    <script src="https://www.gstatic.com/firebasejs/4.10.1/firebase.js"></script>
    <script src="assets/js/config.js"></script>
  </head></code>

# Web Banner
  <body>
	<!-- Banner -->
		<section id="banner" style="height: 10px;" img src="images/banner_1.jpg">
		   <div class="inner">
		      <header>
			<h1>NFC Order</h1>
		      </header>
		    </div>
		</section>

# 각 table 별로 box를 만들어 주문 내용 표시, DOM 형태로 Pos기 화면을 구현하였다.
# table 위치를 나타낸 이미지가 상단에 뜨며, 주문한 메뉴와 state값, 제조 완료 버튼이 있다.

	 <!-- Main -->
		<div id="main">
		  <div class="inner">
		    <!-- Boxes -->
		     <div class="thumbnails">
			<div class="box">
			   <a class="image fit"><img src="images/table_1.jpg" alt="" /></a>
			   <div class="inner">
			      <h3>테이블 1</h3>
			      <p style="margin-bottom:10px;">◆시킨 메뉴◆</p>
			      <div id="getmenu1"></div>
			      state 값: <h1 id="state1"></h1>
			      <a class="button fit" onclick="changestate(this);">준비 완료</a>
			    </div>
		         </div>
