# Knowledge Base

이 레포는 학습한 내용을 정리하고, PR 기반으로 관리하는 Knowledge Base 레포입니다.  
문서는 Obsidian에서 작성하고, GitHub에서 이력과 변경 사항을 관리합니다.

---

## 목적

- 학습 내용을 Markdown 문서로 축적
- 문서 간 링크를 통해 지식 구조화
- 브랜치 / 커밋 / PR 단위로 변경 이력 관리
- 향후 GitHub Pages 등으로 외부 공개 가능하도록 설계

---

## 작업 흐름

기본 작업 순서는 아래와 같습니다.

1. `main` 브랜치에서 최신 내용 pull
2. 새 작업용 브랜치 생성
3. Obsidian에서 문서 작성 또는 수정
4. 변경 파일 확인
5. 커밋 작성
6. Pull Request 생성
7. 검토 후 `main`에 머지

---

## 브랜치 규칙

작업 내용에 따라 아래 규칙으로 브랜치를 생성합니다.

- `docs/{topic}`: 문서 작성 / 수정
- `feat/{topic}`: 기능성 요소 추가
- `chore/{topic}`: 구조 변경, 설정 작업
- `fix/{topic}`: 오타, 링크 오류, 잘못된 내용 수정

### 예시

- `docs/readme-guide`
- `docs/rag-overview`
- `chore/folder-structure`
- `feat/github-pages`

### 브랜치 생성 방법

```bash
git checkout main
git pull origin main
git checkout -b docs/readme-guide