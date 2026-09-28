# package-publish-workflows

Com2uS Platform 제품의 패키지 레지스트리 게시용 Reusable Workflow입니다.

**이 저장소는 Official Repository가 아닙니다.** 제품 코드와 설치 안내는 각 제품의 Official Repository에 있습니다.

- 각 Official Repository의 진입점 Workflow가 이 저장소의 Workflow를 전체 Commit SHA로 호출합니다.
- 이 저장소에는 Secret과 인증정보를 두지 않습니다. 게시 자격증명은 호출한 저장소의 Workflow가 OIDC로 발급받습니다.
- 변경은 Pull Request와 code owner 승인으로만 반영합니다.

| Workflow | 레지스트리 | 상태 |
| --- | --- | --- |
| `npm-publish.yml` | npm | 리허설 전 |
