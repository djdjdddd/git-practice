Branch Protection Rule 테스트
- `main`과 `release` 브랜치는 보호 받고 있습니다.
- (1) direct push 금지
- (2) merge 전 PR 요구

테스트 실패
- `release/**` 라고 입력하여 실패
- `release/*` 로 재입력 후 재시도