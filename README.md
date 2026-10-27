# 영업소장 대시보드

영업소장용 바로가기 페이지(외근 중 외부망·휴대폰 접속용). 영업관리팀용 `플랫폼 허브`(172.20.10.89:8002)를 복사해 만든 정적 HTML 페이지이며 GitHub Pages로 공개 서비스합니다. 허브 자체에는 비밀번호가 없습니다.

## 링크 추가/수정

구글시트만 편집하면 됩니다(새로고침 시 바로 반영). 영업관리 시트와 **별도 파일**입니다. 이 페이지가 공개되면 시트 ID도 공개되므로, 사내 IP 목록이 있는 영업관리 시트와 섞지 않습니다.

- 시트: https://docs.google.com/spreadsheets/d/14Hf32sz3B6EhnXAZjd4d0j25gc3TCLltAhTuGh5BzhI/edit?gid=0
- 컬럼: `구분` / `설명` / `URL` (첫 번째 탭)
- 공유 설정: 링크가 있는 모든 사용자 — 뷰어

## 카드 모양(배지·아이콘·색·사내망 전용 표시)

`index.html`의 `TYPE_MAP`에서 카드 이름(`구분` 값과 정확히 일치)으로 정합니다. 목록에 없는 이름은 기본 모양(폴더 아이콘, 남색)으로 나옵니다. 서비스가 외부에 열리면 해당 항목의 `internal`을 `false`로 바꿉니다.

## 배포

GitHub 저장소에 push하면 GitHub Pages가 1분 안팎으로 반영합니다.

- 주소: https://innodep-sales.github.io/
- 저장소: https://github.com/Innodep-Sales/innodep-sales.github.io (GitHub 조직 Innodep-Sales, 개인 계정 wkdwlstjr914-commits가 관리자)
