---
layout: post
title: "비밀번호 보호 포스트"
date: 2024-10-17
categories: [비공식]
---

<h2>비밀번호 입력</h2>
<input type="password" id="password" placeholder="비밀번호를 입력하세요">
<button onclick="checkPassword()">확인</button>
<div id="content" style="display:none;">
  <h3>비밀번호 보호된 내용</h3>
  <p>여기에 비밀번호로 보호된 포스트 내용이 들어갑니다.</p>
</div>



<script>
function checkPassword() {
  const password = document.getElementById("password").value;
  const correctPassword = "1234"; // 여기에 원하는 비밀번호를 입력하세요.
  if (password === correctPassword) {
    document.getElementById("content").style.display = "block";
  } else {
    alert("비밀번호가 잘못되었습니다.");
  }
}
</script>
