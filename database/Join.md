# JOIN
Join: 두 개 이상의 테이블 or DB를 연결해 검색하는 방법 <br>
(적어도 하나의 칼럼을 서로 공유해야함)
<br>

## 종류
- inner join<br>
  
  ![inner join](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FZiezB%2FbtqC3rs5tsT%2Frt6imsvIsU7gh0Wm0JPTk0%2Fimg.png)
  <br>
  
  select <br>
  A.name, B.age <br>
  from ex_table A <br>
  inner join join_table B on A.no_emp=B.no_emp<br>

- left outer join
  
    ![left outer join](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcGzLt9%2FbtqC21H7s3O%2FKaOeOKQP63GMmooh15ZBF0%2Fimg.png)
    
    select <br>
    A.name, B.age <br>
    from ex_table A <br>
    left outer join join_table B on A.no_emp=B.no_emp<br>

- right outer join
  
  ![right outer join](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2F2zm1r%2FbtqC4uQqEzd%2FvzlPP2G5sIFkk6CYOv63Vk%2Fimg.png)

    select <br>
    A.name, B.age <br>
    from ex_table A <br>
    right outer join join_table B on A.no_emp=B.no_emp<br>


- full outer join
  
  ![full outer join](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbEwa8U%2FbtqCZymSjyT%2FGM2d6rnDkw2JTfM5XHgADK%2Fimg.png)

    select <br>
    A.name, B.age <br>
    from ex_table A <br>
    full outer join join_table B on A.no_emp=B.no_emp<br>

- cross join
  
  ![cross join](https://t1.daumcdn.net/cfile/tistory/997A563D5DCEA67328)

    모든 경우의 수를 표현하는 방식<br>
    ex) A: 3개 , B: 4개 --> 3 x 4 = 12개 표현<br>
    select <br>
    A.name, B.age <br>
    from ex_table A <br>
    cross join joim_table B

- self join
  
   ![self join](https://t1.daumcdn.net/cfile/tistory/993262335B1791442D)

   자기자신과 조인하는 것<br>
   하나의 테이블 여러번 복사해 join함<br>
   자신이 갖고 있는 칼럼을 다양하게 변형하고 싶을 때 사용<br>
    select <br>
    A.name, B.age <br>
    from ex_table A, ex_table B <br>
    

