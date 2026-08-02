# webpag_test_1

GitHub Pages 로 배포하는 정적 웹 페이지입니다. 빌드 도구나 의존성 없이 HTML/CSS 파일이 그대로 배포 산출물이 됩니다.

**배포 주소:** https://jsoncorp.github.io/webpag_test_1/

📖 **처음 하시는 분은 [GitHub Pages로 내 웹페이지 무료 배포하기](docs/blog-post.md)** 를 보세요. 저장소 생성부터 Pages 설정까지 화면 캡처와 함께 정리해 뒀습니다.

## 구조

```
index.html    페이지 본문
style.css     스타일 (라이트/다크 자동 전환, 반응형)
.nojekyll     Pages 의 Jekyll 전처리 생략
```

## 로컬 미리보기

```bash
python -m http.server 8000
```

브라우저에서 http://localhost:8000 접속.

## 배포

`main` 브랜치 루트가 Pages 소스로 지정되어 있습니다. push 하면 1~2분 내 자동 반영됩니다.

```bash
git add -A
git commit -m "update"
git push
```

## 참고

- 프로젝트 페이지라 사이트가 `/webpag_test_1/` 하위 경로에 서빙됩니다. CSS·이미지·링크는 루트 절대경로(`/style.css`)가 아닌 **상대경로**(`style.css`)로 작성해야 합니다.
- 배포 상태는 저장소의 **Settings → Pages** 또는 **Actions** 탭에서 확인할 수 있습니다.
