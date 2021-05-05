# 김민균 MinKyun Kim RESUME

:telephone_receiver: 010-2334-9654

:email: mkzzang0928@gmail.com

:ledger: https://blog.nvaer.com/mkzzang0928

:computer: https://github.com/mkkim90

</br>

## ABOUT ME

안녕하세요. Java & Spring 기반의 6년차 백엔드 개발자로,  **금융 가입설계/청약과 제휴 마케팅 서비스 분야에서 API/Batch를 주로 개발해왔습니다.**</br>
레거시 코드를 분석하여 점진적으로 리팩토링하는 것을 좋아하며, 코드 리뷰와 단위테스트를 통해 실수를 예방하고 안정적인 완성도를 높이는 것을 중요시합니다.</br>
재사용성 및 유지보수용이한 코드를 지향하며, 좋은 코드에 대한 고민을 많이 하는 편입니다.    

### 다양한 프로젝트 개발 경험을 통해 노하우 

- **Security 코딩과 개인정보 암호화 처리 준수**
    * 보안취약점진단 및 금융감독원 감사 및 권고사항에 대한 조치 경험

- **제휴사 솔루션 모듈 및 오픈소스 라이브리러리 연동 및 시스템 내재화**  
    * NICE결제, KCB신용인증, KaKaoPay인증, SSO로그인, RSA-OTP 로그인, 보안키패드, 전자문서, MDM, 콜장비 등 모듈 및 오픈소스 라이브러리 연동 경험

- **레거시 코드 분석 및 리팩토링**  
    * PHP model1 방식 → PHP CodeIgniter MVC, Java PlayFramework1.0 REST API → Java SpringFramework4.0 REST API</br>
      JSP Model1방식 → Java Spring MVC 컨버팅 작업 및 차세대 프로젝트 개발 경험
  
주도적으로 문제를 해결 및 자체 개선해왔으며, 솔선수범하고 긍정적인 자세로 임하고 있습니다.</br> 
사람이 우선인 공간 속에서 함께 성장하고 서로 머리를 맞대어 성과를 이뤄낼 수 있는 좋은 개발자가 되기위해 항상 최선을 다하겠습니다.  


## SKILL

### Languages
- **Java8**, JavaScript, PHP

### Frameworks / Libraries
- **Spring4**, AngularJS1.7, JQuery, BootStrap

### Databases / ORM 
- Oracle11g, MySQL, MyBatis, JPA

### Etc
- Git, Subversion, Jenkins, Jira, Confluence


## Experience & Project

### KB생명보험(2019.1~2020.12)
```
- 회사소개 : KB금융그룹 계열사 종신, 변액, 연금 생명보험 금융 서비스
- 주 업무 : 청약 및 가입설계 프로세스 기반의 B2B 영업지원시스템 스마트 스타드림 개발/운영
```
### 프로젝트 
#### 변액 적합성 진단 프로세스 고도화(2020.3~2020.5)
```
금융감독원의 권고사항 지침에 따라 모바일 변액보험 상품 판매를 위한 변액보험 적합성 진단 프로세스를 강화하는 것이 주목적입니다.
변액보험 적합성 진단은 고객의 정보 및 보험 성향 분석을 통하여 고객에게 알맞은 맞춤 상담을 실시하고, 적합한 상품의 권유를 위한 절차입니다.
이를 모바일 서비스에 적용하기 위해 맞춤형 가입설계 프로세스 변경 및 청약 서류를 추가 작업하였습니다. 주로 API 개발을 담당하였습니다.
```
- **변액 적합성 진단 API 개발**
   * 모바일 화면과 모바일 전자 문서에 변액보험 진단 결과를 노출하며, 고객의 진단 결과에 따라 유형별 전자 문서를 생성하고 입력 항목을 노출하기 위함
   * Java Tmax library를 통해 변액보험 적합성 진단 설문 정보 데이터를 XML 데이터로 변환하여 기간계 서버에 등록 요청 API 개발
   * Java Tmax library를 통해 변액보험 적합성 진단 결과 XML 데이터를 문자열로 변환하여 진단 결과 유형 코드를 Oracle DB에 적재
   * MyBatis를 이용해 변액보험 적합성 진단 DB 질의를 조회하여 결과를 응답하는 JSON 포맷의 REST API 개발
   * 적합성 진단 전자 문서의 입력 항목을 EnumaEnum 클래스로 관리하며 전자문서의 규격 XML 포맷의 REST API 개발 

- **Tech** : Java1.7, Spring3.5, Oracle, MyBatis, Junit4

***

#### NICE 인증 모듈 → KCB 신용정보 인증 모듈 개편(2019.11~2020.1)
```
PC, Tablet, MOBILE 영업지원시스템의 NICE 인증 모듈에서 KCB 신용정보 인증 모듈로 전면 개편하는 것이 주목적입니다.
NICE 인증 모듈의 영향도를 분석하고 개발 범위를 산정하며, 기존 프로세스를 유지한 상황에서 KCB 신용정보 인증 모듈을 연동한 새로운 API를 설계 및 구축하였습니다.
안정적인 완성도를 높이고자 충분한 단위테스트를 진행하였으며, PC/Tablet/MOBILE 영업지원시스템을 순차적으로 릴리즈하는 방식으로 개편하여, 경과를 모니터링했습니다.
최종적으로 전면 개편이 완료되는 시점에 NICE 인증 모듈을 제거하였습니다. 
```

- **인증 요청 & 결과 응답 API 개발**
   * 고객정보 동의 및 고객 확인 절차에 필요한 인증을 하기 위함
   * PC/Tablet/Mobile 환경별 JSON, XML, 구간 암호화 포맷으로 구성
   * PC/Tablet/Mobile 환경별 보안키패드 복호화 및 인증 모듈 요청을 위한 입력 데이터 처리
   * 신용카드사 코드 및 인증 결과코드 Enum Class로 관리
   * License Key 암호화하여 서버별 properties 파일 관리
   * KCB 신용정보 인증 모듈 객체를 조합(Composition)한 싱글톤 패턴의 Util 클래스로 인증 요청/결과 응답처리 및 인증 이력 DB 적재
   
- **Tech** : Java1.7, Spring3.5, Oracle, MyBatis, Junit4

***

#### 디지털 채널계 고도화(2019.7~2019.10)
```
기존 복잡한 청약 단계를 간소화하여 사용자 입장에서 편의성과 효율성을 제공하는 것이 주목적입니다. 
기획 요구사항에 맞춰, 가입설계 및 청약에 최적화된 화면으로 재구성합니다. 불필요한 기능 제거와 여러 번 중복되는 데이터를 효율적으로 사용할 수 있는 방안을 모색하며, 화면에 필요한 API를 설계 및 구축하였습니다.
```

- **전자 문서 환경의 모바일 서명, 보험상품 관련 정보 API 개발**
   * 청약에 필요한 전자문서들에 서명과 보험 상품 관련 가입설계된 정보를 자동으로 주입해주기 위함
   * Reporting 플랫폼을 활용하여 전자문서에 데이터 바인딩할 위치 좌표 천공 작업
   * 사용자 서명 좌표 데이터,  가입 보험 상품 관련 전자문서에 필요한 정보를 Java Reporting Library를 이용하여 전자문서와 호환되는 XML로 변환하고 DB암호화하여 저장
   * 종신/변액/연금 등 보험 상품별 처리되는 청약 서류가 다르므로, Factory패턴을 활용하여 문서서류코드별 객체를 생성
   * 각 정보 항목은 Enum 클래스로 관리하여 전자문서와 호환되는 XML기반의 데이터로 가공하는 API 개발

- **전자서명에 대한 x,y좌표 데이터를 경량화(50~60% 용량 크기 감소)**
   * 서명을 그리는 화면에서 좌표를 랜더링 속도를 개선하고 좌표 저장 용량을 감축하기 위함
   * jQuery Canvas 라이브러리의  위치 x,y 좌표를 소수자리 2자리 반올림
   * 성명과 서명의 영역 좌표 산출 계산 알고리즘을 분석하여 중복 계산식은 괄호처리 및 불필요 계산식은 제거

- **SPA기반 Application 비동기 처리**
   * 불필요한 화면 넘김을 통한 로딩을 최소화하기 위함
   * AngularJS의 $https와 Spring REST API 개발을 통해 비동기 방식 API를 호출하고 JSON데이터를 바인딩처리

- **가입설계 청약단계에서 에러 로그 적재 및 청약 경과 모니터링 화면 개발**
   * 기간계/전자문서플랫폼 영역/IOS&Android영역/이미지시스템영역 등 다양한 연계된 시스템의 간헐적인 오류 포인트를 확인하고 빠른 대응하기 위함
   * Spring Exception Handler를 이용하여 공통 모듈로 에러 메시지의 필요한 항목 Parsing 및 Oracle DB적재
   * MyBatis를 이용하여 DB 쿼리 작성 및  화면 조회에 필요한 데이터 Spring REST API 개발
   * AngularJS를 이용하여 보험 설계사 청약 경과 조회 화면 개발

- **Tech** : Java1.7, Spring3.5, MyBatis, Oracle, AngularJS, Jeus8, WebToBe

- **향후 개선 방안**
   * 문서 각 항목 코드를 Enum클래스를 DB로 전환함으로써, 해당 코드 추가 수정 작업을 자동화 방안
   * 전자문서 기반의 XML 기반의 암호화 데이터 관리를 Oracle에서 NoSQL Redis로 전환
      * 가입설계 정보를 특정 기간 내에 자동 삭제 가능하며, 가입설계 ID 기준의 전자문서 병합을 위한 동적인 XML 컬럼 형태이므로 key/value 기반이 오히려 적합
   * 데이터를 비동기 방식으로 속도를 개선할지라도, 동시성 이슈를 고려하여 데이터가 임계영역인지 판단하고 경우에 따라서 동기화로 처리

***

#### 차세대 디지털 채널계 안정화(2019.1~2019.4)
```
디지털 채널계 시스템 (어드민/대고객/SFA/온라인보험)의 차세대 SI 프로젝트 도급 과정에서 프로덕션을 일부 완수하지 못하였습니다.
오픈이 지연되는 상황이었으므로, 개발 지원을 통해  안정적으로 오픈하는 것이 주목적이었습니다.
어드민/모바일 영업지원시스템의 누락 기능을 인수·인계받아서 코드를 분석하고 요구사항에 맞춰 주로 개발하였습니다.
```

- **어드민 시스템 AS-IS 어드민 모델 1 방식의 JSP 레서시 코드를 분석하여 Spring MVC 기반의 전자정부 프레임워크 & MyBatis로 컨버팅**
 * 기존 로그인 로직인 비밀번호 정책 및 1차 로그인인 SSO 통합 인증 서버 연동과 2차 로그인인 RSA Token 기반의 OTP 서버  Java IO를 활용하여 연동 개발
 * 고객 상담 QNA / 지급 / 상품 등록 등 10여 페이지 Jsp 및 Bootstrap 개발

- **모바일 영업지원시스템 스마트 스타드림 SPA 기반의 하이브리드 웹앱 화면 개발 및 API 개발**
 * AngularJS & Apache Cordova 플러그인 라이브러리의 PDF / MDM / 연락처 가져오기 / 보안키패드 연동 개발 및 IOS / Android 협업
 * java File 라이브러리와 HTTP Context-type 변환하여 PC/모바일 약관 보기/다운로드 API 개발
 * MyBatis를 이용하여 가입설계 고객 DB 데이터를 조회하고 java 기반의 SMS&Email 전송 모듈을 통해 모바일 약관 전송 API 개발
 * AngularJS를 이용하여 가입설계 특약/고객 인증/전자문서 화면 분석 및 누락 기능 개발

- **Tech** : java1.7, 전자정부 프레임워크 3.5, MyBatis, AngularJS, Apache Cordova

***

### SK M&Service(2017.4~2018.11)
```
- 회사 소개 : SK ICT 그룹 계열사로 오케이캐쉬백, T쿠폰, 마케팅 Sales, 복지몰 커머스B2B 서비스
- 주 업무 : SKT 1000여만 마켓팅 동의 고객 DB를 기반으로 제휴 보험 텔레마켓팅 B2B 서비스 ‘보험TAS’ 개발 및 운영 
```

### 프로젝트
#### 차세대 보험TAS(2018.1~2018.11)
```
보험TAS는 제휴 보험 텔레마켓팅 B2B서비스로 폐쇄망 환경의 20여개의 센터지점에서 운용되고 있습니다.
전체 센터 지점을 차세대 보험 TAS로  전면 개편하는 것이 주목적입니다.   
제휴 콜장비 업체와 보험사간 상호 교환하는 데이터 API와 Batch를 주로 개발하였습니다. 
```

- **보험사 고객 정보 및 콜장비 연동 서비스 API 개발**
   * 구 보험 TAS를 개편함에 따라 신규 보험 TAS로 청약정보를 상호 교환하기 위함
   * 제휴 보험사와 콜장비 업체와 협의하여 ActiveX를 활용한 Socket 통신 및 Java Spring Rest API를 설계 및 구축

- **보험사 청약 데이터 및 콜장비 녹취 데이터 Batch 개발**
   * 금융감독원 감사 조치에 따른 완전판매를 위한 QA 녹취 파일 수집 및 고객 배정을 위한 청약 데이터 수집
   * DMZ 영역의 NAS 특정 경로에 각 보험사별 청약 데이터 파일 및 녹취 파일을 수집
   * 수집된 데이터 Java Quartz 및 Linux crontab Deamon shell 스케줄링 배치 개발 및 수집 데이터 결과값을 활용해 DB 적재하여 배치 경과 화면   

- **지인/파생 프로세스 개발**
   * 보험 설계사간 지인/파생 고객을 등록하여 보험 설계 고객 확보하기 위함 
   * 지인/파생 관련 승인 & 인증, 고객, 캠페인, SKT 마켓팅동의고객 DB 설계
   * 지인/파생 고객 DB 인증 기간내 삭제 처리 및 SKT 마켓팅 동의 고객 1000만 데이터 익일 등록 처리 Batch 개발

- **SK 인포섹 보안 취약점 진단 및 완전판매 관련 금융감독원 감사 조치**
   * CSRF 대응 방안으로 Spring Interceptor를 통해 로그인체크 및 Token 검증 및 로그인시 세션에 랜덤 Token 추가
   * SQL Injection 및 XSS 대응 방안으로 Spring Filter를 활용하여 우회코드로 대체
   * 청약 데이터와 녹취파일 암호화 개인정보 NAS 보관 및 crontab을 이용하여 특정 기간 일자에 삭제 처리
   * 개인정보 일부 마스킹 처리 및 프로세스상 마스킹 처리 불가한 항목은 개인정보 활용 사용자 추적 로그 DB 적재
   * SQL Injection 대응방안으로 동적쿼리 지양
   * http 프로토콜 https 전환
   * IDC 및 사설 VPN 폐쇄망 환경에서의 콜 센터 지점 운영을 위한 인프라 구축 협업
   * QA평가를 위한 QMS품질관리시스템 구축 관련 외주 관리 

- **DB성능 튜닝**
   * 센터 지점 오픈시, 안정화를 위한 Scouter APM 상시 모니터링
   * Scouter XLog를 통해 8초 이상  슬로우쿼리 추출
   * Explain Plan와 쿼리분석을 통해 컬럼 경량화 및 서브쿼리를 JOIN 쿼리로 전환(8~15초-> 2초 내외)

- **고객만족을 위한 20여개의 센터에서 QnA간담회/설문조사/가이드 등 사용자 피드백을 통해 UI/UX 편의성 기능 개선** 

- **트러블 슈팅 및 개선**

   1. **DB & 네트워크 병목 구간 발생에 따른 Scale-out과 Scale up**
   
      - 문제
         * 신규 서비스로 센터 지점에 오픈하는 당시, 사용자가 많은 특정 지점에서 콜 장비 API 데이터 수신이 원활히 이루어지지 않는 현상이 간헐적으로 발생하였습니다.   
      - 원인
         * 사용자가 많은 특정 지점에서 VPN 네트워크 대역폭간 패킷 유실 발생
         * Scouter APM 모니터링 당시, 12초 슬로우쿼리를 빈번하게 호출
      - 해결
         * Scale-out : 당시 병목구간을 찾기 위해서 Scouter APM 및 DB 용량 모니터링 결과 정상적인 수치로 판단이 되었고, 네트워크 병목 구간 이슈로 판단하였으며, VPN 네트워크 대역폭 증설
         * Scale-up : 고객 조회의 빈번하게 발생하는 슬로우쿼리의 느려진 컬럼을 찾았고 불필요 판단하여 컬럼과 컬럼을 추출하기 위한 서브쿼리를 제거
         * API 데이터 정상적 수신
      - 향후 방안 / 배운점
         * Client/OS/DB/네트워크 등 병목 구간 발생 소지를 인지하며 상시 모니터링
         * 신규 시스템 오픈 시, 부하 테스트 시나리오 작성을 통해 사전 실수 예방
         * 주도적으로 코드 리팩토링 및 EXPLAIN Plain을 통해 DB 성능 튜닝 등을 통해 지속 개선
 
   2. **대용량 데이터 익일 Batch 성능 튜닝**
   
      - 문제
         * 지인/파생 프로세스 개발 당시, SKT마켓팅 동의를 검증하는 1000여만 데이터 파일을 DB로 저장하는 Java Batch가 3~4시간 소요
         * 데이터 파일을 읽어들이고 Java SQL 라이브러리를 활용하여 쿼리를 1000건씩 처리하는 것을 10000건씩 처리하도록 해봤으나, 서버단에서 Out Of Memory 발생
         * 그 외 수백건의 배치가 순차적으로 돌기때문에 어플리케이션 환경에서 리스크가 있다고 판단하여 다른 방법 모색
      - 해결
         * 대용량 파일 등록에 특화된 SQL Loader 활용(3~4시간 → 20분 단축)
      - 배운점
         * DB 프로시저는 문자열 조합 처리가 있다면 부적합
         * Java에서 많은 쿼리를 처리할 경우, Out Of Memory 발생 소지가 있기에, 적합한 수치 계산 필요
         * SQL Loader는 DirectPath를 통해 Buffer Cache를 타지 않고 바로 Block으로 등록 가능하나, DB Lock이 걸리므로 실시간 사용에는 부적합
         * 익일 갱신 데이터는 데이터 인덱스가 남을 것을 고려하여 Delete보다는 Truncate 하는 것이 메모리 용량 감소에 
         * 대용량 데이터 인덱스를 최소화

***

#### SK 이패밀리샵 임직원몰 기프티콘 고도화(2017.5~2017.8)
```
SK임직원 전용 복지몰 가전제품 e-커머스 서비스 ‘이패밀지샵’을  제휴사 KB/NICE/공공기관 전용 복지몰로 확대와 다양한 상품 확대를 위한 SKP 기프티콘 적용이 주목적입니다. 
프로젝트 팀원으로 개발 및 외주인력 매니징하였습니다.
```

- **SK플래닛 기프티콘 전문 통신 API 연동(SMS발송)**
   * 싱글톤 패턴 Util성 클래스를 생성하여  기프티콘 전문 통신 API를 Java IO URLConnection 호출
   * 상품 주문 결제 성공 시, 기프티콘 분류 코드를 통해 기존 가전제품 상품DB 및 주문 DB 처리와 별도 로직을 분리하여 기프티콘 다중/단일 SMS 발송 결과 값 기프티콘 발송 이력 DB로 관리
   * 어드민 기프티콘 이력 조회 MPA 기반의 어플리케이션 JSP & Java Spring MVC 어드민 기프티콘 이력 DB 조회 및 화면 개발 

- **제휴사별 광고 배너 및 약관 정보 자동화**
   * 제휴사별 도메인으로 if 조건문으로 하드코딩하여 광고 배너 및 약관 정보 추가 작업이 번거로움
   * 제휴사 정보와 제휴사별 상세 정보 DB 설계
   * MPA기반의 어플리케이션 JSP & Java Spring MVC 어드민 제휴사 도메인별 약관 / 광고 배너 DB CRUD 및 화면 개발

- **트러블 슈팅 및 개선**

   1. **선착순 이벤트 시스템 부하**

      - 상황
         * 제휴사 복지몰 확대를 통한 KB패밀리몰이 출시되었으며, 매일 선착순 이벤트를 하게되었습니다.
      - 문제
         * 특정 시간 기준점으로 트래픽이 몰리면서 시스템이 멈추는 현상이 발생
      - 원인 
         * 특정 시간에 접속자가 급격히 증가하여 발생한 이슈
      - 해결
         * 미들웨어&시스템 엔지니어와 협업을 통하여 SK서버 인프라 규격보다 Apache 동시접속자와 최대 스레드 및 Tomcat Connection DB pool과 Thread Pool 수를 증가 요청
         * Jmeter를 활용하여 부하테스트를 진행하면서 테스트시나리오 작성
         * Web 1대 및 WAS 2대 증설
         * 시스템 OutOfMemory 해결

   2. **동시성 이슈로 추가 결재**
   
      - 상황
         * 시스템 멈추는 현상은 발생하지 않았으나, 선착순 재고가 떨어졌음에도 추가적으로 결제되는 현상이 발생

      - 원인 
         * 상품 재고 수에 대한 동시성 이슈
         * 결제 성공/실패 전 후로 상품 재고 검증 프로세스 누락  

      - 해결
         * 상품DB low-lock 
         * 결제 성공/실패 전 후로 상품 재고 검증 프로세스 추가 

   3. **향후 개선 방안**
      - IDC기반의 VMWARE에서 AWS Cloud Autoscaling & Docker 기반의 환경으로 전환함으로써, Apache & Tomcat 환경 설정 및 서버 증설 작업 기간 및 인력 최소화
      - 선착순 이벤트를 Queue를 활용하여 선착순 마감 인원에 따른 결제 프로세스를 순차적으로 진행함으로써, 상품 DB lock으로 인한 DB부하 우려 감소
      - 상품 DB lock이 아닌 낙관적잠금 활용 UPDATE tb_product SET stock=stock-1 WHERE stock-1 >= 0 AND id =#{id}"
      - 주문/결제/상품재고 업무 도메인에 따라 임계구역을 명확히 구분하여 트랜잭션 처리 

***

### 소리바다(2015.7~2017.4)
```
- 회사 소개 : 누적 100여만 다운도드 국내 음원 B2C서비스
- 주 업무 : 플레이리스트/앨범 및 마케팅 콘텐츠 API 개발 
```

### 프로젝트
#### REST API 컨버팅(2015.10~2016.2)
```
기존 Java1.5 PlayFramework 1 의 레거시 시스템의 호환성 이슈로 인해 Java1.7 & Spring4.0으로 전면 개편하는 것이 주목적입니다.  
프로젝트 팀원으로 개발하였습니다. 
```

- **플레이리스트/앨범자켓 REST API 컨버팅**
   * IOS/Android/Mobile Web/PC Web 환경 및 버전별 API 데이터 영향력 조사를 통해 불필요한 데이터 제거
   * PlayFrameWork의 라우터 파일 분석하여 Spring @RestController와 @RequestMapping 방식의 어노테이션으로 변경
   * PlayFrameWork의 JSONObject로 변환 로직 제거하여 Spring Rest Librariy를 이용하여 ResultEntity 객체만 return
   * PlayFrameWork ORM을 MyBatis 쿼리방식으로 변환 
   * 캐시성 NoSQL Redis에 적재하며, 앨범/플레이리스트ID를 Key로 활용

- **Tech** : Java1.7, Spring4.0 REST, Redis, MySQL

*** 

#### 어드민 개편(2016.3~2016.5)
```
PHP Model1 방식 레서시 코드를 PHP CodeIgniter MVC 기반으로 개편하는 것이 주 목적입니다. 프로젝트 팀원으로 개발하였습니다.
````
- **PHP CodeIgniter MVC 컨버팅 작업**
   * PHP Model1 방식의 레서시 코드 분석
   * 30여개 어드민 페이지 화면을 PHP CodeIgniter code 가이드라인에 맞춰 CRUD 개발
   * UI 가이드라인에 맞춰 BootStrap CSS 태그 적용 및 jQuery Front-end 개발

- **Tech** : PHP, CodeIgniter, jQuery, BootStrap, CSS

*** 

#### 이미지 리사이징 구축(2016.09~2016.10)
```
일정 비율 규격 이미지 리사이징 모듈만 사용해야 하는 상황에서 현업 불편함을 해소하고자 자체 사내 이미지 리사이징 모듈을 개발하였습니다.  
다양한 비율과 높이/넓이로 이미지 리사이징 할 수 있는 플랫폼을 제공하는 것이 주목적입니다.
```
- **이미지 리사이징 API 개발**
   * 이미지URL 및 File DB 경로 를 확인하여  java File 및 ImageBuffer 입출력
   * 리사이징 오픈소스 라이브러리를 활용하여 포커스 위치 선정과 비율과 넓이/높이 등 다양한 기능 개발
   * 캐시성 NoSQL Redis에 적재하며, 앨범/플레이리스트ID와 입력값을 조합한 Key로 사용하여 Redis에 이미지 파일이 있을 경우 바로 조회 기능 개발

- **Tech** : Java1.7, Spring4.0, Redis, MySQL

***

#### Magazine 이벤트 자동화 프로세스(2016.05~2016.6)
```
회사 경영 악화로 구조조정이 있었으며, Front-end를 인수인계 받으면서 이벤트 페이지를 개발하게되었습니다. 
이벤트 페이지 퍼블리싱 및 API 개발을 자동화하는 것이 주목적입니다.     
```

- **Magazine이벤트 자동화 개발**
   * 이벤트 정보 및 상세 페이지 MySQL DB설계
   * PHP CodeIgniter기반의 이벤트 정보 및 상세 페이지 삭제/등록/조회 REST API 개발
   * BackBoneJS기반의 유형별 이벤트 View 모듈 개발
   * 유형별 이벤트를 등록할 수 있도록 PHP CodeIgniter&BootStrap&JQuery를 활용하여 개발 

- **Tech** : PHP, CodeIgniter, BackBoneJS, BootStrap, jQuery, MySQL, Redis


## 수상 & 외부 활동

### BSIDE 1기 (2019.12~2020.4)
```
기획자, 디자이너, 개발자 협업 사이드 프로젝트 모임
```
   - 30.1팀 Dspot - 모임 위치 찾아주는 서비스
   - Https://www.bside.best/bside1
   - React 하이브리드드웹앱, TMap 지도 API 연동, Firebase기반의 호스팅, NoSQL 구축 경험

### 16년 트렌드 X MEDICAL HACKATHON(2016.9~2016.10)
```
삼성서울병원, 성균관대학교, 서울창조경제 주체 디지털 헬스케어 해커톤
```

   - 마이하트팀 약물복용도우미-빅데이터 기반의 처방 스케줄링 서비스
   - 시상내역 : 최우수상(청년위원장상-장관급)
   - 헬스케어이노베이션 2016 포럼 발표 
   - https://biz.chosun.com/site/data/html_dir/2016/11/03/2016110301550.html 
   - 의료공공데이터, Google Vision 오픈 API 연동, AWS EC2, S3 구축,  Java Spring 전자정부프레임워크, AngularJS 기반 IONiC 하이브리드웹

### KOSTA 개발자 양성 실무 프로젝트(2015.5~2015,7)
```
한국소프트웨어기술진흥협회 주체 공모
```

   - 개인자원관리통합시스템
   - 시상내역 : 우수상(협회장상)
   - Java1.7 Spring, MySQL, BootStrap, JSP, jQuery 

### 14년 제9회 창업 아이템 경진대회(2014.9~2014.11)
```
백석대학교 교내 주체 공모
```
   - Quality팀 IOT기반의 휴대용 척추 측만증 측정기
   - 시상내역 : 최우수상(총장상)
   - 척추비틀림 자이로센서를 이용해 자세 교정 제안



## EDUCATION

### 우아한테크캠프 Pro 1기 과정(2020.11~2021.1)
```
Java백엔드 개발자로써, 실무 역량 강화 커리큘럼 3개월 과정
```

   - 테스트 주도 개발 및 리팩토링 역량 강화를 목적으로 참여
   - 미션 과제 코드 리뷰 및 피드백을 통한 개선
   - 클린코드 / TDD / ATDD / DDD / 리팩토링 학습

### 한국소프트웨어기술진흥협회(2015.1~2015.7)
```
Java프로그래밍과 OpenSource Framework 개발자 양성 6개월 과정
```

   - 자바 및 스프링프레임워크 역량 강화를 목적으로 참여
   - Java 객체지향 및 SpringFramework프로젝트 학습

### 백석대학교 컴퓨터공학부 학사 졸업(2009.3~2015.8)
    
   - ICT학생회 기획국장 및 소프트웨어전공장 역임
   - 15년 학부봉사상(학장상) 수여 및 우수성적장학금 8회, 수석 4.5 졸업



## License

   - SQLD (2019.9 / 한국데이터산업진흥원)
   - 정보처리기사(2015.5 / 한국산업인력공단)

