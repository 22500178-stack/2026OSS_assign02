# 22500178 김지원

# Assignment 02 수행 내용
이번 과제에서는 동일한 HTML 구조에 서로 다른 CSS를 적용해 페이지의 모습이 어떻게 달라지는지 실습하고, Bootstrap 프레임워크를 사용해보았다.

# 각 페이지 설명 및 URL
nostyle.html : CSS를 적용하지 않은 기본 HTML 구조 
style1.html : nostyle.html과 동일한 HTML에 CSS(그린 테마, Grid 레이아웃)를 적용
style2.html : nostyle.html과 동일한 HTML에 CSS(테라코타 테마, Grid 레이아웃)를 적용
bootstrap_ex.html : Bootstrap CDN을 이용해 Navbar, Hero, Features, Footer로 구성한 예제 페이지
index.html : 위 4개 페이지로 이동할 수 있는 목차 페이지

# Vercel Deploy URL

# Key Learning: 이번 주 배운 핵심 내용 3가지
- HTML은 화면의 구조와 영역을 담당하고, 디자인적인 부분은 CSS가 담당한다는 것을 알게되었다.
- CSS Grid를 쓰면 태그 순서를 안 바꿔도 원하는 자리에 요소를 놓을 수 있다는 것을 알게되었다.
- 페이지끼리 <a href="파일명">으로 서로 연결해야 클릭했을 때 실제로 이동한다는 것을 알게되었다.

# HTML vs CSS: HTML과 CSS의 역할을 자신의 말로 간단히 정리
HTML은 웹페이지 안에 어떤 내용을 넣을지를 정하는 것이고, CSS는 그 내용은 어떻게 보여줄지에 관한 것이다. 제목, 첫 번째 문단, 두 번째 문단, 목록과 같은 콘텐츠의 구조나 내용은 HTML이 담당하고, 그 내용의 폰트나 글자크기, 색상 등은 CSS가 담당하는 것이다.

# Bootstrap 사용법 : Bootstrap 사용하는 이유 및 사용법 간단히 정리
Bootstrap은 미리 만들어진 CSS 스타일 모음이다. 원래는 버튼 하나를 예쁘게 꾸미려고 해도 CSS를 직접 써야 하는데, Bootstrap을 쓰면 그럴 필요가 없다.
사용법은 <head>에 Bootstrap CDN 링크를 한 줄 추가하고, 꾸미고 싶은 태그에 정해진 class 이름을 붙인다.

# Problem & Solution: 실습 중 발생한 문제와 해결 과정 1가지
style1.html을 만들 때 HTML은 nostyle.html이랑 똑같이 둬야 하는데, 원본처럼 사이드바를 오른쪽에 배치하려니 잘 안 됐다. 사이드바 div가 본문보다 뒤에 있어서 그냥 CSS로는 오른쪽으로 안 옮겨졌다. 하지만 CSS Grid를 쓰면 HTML 순서를 안 바꿔도 원하는 위치에 요소를 놓을 수 있다는 것을 알게되었다. 각 요소에 grid-area 이름만 지정해서 메뉴, 본문, 사이드바를 원하는 자리에 배치해 해결했다.

# AI Usage: AI를 어떤 부분에 활용했으며, 생성된 코드를 어떻게 확인/수정했는지 작성
- style1.html을 만들 때 HTML은 nostyle.html이랑 똑같이 둬야 하는데, 원본처럼 사이드바를 오른쪽에 배치하려니 잘 안 됐다. AI에게 이 문제를 물어보니 CSS Grid를 쓰면 HTML 순서를 안 바꿔도 원하는 위치에 요소를 놓을 수 있다는 걸 알려주었고, 각 요소에 grid-area 이름만 지정해서 메뉴, 본문, 사이드바를 원하는 자리에 배치해 해결하였다. 
- Bootstrap에 대해 잘 이해가 안 갔었는데, AI에게 물어보면서 "CSS를 직접 안 써도 class만 붙이면 스타일이 적용된다"는 개념과 실제 사용법을 이해할 수 있었다.

# Reflection: 새롭게 알게 된 점 또는 궁금한 점 1가지
HTML 구조를 전혀 바꾸지 않고도 CSS Grid의 grid-area만 활용하면 화면 배치를 자유자재로 바꿀 수 있다는 것을 알게 되었다.