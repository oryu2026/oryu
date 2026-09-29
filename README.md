# 오류고등학교 VR 학교 안내 웹 브로셔

360도 사진으로 교정을 둘러보는 오류고등학교 웹 브로셔입니다. `index.html` 한 파일에 이미지·배경음악·아이콘이 모두 포함되어 있어(약 5MB), 별도의 파일이나 빌드 과정 없이 그대로 정적 호스팅할 수 있습니다.

## GitHub Pages로 호스팅하기

1. 이 저장소(`oryu2026/oryu`)에 `index.html`을 커밋·푸시합니다.
2. GitHub 저장소 페이지에서 **Settings → Pages**로 이동합니다.
3. **Build and deployment → Source**를 `Deploy from a branch`로 두고, **Branch**를 `main`(또는 기본 브랜치), 폴더를 `/ (root)`로 선택한 뒤 저장합니다.
4. 잠시 후 `https://oryu2026.github.io/oryu/` 주소로 접속하면 브로셔가 바로 열립니다.

## 로컬에서 미리보기

```bash
git clone https://github.com/oryu2026/oryu.git
cd oryu
# index.html을 더블클릭해서 열거나:
python3 -m http.server 8000
# 이후 브라우저에서 http://localhost:8000 접속
```

## 참고

- 배경음악, 4장의 360도 사진, 파비콘이 모두 `index.html` 안에 base64로 포함되어 있어 인터넷 연결 없이도(로컬 파일로 열어도) 정상 동작합니다.
- 온라인 문의 버튼은 별도의 구글 설문 링크로 연결됩니다.
- 사진이나 문구를 바꾸려면 `index.html`을 다시 생성해서 같은 이름으로 덮어써 주세요.
