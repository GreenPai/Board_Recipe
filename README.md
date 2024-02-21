# Board_Recipe
스프링부트, mysql, jpa를 사용해서 만든 게시판입니다.

# 개발환경
1. IDE : IntelliJ IDEA Community
2. Spring Boot 2.6.13
3. JDK 11
4. mysql
5. Spring Data JPA
6. Thymeleaf

# 게시판 주요 기능
1. 글쓰기(/board/save)
2. 글목록(/board/)
3. 글조회(/board/{id})
4. 글수정(/board/update/{id})
    - 상세화면에서 수정 버튼 클릭
    - 서버에서 해당 게시글의 정보를 가지고 수정 화면 출력
    - 제목, 내용 수정 입력 받아서 서버로 요청
    - 수정 처리
5. 글삭제(/board/delete/{id})
6. 페이징처리(/board/paging)
   - /board/paging?page=2
   - /board/paging/2
   - 게시글 14개가 있으면
     - 한 페이지에 5개씩 -> 3개 페이지 필요
     - 한 페이지에 3개씩 -> 5개 페이지 필요