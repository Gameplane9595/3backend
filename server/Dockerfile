# 기본 이미지 선택 (Node.js 이미지)
FROM node:18

# 작업 디렉토리 설정
WORKDIR /app

# 패키지 파일(package.json) 복사
COPY package*.json ./

# 패키지 설치
RUN npm ci

# 소스 코드 복사
COPY . .

# 백엔드 서버 포트 번호 설정
EXPOSE 80

# 백엔드 서버 실행
CMD ["npm", "run", "start"]