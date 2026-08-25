# BENCH — 학교용 (bench-school)

3D 프린팅 도구 모음의 **학교용** 배포본입니다. 한국어 전용이며 Sindoh 3DWOX1 / 1X / 7X 프로필이 저장되어 있습니다. 다른 프린터를 쓸 때는 프린터 선택에서 "직접 입력 — 다른 프린터"를 고르고 베드 가로·세로·최대 높이를 mm로 입력하세요.

```
index.html      대시보드 (단일 파일, 오프라인 동작)
tools/          도구별 폴더 — 원본 저장소에서 복사해 넣으세요
```

## GitHub Pages로 올리기

1. GitHub에서 새 저장소 `bench-school`을 만듭니다 (Private 권장).
2. 이 폴더의 `index.html`을 저장소 루트에 올립니다.
3. 원본 저장소(`3D-website`)의 `tools/` 폴더를 그대로 복사해 같은 루트에 넣습니다.
4. Settings → Pages → Source: `Deploy from a branch`, Branch: `main` / `(root)` → Save.
5. 몇 분 뒤 `https://<계정>.github.io/bench-school/` 에서 열립니다.

## 도구 링크 주소 바꾸기

`index.html` 안의 아래 한 줄이 도구 페이지의 기준 주소입니다. 3번에서 `tools/`를 같은 저장소에 넣었다면 상대 경로로 바꾸세요.

```js
const SITE = 'https://yeseul100512.github.io/3D-website/';   // → './'
```
