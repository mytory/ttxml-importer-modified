# TTXML Importer Modified

기존 TTXML Importer를 약간 개선한 버전이다.

1. 이전에는 이미지만 옮길 수 있었지만, 모든 파일을 일단 옮기도록 시도하게 했다. hwp를 위험한 파일로 인지하지 않게 설정했으므로 hwp는 잘 옮겨질 것이다.
1. 기존엔 첨부 파일을 모두 `1`이란 디렉토리를 만들고 넣게 돼 있었다. 이제 워드프레스 설정에 따라 업로드 디렉토리를 만들어서 넣는다.
1. 본문 첨부파일의 링크 텍스트가 `cfile29.uf.2260EF4B533846E8349C1B.zip` 식으로 들어가서 보기 흉했는데, 원래 업로드한 파일명으로 링크텍스트가 나오게 했다.
1. `deprecated` 함수를 두 개 지웠다. (`screen_icon()`, `$wpdb->escape()`)
1. `postmeta`에 `_tistory_id`라는 이름으로 티스토리의 고유번호를 넣었다. 원래의 티스토리 URL과 매치할 생각이 있는 사람들이 활용할 수 있도록 한 것이다.

