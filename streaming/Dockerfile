# 1. 실행용 경량 JDK 이미지 사용
FROM openjdk:17-jdk-slim

# 2. 작업 디렉토리 설정
WORKDIR /app

# 3. 로컬에서 빌드한 JAR 파일을 컨테이너 내부로 복사
COPY build/libs/*.jar app.jar

# 4. 컨테이너가 실행될 때 JAR 파일 실행
ENTRYPOINT ["java", "-jar", "app.jar"]
