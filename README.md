# wordcloud(형태소 분석을 통한 키워드 추출)

</br>

- 팀 구성원

| frontend                                   | backend                                   |
| ------------------------------------------ | ----------------------------------------- |
| 🐶 [김종원](https://github.com/jonnygim)   | 🐱 [손현오](https://github.com/SonHyeono) |
| 🐔 [정지현](https://github.com/jjhyunjung) | 🐰 [김진주](https://github.com/dingdoooo) |

</br>

- 서비스 소개 :**_형태소 분석을 통한 키워드 추출🚀_**

- 프로젝트 기간 : 22/02/23 ~ 22/02/25

- 기술 스택

|                                                                                                                    |                                                                                                                   |                                                                                                                                 |                                                                                                                 |
| ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| ![html](https://user-images.githubusercontent.com/26592315/155648679-2bb5cba7-6f74-4f5c-a25a-1eb2adb80953.png)HTML | ![css](https://user-images.githubusercontent.com/26592315/155648681-bcbe82bd-f25a-4d4c-8aa0-d85651c2769f.png) CSS | ![javascript](https://user-images.githubusercontent.com/26592315/155648740-abbf6915-e760-4a4a-860a-9bf0ff4c02b4.png) JavaScript | [Naver 오픈 api(검색 api)](https://developers.naver.com/docs/serviceapi/search/news/news.md#%EB%89%B4%EC%8A%A4) |

</br></br>

- 프로그램 실행 화면

1. < 시작 화면 >
   ![image](https://user-images.githubusercontent.com/26592315/155640962-74394f1f-c278-414b-b85c-7a9d6d296fef.png)

2. '대선' 검색

3. < 실행 결과 >
   ![image](https://user-images.githubusercontent.com/26592315/155640999-d3ac879e-6ebe-49ac-af95-19b2d7154004.png)

---

</br>

## wordcloud-backend

1. 사용한 npm list

   | npm list |
   | -------- |
   | express  |
   | request  |
   | dotenv   |
   | koalanlp |

2. wordcloud-backend 설명

- main : server.js
- server.js -> index.html -> script.js -> server.js -> script.js

> - 입력한 text를 script.js에서 debouncer(2초)를 통한 입력을 받고 server.js로 넘긴 후 Naver api를 이용해서 검색된 값을 긁어 온 후 KoalaNLP로 명사만 추출.
> - 명사의 빈도수를 계산하고, 내림차순 정렬 후의 객체를 script.js로 넘겨서 키워드 10개를 출력.

3. 참고

#### [KoalaNLP](https://github.com/koalanlp/nodejs-support)

---

## 개선점

1. github 저장소 정리
2. 결과 값이 3글자면 늘어지는 부분
3. 한번 검색하면 다시 재 검색 안되는 부분.
4. 데이터 별로 접근해서 front에서 조정해야 함.
5. 코드 정리 후 Lighthouse로 코드 개선하기.

---
