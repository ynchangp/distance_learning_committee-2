# 📚 Distance Learning Committee App v2

KDI 대학원 원격수업운영위원회 준비를 위한 맞춤형 웹 애플리케이션입니다.  
교원 이메일 검색 기능과 Course Modality DB 관리 기능을 통해 효율적인 위원회 운영을 지원합니다.

---

## 🚀 주요 기능

### 1. Faculty Email Finder
- 교원 리스트 엑셀 업로드 → 이메일 자동 매칭 → 결과 엑셀 다운로드
- 개별 교원 이름 검색 시 이메일 주소 확인 가능
- 교원 DB 구조: `순번, 국문명, 영문명, 구분, 이메일주소`

### 2. Course Modality DB
- 엑셀 업로드 및 전체 정보 다운로드
- 개별 정보 입력, 수정, 검색 기능
- 검색 기준: `Name`, `Course format`, `Year Semester`
- 출력 시 국문명 옆에 영문명 자동 매칭
- `None` 값은 그대로 유지
- `Reason for Applying`은 영어 번역 결과도 함께 제공

---

## 🛠️ 설치 방법

```bash
# 1. 프로젝트 클론
git clone https://github.com/your-username/distance_learning_committee-2.git
cd distance_learning_committee-2

# 2. 가상환경 생성 및 활성화
python -m venv venv
source venv/bin/activate  # Windows는 venv\Scripts\activate

# 3. 패키지 설치
pip install -r requirements.txt

# 4. 앱 실행 (FastAPI 예시)
uvicorn app.main:app --reload

