# 캐릭터 아카이브

캐릭터 프로필과 로그를 보관하는 정적 사이트예요. 서버 없이 GitHub Pages로 돌아가요.

## 폴더 구성

```
index.html        보는 페이지 (홈 / 프로필 / 로그)
admin.html        편집기 (캐릭터·사진·로그 추가/수정)
data/archive.js   모든 글 데이터 (편집기가 자동으로 갱신해요)
images/           캐릭터 사진 (편집기가 자동으로 채워요)
```

## 1. GitHub에 올리기 (처음 한 번)

1. GitHub에서 **New repository** → 이름은 `character-archive` 같은 걸로, **Public** 으로 만들어요. (무료 플랜은 Public이어야 Pages가 돼요)
2. 만든 저장소에서 **uploading an existing file** → 이 폴더 안의 `index.html`, `admin.html`, `README.md`, `data` 폴더를 끌어다 놓고 Commit.
3. **Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save**
4. 1~2분 뒤 `https://<내아이디>.github.io/<저장소이름>/` 에서 열려요. 편집기는 주소 뒤에 `admin.html`.

> 저장소와 사이트는 누구나 볼 수 있어요. 공개하기 싫은 내용은 올리지 마세요. `admin.html` 주소는 링크를 모르면 찾기 어렵지만 비밀번호가 걸려 있진 않아요. (토큰 없이는 저장은 못 해요)

## 2. 편집기 쓰기

`admin.html` 을 열고 (내 컴퓨터에서 파일을 바로 열어도, 사이트 주소로 열어도 돼요)

- **사이트** 탭: 홈 제목/소개 문구
- **캐릭터** 탭: 정보, 사진 여러 장(첫 장이 대표), 설명, 특이사항, 한마디, 추가 항목
- **로그** 탭: 제목, 날짜, 캐릭터(한 명), 본문

작성 내용은 자동으로 브라우저에 임시 저장돼요. 저장 방법은 둘 중 하나:

**A. GitHub에 바로 저장 (추천)**
1. [토큰 만들기](https://github.com/settings/personal-access-tokens/new) → Repository access: *Only select repositories* → 이 저장소만 → Permissions: **Contents: Read and write**
2. 편집기의 **GitHub 설정**에 아이디 / 저장소 / 브랜치(main) / 토큰 입력
3. **GitHub에 저장** 버튼 → 1~2분 뒤 사이트에 반영

토큰은 비밀번호와 같아요. 남에게 보여 주거나 저장소에 올리지 마세요. 공용 PC에서는 쓰지 말고, 쓴 뒤 **토큰 삭제**를 눌러요.

**B. ZIP으로 내보내기**
**ZIP으로 내보내기** → 압축을 풀어 나온 `data`, `images` 폴더를 저장소에 업로드(덮어쓰기).

## 3. 로그 본문 쓰는 법

- 서술은 그냥 적어요.
- `"…"` `“…”` `「…」` `『…』` 로 감싼 부분은 대사로 강조돼요.
- 줄 맨 앞에 `>` 를 붙이면 내 대사/행동으로 따로 표시돼요.
- `---` 한 줄은 장면 구분선이에요.
- 빈 줄은 그대로 간격이 돼요.

## 4. 프로필 쓰기 팁

- 설명: 빈 줄로 문단을 나눠요.
- 특이사항·한마디: 한 줄에 하나씩, 가운데 정렬로 보여요.
- 관계인물에 등록된 캐릭터 이름을 적으면 자동으로 그 프로필로 링크돼요.
- 테마곡에 `https://` 링크를 넣으면 눌러서 열려요.
