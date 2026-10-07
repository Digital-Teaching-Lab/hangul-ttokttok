# 한글 톡톡 — GitHub + Vercel 배포 안내

이 폴더의 `index.html`이 게임 시작 페이지입니다. 정적 HTML 파일이라 별도의 빌드나 설치 없이 Vercel에 배포할 수 있습니다.

## 1. GitHub에 게임 파일 올리기

1. [GitHub](https://github.com)에 로그인하고 오른쪽 위 `+` → **New repository**를 선택합니다.
2. 저장소 이름을 `hangul-ttokttok`처럼 정합니다. 공개 범위는 원하시는 대로 **Private** 또는 **Public**을 선택합니다.
3. **Add a README file** 옵션은 선택하지 않아도 됩니다. **Create repository**를 누릅니다.
4. 새 저장소 화면에서 **Add file** → **Upload files**를 선택합니다.
5. 압축을 푼 이 폴더에서 `index.html`과 `README.md`를 업로드 영역으로 끌어다 놓습니다.
6. 아래 **Commit changes**를 눌러 저장합니다. `index.html`은 저장소 최상위에 있어야 합니다.

## 2. Vercel에서 GitHub 저장소 연결하기

1. [Vercel](https://vercel.com)에 로그인하고 **Continue with GitHub**로 계정을 연결합니다.
2. 대시보드에서 **Add New…** → **Project**를 선택합니다.
3. 방금 만든 `hangul-ttokttok` 저장소 옆의 **Import**를 누릅니다. 저장소가 보이지 않으면 GitHub 앱 권한 설정에서 해당 저장소 접근을 허용합니다.
4. 프로젝트 설정은 다음처럼 둡니다.
   - **Framework Preset:** Other
   - **Root Directory:** `./`
   - **Build Command:** 비워둠
   - **Output Directory:** `.`
5. **Deploy**를 누릅니다. 배포가 끝나면 `https://...vercel.app` 주소가 만들어지고, 주소를 열면 게임이 바로 시작됩니다.

## 3. 나중에 게임을 수정할 때

수정된 `index.html`을 같은 GitHub 저장소에 다시 업로드하고 변경 내용을 **Commit changes** 하면 Vercel이 새 버전을 자동 배포합니다.

## 게임 기록 관련

현재 게임의 오늘의 기록은 브라우저 페이지가 열려 있는 동안만 저장됩니다. 새로고침하거나 페이지를 닫으면 초기화되며, 기기 간 기록 공유나 영구 저장은 하지 않습니다.
