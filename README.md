# codyssey_git_workflow

실전 Git 협업 워크플로우 미션 저장소입니다.

3인 팀이 GitHub Flow를 적용하여 브랜치 · PR · 코드 리뷰 · 이슈 연동 · 충돌 해결 · 트러블슈팅을 실습하고, 그 과정을 문서로 남깁니다. 복잡한 기능 구현이 아니라 **협업 과정 자체**가 목적이므로, 결과물은 팀원 소개 문서로 갈음합니다.

---

## 👥 팀원 소개

| 이름 | GitHub | 한 줄 소개 | 소개 문서 |
| --- | --- | --- | --- |
| 임대균 | [@yun-lim](https://github.com/yun-lim) | AI, Agent, Product를 좋아하는 마리너입니다. | [team/yun-lim.md](./team/yun-lim.md) |
| 신희수 | [@star-candy](https://github.com/star-candy) | ai, 정보보안에 관심이 있는 마리너입니다. 잘부탁드립니다! | [team/star-candy.md](./team/star-candy.md) |
| 이동현 | [@mov-hyun](https://github.com/mov-hyun) | AI로 새로운 가치를 만들어가고자 하는 이동현 마리너입니다. | [team/mov-hyun.md](./team/mov-hyun.md) |

---

## 📚 문서

| 문서 | 내용 |
| --- | --- |
| [docs/CONTRIBUTING.md](./docs/CONTRIBUTING.md) | 브랜치 전략, 브랜치 네이밍, 커밋 컨벤션, PR · 코드 리뷰 규칙, 충돌 대응 흐름 |
| [docs/conflict-resolution.md](./docs/conflict-resolution.md) | 충돌 발생 상황과 해결 과정 기록 |
| [docs/troubleshooting-log.md](./docs/troubleshooting-log.md) | Git 트러블슈팅 실습 기록 |
| [SUBMISSION.md](./SUBMISSION.md) | 제출물 인덱스 (팀원별 Issue · PR 링크, Git 히스토리 증빙) |

---

## 🌿 브랜치 전략

`main`은 항상 배포 가능한 상태를 유지하며, 모든 작업은 `feature/*` 브랜치에서 진행한 뒤 PR과 리뷰 승인을 거쳐 병합합니다.

GitHub Flow를 선택한 이유와 상세 규칙은 [docs/CONTRIBUTING.md](./docs/CONTRIBUTING.md)에 정리되어 있습니다.
