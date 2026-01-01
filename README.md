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
   pip install -r requirements.txt
   ```
2. 문서 서버 실행
   ```bash
   mkdocs serve
   ```
   - 기본 포트: http://127.0.0.1:8000

## GitHub Pages 배포 (예시)
1. `mkdocs.yml`의 `site_url`을 자신의 GitHub Pages URL로 수정합니다.
2. Codespaces나 로컬에서 다음을 실행합니다.
   ```bash
   mkdocs build
   mkdocs gh-deploy --force
   ```
3. GitHub Pages 설정에서 `gh-pages` 브랜치를 소스로 선택합니다.
4. 배포 후 `https://<github-id>.github.io/<repo-name>/`에서 사이트를 확인합니다.

> 이 위키는 “3GPP를 읽는 곳”이 아니라 “3GPP로 구현하는 곳”입니다.

## Codespaces 빠른 시작 (브랜치 생성 → 설치 → 빌드)
> Codespaces에서 MkDocs를 바로 돌릴 때 따라 하면 됩니다.

1. 작업 브랜치 생성 (예: `mkdocs`)
   ```bash
   git checkout -b mkdocs
   ```
2. 의존성 설치
   ```bash
   pip install -r requirements.txt
   ```
3. 로컬 빌드로 정적 산출물 확인 (정상 시 `site/` 생성)
   ```bash
   mkdocs build
   ```
4. 실시간 미리보기 (포트 포워딩 사용)
   ```bash
   mkdocs serve --dev-addr=0.0.0.0:8000
   ```
   - Codespaces 포트 포워딩에서 8000 공개 후 접속: `https://<codespace-url>/`
5. 배포 (옵션: GitHub Pages)
   ```bash
   mkdocs gh-deploy --force
   ```
6. 푸시
   ```bash
   git push origin mkdocs
   ```
