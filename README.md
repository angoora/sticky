# sticky
sticky : 스크롤 발생시 엘리먼트를 상단에 고정

jquery 라이브러리를 사용합니다.

[기능] 
1. window 상하스크롤이 발생시 엘리먼트를 화면상단에 고정.
2. 반응형에서도 엘리먼트의 크기와 위치가 조정됨.

[방법]
1. jquery 사용.
2. sticky() 함수를 선언하고 문서가 준비되면 호출.
3. 고정시키고자 하는 엘리먼트에 stick 클래스 부여.

[URL]
https://angoora.github.io/sticky/sticky.html


[문제상황]
1. 후처리시 과정에서 엘리먼트에 margin-top 값이 있는 경우 그 값만큼 화면상단에 여백이 발생함.
2. 엘리먼트의 margin-top 값을 구하고 position top에 음수값을 부여하여 여백을 감출수 있으나 스타일에 따라 margin-top이 들어가는 경우도 있으므로 모든 유형을 맞출수가 없음.

결론 - 후처리 과정에서 엘리먼트의 margin 값으로 인한 여백 발생시 margin-top을 제거하고 스타일 수정.