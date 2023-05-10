## [4Week] 박진영

### 미션 요구사항 분석 & 체크리스트

---  

**[사전작업]**
- 번역 작업


###
**[필수과제]** 네이버클라우드플랫폼을 통한 배포, 도메인, HTTPS 까지 적용
- [x] https://www.codelike.jny0.xyz 에서 접속 가능
- [x] 운영서버에서 각종 소셜로그인, 인스타 아이디 연결이 잘 되야함


###
**[필수과제]** 내가 받은 호감리스트(/usr/likeablePerson/toList)에서 성별 필터링기능 구현
- [x] UI 작업
- [x] 특정 성별을 가진 사람에게서 받은 호감만 필터링해서 볼 수 있음

###
**[선택과제]** 젠킨스를 통해서 리포지터리의 main 브랜치에 커밋 이벤트가 발생하면 자동으로 배포가 진행되도록

###
**[선택과제]**  내가 받은 호감리스트(/usr/likeablePerson/toList)에서 호감 사유 필터링 기능
- [x] 특정 호감사유에 대한 호감만 필터링해서 볼 수 있음


###
**[선택과제]**  내가 받은 호감리스트(/usr/likeablePerson/toList)에서 정렬기능
- [ ] 최신순(기본)
    - 가장 최근에 받은 호감표시를 우선적으로 표시
- [ ] 날짜순
  - 가장 오래전에 받은 호감표시를 우선적으로 표시
- [ ] 인기 많은 순
    - 가장 인기가 많은 사람들의 호감표시를 우선적으로 표시
- [ ] 인기 적은 순
    - 가장 인기가 적은 사람들의 호감표시를 우선적으로 표시
- [ ] 성별순
    - 여성에게 받은 호감표시를 먼저 표시하고, 그 다음 남자에게 받은 호감표시를 후에 표시
  - 2순위 정렬조건으로는 최신순
- [ ] 호감사유순
  - 외모 때문에 받은 호감표시를 먼저 표시하고, 그 다음 성격 때문에 받은 호감표시를 후에 표시, 마지막으로 능력 때문에 받은 호감표시를 후에 표시
  - 2순위 정렬조건으로는 최신순



###
### 4주차 미션 요약

---  

**[접근 방법]**
1. toList에서 성별 및 호감사유 필터링
- `@RequestParam` 어노테이션을 사용하여 `gender`와 `attractiveTypeCode` 파라미터를 받아와 필터링하는 로직 구현
- 성별을 선택하지 않고 호감 사유만 선택했을 때 필터링되지 않는 오류 해결해야함


###
**[특이사항]**