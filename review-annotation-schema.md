# 이미지 리뷰 분류·선별 스키마

리뷰 사이트는 다음 두 localStorage 키를 사용합니다.

- `series-reference-categories-v1`: 이미지 키(ID_번호)와 선택된 범주 ID 배열
- `series-reference-decisions-v1`: 이미지 키(ID_번호)와 `pick` 또는 `drop` 값

| ID | 범주 |
|---|---|
| shape | 형태유사 |
| color | 색상유사 |
| material | 재질유사 |
| feature | 특징적 요소 공유 |
| volume | 부피감유사 |
| technique | 제조기법유사 |

분류·선별 JSON 저장은 상태가 기록된 이미지의 파일명·작가·출처·선택 범주·선별 상태를 `series-reference-annotations.json`으로 저장합니다. 내보내기 스키마는 `series-reference-review-v2`이며 `reviewed_images`, `picked_images`, `dropped_images`를 포함합니다. Drop 상태의 이미지는 리뷰 화면에서 낮은 불투명도와 블러로 블라인드됩니다.
