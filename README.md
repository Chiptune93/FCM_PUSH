## 2021.06.02

# FCM_PUSH
스프링 기반 웹 서비스에서 FCM을 통해 앱으로 푸시를 보내는 JAVA 예제입니다.
기본 구성은 다음과 같습니다.

- PUSH 를 보내는 Thread
- 해당 Thread 를 반복 실행하는 스케줄 빈(BEAN)

어디까지나 예제의 하나로써 제 경우에 맞추어 짜여진 코드이기 때문에
필요에 맞게 수정하셔서 사용하기바랍니다.

# 내부 요소

- 큐(Queue) 테이블이 존재하여 모든 전송해야하는 메세지는 해당 테이블에 저장된다.
- 메세지 전송에 대한 결과를 로그 테이블에 푸시 정보와 같이 저장한다.
- 단건 전송임.
- 스케줄링을 통해 지속적으로 체크하여 전송.



