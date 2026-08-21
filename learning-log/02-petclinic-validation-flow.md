# Petclinic 검증 실패 흐름 추적

- 찾은 Controller와 메서드: OwnerController, processCreationForm
- POST 요청: /owners/new
- @Valid: 입력 파라미터 owner의 필드 값이 유효한지 검사한다.
- BindingResult: 오류 결과를 보관한다.
- 오류 판단: result.hasErrors()
- 오류 시 결과: 새 Owner 입력 화면을 반환한다.
