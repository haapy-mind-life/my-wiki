# 3GPP Study Wiki (MkDocs)

3GPP 스펙을 개발 관점에서 학습하고 SW/Web App으로 연결하는 공개 위키 예제입니다. MkDocs(Material 테마)로 구성되어 GitHub Pages에 바로 배포할 수 있습니다.

## 구조
```
docs/
  specs/        # 3GPP 시리즈 요약
  breakdown/    # 절차별 메시지/상태 해설
  sw/           # SW 설계 아이디어
  webapp/       # Web App/시각화 아이디어
  reference/    # 용어집 및 링크
mkdocs.yml
```

## 로컬 미리보기
1. 의존성 설치
   ```bash
   pip install mkdocs-material
   ```
2. 문서 서버 실행
   ```bash
   mkdocs serve
   ```
   - 기본 포트: http://127.0.0.1:8000

## GitHub Pages 배포 (예시)
1. `site_url`을 자신의 GitHub Pages URL로 수정합니다.
2. 배포 실행
   ```bash
   mkdocs gh-deploy --force
   ```
3. GitHub Pages 설정에서 `gh-pages` 브랜치를 소스로 선택합니다.

> 이 위키는 “3GPP를 읽는 곳”이 아니라 “3GPP로 구현하는 곳”입니다.
