# HealthData DCAT-AP 명세 (ReSpec)

DCAT-AP / HealthDCAT-AP 기반 보건의료 데이터 메타데이터 명세입니다.
[DCAT-AP-KR]([https://vocab.datahub.kr/def/dcat-ap-kr/]) 와 동일한 ReSpec(W3C 명세) 스타일로 작성되었습니다.
좌측 목차(TOC)는 ReSpec이 자동 생성하며, 각 속성 우측 배지는 중개포털(안) 기준 요구 수준입니다.

## 로컬 미리보기
`index.html`을 브라우저로 직접 열면 됩니다. (ReSpec 스크립트는 CDN에서 자동 로드)
간단히 로컬 서버로 보려면:

```bash
python -m http.server 8000
# http://localhost:8000 접속
```

## GitHub Pages 배포

### 1) 저장소 생성 & 업로드
```bash
git init
git add .
git commit -m "add healthdata dcat-ap spec"
git branch -M main
git remote add origin https://github.com/kdyoung100/healthdata-spec.git
git push -u origin main
```

### 2) Pages 활성화
GitHub 저장소 → Settings → Pages → **Build and deployment → Source: GitHub Actions** 선택.
push하면 `.github/workflows/pages.yml`이 자동 배포합니다.
배포 후 주소: `https://<username>.github.io/healthdata-spec/`

### 설정 수정
`index.html` 상단 `respecConfig`의 `editors`, `github`, `edDraftURI`를 본인 정보로 바꾸세요.
