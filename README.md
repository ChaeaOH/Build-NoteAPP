#💻Build A Notes APP 
JavaScript을 기반으로 만들어진 노트 앱으로 노트 추가,편집,삭제기능을 가지고 있습니다.


# 🔍Detail
- forEach문을 통해 노트,인덱스 인자를 불러와 작성, 편집과,삭제기능을 구현하였습니다.
- `elem.insertAdjacentHTML` 메소드를 사용하여 메모가 작성된 후 (addBox) 바로 다음 요소에 새 노트가 생성됩니다.
- `Date` 객체의 메서드를 사용하면 연, 월, 일 등의 값을 얻어 노트를 작성한 날짜를 출력하였습니다.
- `confirm` 메소드를 사용하여 노트 삭제 알림창을 통해 true를 반환하여 확인 클릭시 노트가 삭제됩니다.
- 앱에 추가한 노트는 브라우저의 localStorage 에 저장되므로 페이지 새로 고침 또는 탭 닫기 시 제거되지않습니다.

# 🚀Result
![function](/기능구현.gif)


# 💡Review
- 기존의 노트가 편집된 후 업데이트된 새로운 노트가 추가됐는데 이 문제를 해결하기 위해 별도로 updateNote 함수를 만들어isUpdate=true 와 updateId=noteId;로 할당하여 추가버튼 이벤트리스터 함수에서 !isUpdate(비교연산자)를 통해 업데이트 내용이 아니라면 새로운 노트 추가시키는 방법을 배웠습니다.
- `elem.querySelectorAll` 요소 검색 메서드를 활용하여 elem의 자식 요소 중 주어진 CSS 선택자에 대응하는 요소 모두를 반환하는 방법을 배웠습니다.