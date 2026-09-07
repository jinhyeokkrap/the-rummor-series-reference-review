# 이미지 리뷰 분류 스키마

리뷰 사이트는 series-reference-categories-v1 키로 브라우저 localStorage에 분류를 저장합니다. 값은 이미지 키(ID_번호)와 선택된 범주 ID의 배열로 구성됩니다.

| ID | 범주 |
|---|---|
| shape | 형태유사 |
| color | 색상유사 |
| material | 재질유사 |
| feature | 특징적 요소 공유 |
| volume | 부피감유사 |
| technique | 제조기법유사 |

분류 JSON 저장은 체크가 하나 이상 있는 이미지의 파일명·작가·출처·선택 범주를 series-reference-annotations.json으로 저장합니다.
