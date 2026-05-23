# Agent Ops Command Pack Samples

These are free samples from the full Korean command-template pack.

## Incident Triage

```text
이 알림이 실제로 현재도 진행 중인 장애인지 확인해줘. 배포 시각, 헬스체크, 에러 로그, 관련 API 응답을 나눠서 보고, 이미 종료된 과거 알림이면 그렇게 표시해줘.
```

## Production Deploy Smoke

```text
배포가 끝났다고 가정하지 말고 실제 프로덕션 주소 기준으로 확인해줘. 헬스체크, 핵심 API, 주요 화면, 콘솔/네트워크 에러, 데이터 반영 여부를 확인하고 결과를 표로 남겨줘.
```

## Code Review

```text
코드 리뷰 모드로 봐줘. 칭찬보다 버그, 회귀, 보안, 누락 테스트를 먼저 찾아줘. 파일/라인 근거를 붙이고, 심각도 순서로 정리해줘.
```

## Data Correction

```text
실제 데이터를 수정하기 전에 읽기 전용 쿼리로 현재 상태를 증명해줘. 어떤 row를 왜 바꾸는지, 변경 전 값과 변경 후 예상 값을 먼저 보여줘. 수정 후에는 같은 기준으로 재조회하고 감사 로그를 남겨줘.
```

## Pivot Decision

```text
이 방향이 계속할 가치가 있는지 냉정하게 판단해줘. 막힌 이유가 계정/권한/외부 승인 때문인지, 기술적으로 해결 가능한 문제인지, 아니면 기대값이 낮은 길인지 나눠서 말해줘. 아니다 싶으면 다음 후보로 바로 넘어가줘.
```

## Full Pack Contents

The paid pack adds more templates and reusable files:

- More operation prompts
- Deployment risk prompts
- Frontend bug prompts
- PR documentation prompts
- Checkpoint JSON template
- Incident report template
- Production smoke checklist

