#### AWS 배포

1. 배포하기 위한 프로그램을 만든다.
2. 프로그램을 build 한다.    
2-1. 스프링부트의 경우 powershell로 gradlew가 있는 폴더로 경로를 잡고 ./gradlew build를 한다.   
     build/libs 폴더 안에 .jar 생성된다.  
2-2. 리액트의 경우 npm run build를 한다.(설정파일과 묶어서 압축, 압축시 zip으로 한다. 반디집x)  
3. ed 환경을 만든다 (AWS)
- Elastic Beanstalk : 플랫폼을 구성해주기 때문에 배포할 파일만 업로드하면 된다.
- EC2(Elastic Computer Cloud) : 컴퓨터 직접 업로드 가능
3-1. 백엔드 환경을 만든다.
- 빌드된 .jar 파일을 배포한다.
3-2. 프론트엔드 환경을 만든다.
- 빌드된 압축파일을 배포한다.
4. 오류 발생시 로그 확인
- [error] 중점 확인
5. 코드를 수정한다.
- 각 환경에서 수정 후 배포
#
이클립스 코드 수정 후 git bash로 배포  
1. 프로젝트 위치에서 git bash 열기
2. git add.
3. git commit -m "커밋내용"
4. git push origin main 

