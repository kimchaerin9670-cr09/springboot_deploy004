# 1. 실행 환경 설정 (Java 21)
FROM eclipse-temurin:21-jre-jammy

# 2. 작업 디렉토리 설정
WORKDIR /app

# 3. JAR 파일 복사
# 빌드 컨텍스트를 루트(.)로 잡을 것이므로 경로를 맞춥니다.
ARG JAR_FILE=deploy004_springboot/target/*.jar
COPY ${JAR_FILE} app.jar

# 4. 애플리케이션 실행
ENTRYPOINT ["java", "-jar", "app.jar"]