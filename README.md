# visual studio code (VS code) 
* vs code 실행 시 가장 먼저 확인해야 할 것
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인하기
* (위) -> 안되었다면 파일 - 작업 폴더 닫기 - 폴더 열기 후 다시 진행
# html 시작
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전선언
* `<!DOCTYPE html>`
## HTML 구조태그
* html: 웹의 시작과 끝, 문서 자체 의미.
* head: 웹 문서의 정보, 제목 포함
* meta: 웹 문서의 정보 기록
* title: 웹 문서의 제목 (브라우저 상단 표시)
* body: 웹 문서 내용 (실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html 문서 언어 설정
* `charset="uft-8"` 다국어 문자열 설정
* `description` 사이트 검색 키워드
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백 (속성 개수 제한 없음)
* 속성은 시작태그에만 작성하기
## 구조태그와 'title' 작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 ㅣ 광고문구추가
* 서브페이지 -> 페이지명 ㅣ 사이트명
* ex) 책이름 - 저자명 ㅣ 서점명
* ex) 판매페이지명 ㅣ 사이트명
## h1~h6 제목태그
* h1~h3 태그는 meta keywords와 동일한 검색키워드로 활용된다. [대제목일 수록 높음]
* h4~h6 태그는 거의 사용하지 않는다.
* h1은 사이트의 로고 및, 서브 페이지 제목에서 주로 사용한다.
* h 제목의 1~6 레벨은 순서대로 작성해야 한다.
## 단락 p(block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h) 태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식(x)
## 인라인 태그 br, em, strong, del, s, sup, sub
* `br` : 블록 내 줄바꿈
* `em` : 블록 내 강조 태그, 주로 내용 태그 (p) 등에서 자식으로 사용
* `strong` : 블록 내 경고 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주 사용)
* `sup, sub` : 윗첨자, 아랫첨자, 수학, 과학 등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, q 태그와 부모-자식 관계로 사용해선 안된다.
* `q(inline)` : 단락 내에서 일부 인용문에 해당할 때 사용
* 공통속성 `cite="URL"` : `blockquote`, `q` 로 인용은 처리할 경우 출처표시 용도로 주소를 담아주는 속성
## 특수문자 태그 copy, reg
* `&` : 시작 `;` : 종료
* `&copy;` : 페이지 하단에 나와있는 저작권(카피라이트) 마크 표시
# 주소태그 address
* `address` : 연락처, 회사소개, 고객센터 등에 사용, 다른 블록을 자식이나 자손으로 배치할 수 없어 Inline에만 사용 가능하다.
# 수평선 태그 hr
* `hr` : 회색 수평선 태그. 각 영역을 구분하는 목적으로 쓰인다.
# 컴퓨터 명령어 태그 code, lt, gt
* `code` : html 코드를 입력해야 할 때 사용하는 태그
* `&lt` : 왼쪽 꺽새
* `&gt` : 오른쪽 꺽새
# 링크태그 a
* block, Inline 특성을 모두 가진다.
* 절대경로와 상대경로를 href 속성에 작성한다.
* 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다.
* `./` : 현재 위치에서 시작
* `../` : 상위 폴더로 나가기
* `.doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
* `../doll.jpg` : 사우이 폴더로 한단계 나가서 doll.jpg 파일 찾기
* `../a/doll.jpg` : 상위 폴더로 한단계 나가고 a 폴더로 들어가서 doll.jpg 파일 찾기
* `./b/doll/jpg` : 현재위치에서 b 폴더로 들어가 doll.jpg 파일 찾기
## 바로가기 링크란?
* <a href="#id"> 바로가기 링크 속성 (페이지가 없을 시에는 임시로 "#" 페이지 사용)
* 
## 바로가기 링크 제작 순서 및 주의사항
* 바로가기 이름을 붙여준 뒤 태그를 사용할 때 이름 왼쪽에 #을 작성해야 적용된다.
* 
## 파비콘 적용 순서
*   <link rel="shortcut icon" href="파비콘.ico 경로" type="image/x-icon"> 
    <link rel="icon" href="파비콘.ico 경로" type="image/x-icon">
*   탭 및 작업표시줄 등에 웹을 구분 가능하게 하는 아이콘
## 이미지태그 `img`
* `img` 태그를 사용할 땐 반드시 끝에 `alt=""` 속성을 필수로 함께 작성해야 한다.
* 이미지 사용 시 의미전달이 필요한 이미지와 아닌 이미지를 구분해서 사용해야 한다. 필요하지 않을 경우 alt는 공백으로 둔다.
## 문서 안 사진을 감싸는 틀 `figure` `figcaption`
* `figure` 이미지 태그 바깥 쪽에 삽입을 하면 그 안에 있는 블럭들이 모두 선택된다. 
* `figcaption` 문서 안 사진을 감싸는 틀로써 활용하고 사진의 캡션을 정의할 수 있다.
## 비디오태그 `video`
* 1. 영상이 하나일 경우
    <video src=”동영상 경로”></viedo>
* 2. 호환성때문에 같은 영상을 여러 개 준비했을 경우
    <video>
    <souroe src=”동영상 경로” type=”동영상타입1”>
    <souroe src=”동영상 경로” type=”동영상타입2”>
    </video>
* <video src="./video/cat.mp4" autoplay muted loop controls></video>
* 오토플레이는 재생, 뮤트는 음소거 (새로고침 하자마자 영상 재생) 루프는 반복재생, 컨트롤은 재생바 
* 유튜브 영상을 가져올 경우 URL주소 마지막에 ;을 붙인 뒤 부가태그를 삽입하고 &을 붙여 이어서 삽입한다. 
## class , id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* 예: 의미있는 단어_영역명
* 예시: product_wrap, item_area, price_g, main_contents
## `div, spen` 그룹태그
### `div`
* 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
### span
* 인라인에 2개 이상 형제일 경우 주는 그룹 태그
* 의미없는 디자인 요소 인라인 처리 필요 시 사용
## `HTML5 semantic tag`
### semantic tag란?
* HTML5에서 생성된 의미있는(semantic) 태그
### `header`
* 로고 및 내비게이션을 묶어주는 웹 사이트 레이아웃 태그
* 제목, 로고, 검색 폼, 작성자 이름 등 요소 포함
### `nav`
* 메뉴, 목차 등 주요 카테고리를 묶어주는 웹 사이트 레이아웃 태그
### `gnb, lnb, snb`
* gnb (global navigation bar) - nav 묶이는 대상**
* lnb (local navigation bar)**
* snb (side navigation bar)**
## `ul, ol, li`
* 순서가 중요한 2개 이상의 목록(li) 구조을 묶어주는 그룹태그
* 목록의 순서와 연관이 있을 경우 ol 사용, 없으면 ul 사용
* 순서가 있다는 가정하에 oi - li 반복 가능
* 순차/비순차 목록 사용 시 다른 블록 및 인라인 태그를 사용하려면 반드시 li 안 자식위치로 배치해야한다
* ul 또는 ol 과 li 사이에 다른 태그를 삽입하지 않도록 주의
## `details, summary`
* '열림' 상태일 때만 내부 정보를 보여주는 정보 공개 위젯을 생성 (요약, 더보기)
* <details>
    <summary>요약</summary>
    <spam>내용</span>
    </details>
## ` footer, mark, main, time`
* `footer` : 웹페이지 가장 하단에 위치하며 작성자, 저작권 정보, 관련 문서 등의 내용 등 삽입
* `mark` : 현재 맥락에 관련이 깊거나 중요해 표시한 부분 (노란 형광펜 형태)
* `main` :  문서 <body>의 주요 콘텐츠
* `time` : 시간의 특정 지점 또는 구간
## `dl, dt, dd`
* `dl` : 정의형 제목과 내용을 묶는 그룹
* `dt` : dl 안 자식으로 배치되며 제목을 의미
* `dd` : dl 자식으로 배치되며 dt 다음 형제 요소로 배치된다
* <dl>
    <dt>정의형 제목</dt>
        <dd>내용</dd>
  </dl>