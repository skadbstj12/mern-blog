# MERN BLOG

MERN 스택은 MongoDB, Experss.js, React, Node.js의 약자로, 풀스택 자바스크립트 애플리케이션 개발을 위한 기술 스택입니다.

## react tjcl

vite를 이용하여 리액트를 설치합니다.

```bash
npm create vite@latest
cd client
npm i
npm run dev
```

## tailwind 설치

CSS는 tailwind[https://tailwindcss.com/docs/guides/vite]를 설치하여 작업하겠습니다.

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

tailwind.config.js 파일을 수정합니다.

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

index.css도 다음과 같이 수정합니다.

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## GIT 연동

모든 파일은 git에 연동하여 사용했습니다.

```bash
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/skadbstj12/mern-blog.git
git push -u origin main
```
