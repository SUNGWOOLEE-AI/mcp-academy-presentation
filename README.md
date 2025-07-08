# 🎓 학원 원장을 위한 MCP 실습 프레젠테이션

**Claude + MCP 활용 완전 정복: 초보자를 위한 실습 가이드**

## 📖 개요

이 프레젠테이션은 학원 원장님들을 대상으로 한 60분 MCP(Model Context Protocol) 실습 강의용 자료입니다.

### 🎯 강의 목표
- MCP의 개념과 작동 원리 이해
- Claude Desktop에서 MCP 서버 설정 및 활용
- 학원 업무 자동화를 위한 실무 적용 방법
- 카카오톡 자동 발송 및 학교 일정 수집 실습

## 📊 프레젠테이션 구성 (8슬라이드)

### Part 1: MCP 이해하기 (2슬라이드)
1. **🚀 MCP란 무엇인가?**
   - MCP의 개념 (AI의 USB-C 포트)
   - 학원 운영에서의 변화
   - 기본 작동 원리

2. **✨ Claude MCP의 특징**
   - 기존 방식 vs MCP 활용 비교
   - 핵심 장점 4가지
   - 실무 적용 효과

### Part 2: 설정 및 구성 (2슬라이드)
3. **⚙️ MCP 설정하기**
   - 3단계 설정 과정 (현대적 인포그래픽)
   - 파일 찾기 → 코드 입력 → 재시작
   - 성공 확인 방법

4. **🎯 학원 업무별 MCP 서버**
   - 파일 시스템 연결 (성적표, 출석부)
   - 웹 스크래핑 (학교 일정 수집)
   - 완벽 설정 JSON 코드

### Part 3: 실무 활용 (4슬라이드)
5. **💬 카카오톡 자동 발송 MCP**
   - 주요 기능 (개별/일괄 전송)
   - 활용 시나리오 (공지, 상담 등)
   - 실제 사용 예시

6. **🔧 카카오톡 MCP 기술 구조**
   - 이미지 인식 기반 UI 자동화
   - 구글시트 연동 시스템
   - MCP 서버 인터페이스
   - 설치 요구사항

7. **🏫 Playwright 학사일정 수집**
   - 웹 브라우저 자동화 개념
   - 기존 방식과의 차이점
   - 수집 가능한 정보 유형

8. **💻 Playwright 실습하기**
   - 서버 설정 방법
   - 자연어 명령 사용법
   - 결과 활용 방안

## 🚀 사용 방법

### 온라인에서 바로 보기
**GitHub Pages**: [https://sungwoolee-ai.github.io/mcp-academy-presentation/](https://sungwoolee-ai.github.io/mcp-academy-presentation/)

### 로컬에서 실행
1. 저장소 복제:
   ```bash
   git clone https://github.com/SUNGWOOLEE-AI/mcp-academy-presentation.git
   ```

2. 브라우저에서 `index.html` 파일 열기

### 네비게이션
- **키보드**: 왼쪽/오른쪽 화살표 키
- **마우스**: 하단 이전/다음 버튼
- **현재 위치**: 우상단 슬라이드 번호 표시

## 🎨 디자인 특징

- **현대적 인포그래픽**: 3페이지 설정 과정을 시각적으로 표현
- **발표용 최적화**: 폰트 크기 30% 증가, 가독성 향상
- **학원 특화 내용**: 실제 학원 업무에 바로 적용 가능한 예시
- **인터랙티브**: 부드러운 슬라이드 전환 애니메이션

## 📝 포함된 실습 내용

### 1. 카카오톡 MCP 서버
- **위치**: `D:/Dev/ControlKakaoTak/kakao_mcp_server.py`
- **기능**: 개별/일괄 메시지 전송, 구글시트 연동
- **사용법**: "김선생님에게 메시지 보내줘" 자연어 명령

### 2. Playwright 웹 스크래핑
- **대상**: 불암중학교, 대진고등학교, 서라벌고등학교
- **수집 정보**: 2025년 시험 일정, 방학 기간, 학교 행사
- **활용**: 학원 특강 일정 계획 수립

### 3. 설정 파일 예시
```json
{
  "mcpServers": {
    "sequential-thinking": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-sequential-thinking"]
    },
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "C:/학원자료"]
    },
    "playwright": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-playwright"]
    },
    "kakao-sender": {
      "command": "python",
      "args": ["D:/Dev/ControlKakaoTak/kakao_mcp_server.py"]
    }
  }
}
```

## 🎯 활용 방안

### 강의 진행
- **총 소요시간**: 60분
- **구성**: 이론 15분 + 실습 45분
- **방식**: 각 슬라이드 5-10분씩 설명 + 실시간 시연

### 실습 준비물
- Claude Desktop 설치
- Node.js 설치
- 카카오톡 PC 버전
- 텍스트 에디터 (VS Code 권장)

## 📞 문의 및 지원

- **Issues**: [GitHub Issues](https://github.com/SUNGWOOLEE-AI/mcp-academy-presentation/issues)
- **개선 제안**: Pull Request 환영
- **강의 문의**: 이슈를 통해 연락주세요

## 📄 라이선스

MIT License - 자유롭게 사용, 수정, 배포 가능합니다.

---

**제작**: Claude + Human Collaboration  
**버전**: v1.0  
**최종 업데이트**: 2025.07.08  

🎓 **모든 학원 원장님들의 성공적인 MCP 도입을 응원합니다!**