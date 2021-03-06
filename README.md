# Hyodu Website
**nana@thevitolabs.com**
<br/>

최종 수정일: 2020-01-17
<br/>

## 전달 사항 (20.01.17)
- 기존에 `.page-body` 아래에 있던 `.page-content`의 이름을 `.page-layout`으로 수정했습니다. content를 layout으로 **클래스 네임 수정** 부탁드립니다~!
- 이미지 폴더에 하위 폴더를 나누어 이미지를 분류했습니다. `temp/` 폴더 내의 이미지는 임시용이니 지우셔도 됩니다. 
- 이미지는 `dist/images/` 폴더의 것을 사용하시면 좋습니다. (압축시켜서 용량이 더 작습니다!)
- 모달이 열렸을 때 스크롤을 막는 과정이 복잡해져서, 모바일 버거메뉴를 열었을 때만 스크롤 막는 것으로 변경했습니다.

## 폴더 구조
- 크게 `src/`와 `dist/`로 나뉩니다.
- `src/`는 제가 작업한 원본파일(scss 파일 등)이 들어있고, `dist/`는 컴파일 및 압축한 파일이 들어있습니다.
- 하위 구조는 아래와 같습니다.
  - html/
  - css/ 또는 scss/
  - images/
  - js/
  - fileList.html

## HTML
- `fileList.html`에 정리해 놓았습니다. 작업한 파일은 이렇게 테이블로 정리해서 보내드릴 예정입니다.
- 확인이 필요한 부분은 html 파일 내에 `<!--[전달사항]-->`으로 주석을 달아놓았습니다.

## CSS
- 반응형으로 모바일과 데스크탑에 대응하며, 분기점은 1060px 입니다.
- 폰트 파일은 Noto Sans(본고딕)을 CDN으로 불러와 사용 중입니다.
- 구 버전 IE에 대한 대응은 매우 제한적이며, 최소 Edge부터 호환됩니다.

## JS
- 일부 동작에 대해 임의의 스크립트를 작성했습니다.
- 각 js 파일 안에 세세하게 주석을 달아놓았습니다. 파일 별로 다루는 내용은 아래와 같습니다.
  - common.js : 스크롤을 허용하고 막는 이벤트
  - modal.js : 모달을 여닫는 이벤트
  - header.js : 모바일에서 버거메뉴로 헤더를 여닫는 이벤트, 데스크탑에서 이메일 클릭 시 작은 네비를 여닫는 이벤트 등
  - animation.js : UI 상에서 애니메이션이 들어가야하는 이벤트 (공유하기 모달, 문의 목록 아코디언, 리뷰 작성 시 별점 매기기 등)
