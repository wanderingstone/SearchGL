---
layout: default
title: Part 1 정부·민간기관
nav_order: 1
---

[검색방법설명(PDF) 다운로드]({{ site.baseurl }}/assets/source.pdf)  
[LLM 프롬프트 참고 업로드용 파일(TXT) 다운로드]({{ site.baseurl }}/downloads/guide_part1.txt)  

---
## **한국 보건의료정책 Gray Literature 검색 방법 - Part1. 정부/민간기관**
<div style="text-align:right;">2026.02.18 기준</div>

### **배경**
- 첫째, 한국 보건의료정책 관련 자료 중 Gray Literature는 체계적으로 정리되어 있지 않아 검색이 어려움
  - Peer review된 논문의 경우도 Pubmed에 등재(Pubmed에 등재되는 한국/외국 저널에 실리는 경우)되지 않으면 마찬가지 상황이며 이에 대해서는 따로 정리 예정
  - Gray Literature(회색 문헌) : 학술지나 상업 출판물을 통해 정식 배포되지 않고 비공식 채널로 유통되는 연구·정책 자료. 주로 정부 보고서, 토론회 자료집, 백서, 컨퍼런스 프로시딩, 정책 브리핑 등을 포함
- 둘째, 다양한 LLM과 Search Engine(Google 등)에서 검색이 가능하나, 소위 'LLM이 못 보는 자료'(검색되기 좋은 페이지만 검색하여 결과를 제시하는 편향)가 존재하며 잘 알고 있는 분야를 질의했을 때 검토 Source가 한정된다는 것을 경험할 수 있음
  - 특히 웹페이지 구조가 복잡하고 자료 다운로드와 검색에 로그인(SSO)·권한검증·세션쿠키·토큰만료·캡차·Referer 검사 등이 적용되는 경우 구체적으로 검색방법을 지정하지 않으면 포함하지 않게 됨
- 셋째, 안정적인 아카이빙, 레포지토리가 충분하지 않아 통합적으로 검색할 수 있는 웹페이지가 부족함
  - Part1에서는 기관 중심으로 제시하고, Part2는 DB검색(국립중앙도서관, 국회도서관, 사이언스온, 프리즘 등)을 정리할 예정

### **정리 기준 설명**
- 정부 기관, 민간 기관/단체 중 보건의료정책 관련 자료가 있는 웹페이지를 정리
	- 포함 기준은 작성자의 주관적 판단이며 가능한 넓게 정했으나, 최근 활동이 전혀 없는 웹페이지는 제외
- RSS 가능 여부
	- RSS는 피드(feed) 구독을 통해 신규 게시물을 리더가 주기적으로 수집·집계해주는 자동 모니터링 방식으로 개별 사이트를 순회하지 않고도 업데이트를 한곳에서 받아보는 구독형 정보 수신 방식임
	- RSS가능이라고 표시한 곳은 새로운 연구보고서, 보도자료 등이 올라오면 리더기로 바로 볼 수 있으므로 검색하지 않아도 정보를 얻을 수 있음
	- RSS가 가능하려면 웹페이지가 그에 맞게 만들어져야 하고, 불가능한 웹페이지에서도 RSS feed를 생성하는 서비스가 있기는 하나 유료이고 100% 성공하지는 않음
- 주 자료 메뉴는 Gray literature가 주로 있는 메뉴를 정리했으며, 따로 메뉴 여러 곳에 있거나 웹페이지 전체적으로 자료가 있는 곳은 적지 않음
- 추천 메뉴는 주 자료 메뉴 외에 다양한 자료가 있는 곳으로 특히 정부기관의 경우 사업별 페이지가 따로 있음
- 알리오에 있음이라는 표시는 공공기관 경영정보 공개시스템(https://www.alio.go.kr/)에 자료가 있는 기관으로, 기관별 공시에서 맨 아래부분에 보고서가 공개되어 있음
	- 대부분 웹페이지에 공개되는 것과 동일하나, 알리오에만 있는 경우도 있음
- 웹페이지가 개편되면 방법은 달라짐(2026.2 기준임)

### **검색 방법**
- 1순위. 직접 웹페이지에서 검색
	- 여러가지 한계로 일괄 검색에 의한 결과가 일정하지 않아 가장 정확한 것은 각 웹페이지에서 직접 검색임
- 2순위. 구글링
	- Google의 검색식을 활용하여 검색
	- 자세한 방법은 공식 Help 문서 [더 정확한 Google 검색 결과 얻기] 확인, [고급 검색](https://www.google.com/advanced_search)에서 옵션 선택해서 검색 가능(https://support.google.com/websearch/answer/2466433?hl=ko#)
	- site 지정, AND/OR/-/따옴표 등 이용, 파일Type 이용 권고
	- 다만 구글링도 재현 가능성(같은 검색식으로 검색했을 때 동일한 결과가 나오는 것)은 떨어지나 자세히 설정하면 개선 가능
- 3순위. LLM
	- LLM 종류에 따라 차이가 (매우) 커서, 정확한 자료를 모두 찾는 목적이라기보다는 관련 내용 검색 시에 이 웹페이지를 빼지 말고 찾는 것을 목적으로 함
	- 기관/단체 웹페이지 성격을 고려하여 LLM 프롬프트를 저장해놓고 쓸 수 있음
	- Deep research를 할 때도 이 프롬프트를 추가하면 빠지지 않고 검색 가능
	- 각 웹페이지에 대한 설명을 담은 [파일]({{ site.baseurl }}/downloads/guide_part1.txt)을 업로드하고, 참고하여 답변하라고 요청
	- 필요에 따라 기관/단체를 선택하기 
	- 중요 규칙
		- 절대 링크를 추측/생성하지 말 것
		- “검색 결과 화면에 실제로 존재하는 URL” 또는 “직접 열어 확인된 URL”만 출력할 것
		- 확인 불가하면 빈 칸으로 두고 ‘확인 불가’ 표기할 것


### **기관/단체별 웹페이지 설명**
**A. 정부 기관**
- 보건복지부
	- [https://www.mohw.go.kr/](https://www.mohw.go.kr/)
	- RSS가능
	- 주 자료 메뉴 : 정보 -> 연구조사발간자료
	- 추천 메뉴 : [보건복지부자료실](https://library.mohw.go.kr/), 사업별 페이지(통합돌봄 등)
- 질병관리청
	- [https://www.kdca.go.kr/](https://www.kdca.go.kr/)
	- RSS가능
	- 주 자료 메뉴 : 연구보고서는 국립보건연구원으로 연결
	- 추천 메뉴 : 사업별 페이지(감염병포털, 국건영, 지보계, 만성질환건강통계, 예방접종도우미 등)
- 식품의약품안전처
	- [https://www.mfds.go.kr/](https://www.mfds.go.kr/)
	- RSS가능
	- 주 자료 메뉴 : 법령자료 --> 자료실
	- 추천 메뉴 : 관련 누리집 모음
- 한국보건사회연구원
	- [https://www.kihasa.re.kr](https://www.kihasa.re.kr)
	- RSS가능
	- 알리오에 있음
	- 주 자료 메뉴 : 발간자료(보고서, 정기간행물)
	- 추천 메뉴 : [보건복지데이터포털](https://www.kihasa.re.kr/dataportal/main.html)
	- [연구성과물아카이브](https://repository.kihasa.re.kr/)
- 한국건강증진개발원
	- [https://www.khealth.or.kr](https://www.khealth.or.kr)
	- 알리오에 있음
	- 주 자료 메뉴 : 자료실
	- 추천 메뉴 : 유튜브 토론회/공청회 등
- 국민건강보험공단
	- [https://www.nhis.or.kr/](https://www.nhis.or.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 정책제도 --> 연구통계
	- 추천 메뉴 : 분야별 업무 사이트(건강보험빅데이터플랫폼, 비급여 정보 포탈)
- 건강보험심사평가원
	- [https://www.hira.or.kr/](https://www.hira.or.kr/)
	- RSS가능
	- 알리오에 있음
	- 주 자료 메뉴 : 의료정보 --> 연구통계
	- 추천 메뉴 : 주요연계업무사이트(보건의료빅데이터개방시스템, 병원평가통합포털, [HIRA OAK 리포지터리](https://repository.hira.or.kr/)), 조회/신청 -> 비급여진료비용 정보
- 한국보건의료연구원(NECA)
	- [https://www.neca.re.kr/](https://www.neca.re.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 연구정보
	- 추천 메뉴 : 내부관련사이트(환자중심 의료기술 최적화 연구사업)
- 국립중앙의료원 공공보건의료본부
	- [https://www.ppm.or.kr/](https://www.ppm.or.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 각 센터 자료실
	- 추천 메뉴 : 헬스맵
- 국립암센터
	- [https://www.ncc.re.kr/](https://www.ncc.re.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 따로 없음
	- 추천 메뉴 : 국가암지식정보센터
- 한국보건의료정보원
	- [https://www.k-his.or.kr/](https://www.k-his.or.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 알림마당->자료실
	- 추천 메뉴 : 알림마당 -> 포럼/세미나 자료
- 한국보건산업진흥원
	- [https://www.khidi.or.kr/](https://www.khidi.or.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 동향과정보(게시판별로 따로)
	- 추천 메뉴 : 매트릭스 서비스
- 한국보건복지인재원
	- [https://www.kohi.or.kr/](https://www.kohi.or.kr/)
	- 알리오에 있음
	- 주 자료 메뉴 : 소통마당 --> KOHI자료실
	- 추천 메뉴 : 유튜브
- 국립재활원
	- [https://www.nrc.go.kr/](https://www.nrc.go.kr/)
	- 주 자료 메뉴 : 자료실
	- 추천 메뉴 : 중앙장애인보건의료센터
- 국립정신건강센터
	- [https://www.ncmh.go.kr/](https://www.ncmh.go.kr/)
	- 주 자료 메뉴 : 자료실
	- 추천 메뉴 : 정신건강연구소, 정신건강사업부

**B. 민간 기관, 단체 등**

 - 대한의사협회 의료정책연구원(RIHP)
	- [https://rihp.re.kr/](https://rihp.re.kr/)
	- 주 자료 메뉴 : 연구자료
- 대한치과의사협회 치과의료정책연구원
	- [http://www.hpikda.or.kr/](http://www.hpikda.or.kr/)
	- 주 자료 메뉴 : 자료실, 발간자료
- 대한민국의학한림원
	- [https://www.namok.or.kr/](https://www.namok.or.kr/)
	- 주 자료 메뉴 : 자료실
- 한국의학바이오기자협회
	- [https://kamj.org/](https://kamj.org/)
	- 주 자료 메뉴 : 협회소식 --> 자료실
- 연구공동체 건강과대안
	- [http://www.chsc.or.kr/](http://www.chsc.or.kr/)
	- RSS가능
- 건강권 실현을 위한 보건의료단체연합
	- [https://kfhr.org/](https://kfhr.org/)
	- RSS가능
- 의료 민영화 저지와 무상의료 실현을 위한 운동본부(무상의료운동본부)
	- [https://medical.jinbo.net/xe/](https://medical.jinbo.net/xe/)
	- RSS가능
- 좋은공공병원만들기운동본부
	- [https://peoples-hospital.campaignus.me/](https://peoples-hospital.campaignus.me/)
- 건강세상네트워크
	- [https://konkang2020.tistory.com/](https://konkang2020.tistory.com/)
	- RSS가능
- 인도주의실천의사협의회
	- [https://www.humanmed.org/](https://www.humanmed.org/)
- 건강사회를 위한 치과의사회
	- [https://gunchi.org/](https://gunchi.org/)
- 노동건강연대
	- [https://laborhealth.or.kr/](https://laborhealth.or.kr/)
	- RSS가능
- 전국보건의료산업노동조합(보건의료노조)
	- [https://bogun.nodong.org](https://bogun.nodong.org)
	- RSS가능
- 시민건강연구소
	- [https://health.re.kr/](https://health.re.kr/)
	- RSS가능
- 한국환자단체연합회
	- [http://www.koreapatient.com](http://www.koreapatient.com)
- 돌봄과 미래
	- [https://dolbom-mirae.imweb.me](https://dolbom-mirae.imweb.me)
- 사회건강연구소
	- [https://www.ishealth.org/](https://www.ishealth.org/)
- 참여연대 사회복지위원회
	- [https://www.peoplepower21.org/category/welfare](https://www.peoplepower21.org/category/welfare)
- 전국의료산업노동조합연맹(의료노련)
	- [https://fkmtu.net/](https://fkmtu.net/)
- 내가만드는복지국가
	- [https://mywelfarestate.kr/](https://mywelfarestate.kr/)
- 전국전공의노동조합
	- [https://www.kirulabor.org](https://www.kirulabor.org)
- 대한의학회
	- [https://www.kams.or.kr](https://www.kams.or.kr)

## 원문 PDF 미리보기
<iframe class="pdf-frame" src="{{ site.baseurl }}/assets/source.pdf"></iframe>