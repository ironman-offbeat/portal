# 이하영의 Offbeat 웹앱 포탈

흑백 타이포그래피 중심의 업무용 웹앱 바로가기 포탈입니다.

## 포함된 웹앱

| 웹앱 | URL |
| --- | --- |
| 계약서 및 주요문서 관리 | https://offbeat-document-hub.vercel.app/ |
| 임직원 근무시간 현황 | https://offbeat-working-hours-dashboard.vercel.app/ |
| 오프비트 주주/ 스톡옵션 관리 | https://offbeat-management-admin.vercel.app/ |
| 파트너스 포탈 | https://partners.offbeatplay.com/projects |
| 파트너스 포탈(어드민) | https://partners.offbeatplay.com/admin/users |
| 인사평가 결과 분석 리포트 | https://offbeat-review-dashboard.vercel.app/dashboard |
| 깃헙 전독시 리포트 아카이빙 | https://github.com/gitorvreport/orv-report |
| 매출 프로젝션 시뮬레이터 | https://fp.2hayoung.com/ |

## 구성

- `index.html`: 페이지 구조, 8개 웹앱 링크, SVG 아이콘
- `styles.css`: 맑은 고딕 우선, 흑백 디자인, 호버 및 모바일 반응형
- `favicon.svg`: 포탈 파비콘
- `index.html` 내부의 짧은 JavaScript: 마우스가 지나간 마지막 항목만 연한 회색으로 표시

마우스가 올라간 항목은 검은색 배경/흰 글씨, 방금 떠난 항목은 연한 회색 배경/검은 글씨, 그 이전 항목은 흰 배경으로 표시합니다. 모바일 터치에서는 잔상을 남기지 않습니다.

외부 프레임워크, CDN, 빌드 도구 및 데이터베이스를 사용하지 않습니다.

## 실행 및 배포

`index.html` 파일을 브라우저에서 열면 바로 확인할 수 있습니다.

Vercel에서는 이 저장소를 연결하고 **Framework Preset: Other**로 배포하면 됩니다. 별도 Build Command는 필요하지 않으며, Output Directory는 기본 루트 디렉터리를 사용합니다.

## 웹앱 추가 또는 수정

`index.html`의 `<ul class="app-list">`에 있는 `<li class="app-item">` 항목을 복사한 뒤, 웹앱 이름 및 `href` 값을 수정합니다. 기존 `icon-...` 기호를 재사용할 수 있습니다. 모든 링크는 새 탭으로 열립니다.

## 접근성 및 주의사항

- 키보드 Tab 이동과 포커스 표시, 동작 줄이기 설정을 지원합니다.
- CSS는 **맑은 고딕(Malgun Gothic)**을 우선 사용합니다. 해당 글꼴이 없는 기기에서는 시스템 대체 글꼴이 사용됩니다.
- 저장소가 공개 상태라면 이 웹앱들의 URL도 공개됩니다. 포탈 자체에는 인증이 없으므로, 기밀 업무 시스템의 접근 통제는 각각의 웹앱에서 유지해야 합니다.
