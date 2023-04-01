# Join
두 개의 테이블을 서로 묶어서 하나의 결과를 만들어 내는 것을 말한다.

# 셀프 조인(Self Join)
- 셀프조인은 자신과 자신이 조인한다는 의미로 1개의 테이블을 사용한다.

# 설명
J-4) 자신의 매니저보다 먼저 고용된 사원들의 LAST_NAME 및 고용일을 조회하시오.
- LAST_NAME(이름), HIRE_DATE(고용일)을 조회한다.
- 테이블을 구분하기 위해 EMPLOYEES E(사원), EMPLOYEES M(매니저) 별칭을 해준다.
- 첫번째 조건은 사원 테이블의 매니저아이디랑 매니저 테이블의 사원 아이디를 등가 조인을 해준다.
- AND라는 연산자를 써 다음 조건을 만족시켜야지 결과가 나온다.
- 두번째 조건은 매니저 테이블의 고용일자가 사원 테이블의 고용일자보다 크다라는 조건이다.
# Java Cord
![image](https://user-images.githubusercontent.com/122009563/228715454-ff2f74de-8e56-4fad-80c7-5de38873c71e.png)

# 실행결과
![image](https://user-images.githubusercontent.com/122009563/228715712-0f943b8f-2859-4884-9f72-e2e91b04f22a.png)

# 내부 조인(Inner Join)
둘 이상의 테이블에 존재하는 공통 속성의 값이 같은 것을 결과로 추출하는것을 말한다.

# 설명
J-2) 급여가 2500이하이고 사원번호가 200이하인 서울의 LAST_NAME, 부서명을 조회하시오.
- LAST_NAME(이름), DEPARTMENT_NAME(부서명)을 조회한다.
- 테이블을 구분하기 위해 EMPLOYEES E(사원), DEPARTMENTS D(부서) 별칭을 해준다.
- 첫번째 조건은 사원테이블의 DEPARTMENT_ID(부서 아이디) 부서테이블의 DEPARTMENT_ID(부서 아이디)를 등가 조인을 해준다.
- AND라는 연산자를 써 다음 조건을 만족시켜야지 결과가 나온다.
- 두번째 조건은 급여가 2500 이하라는 조건이다.
- 세번째 조건은 사원번호가 200 이하라는 조건이다.

# Java Cord
![image](https://user-images.githubusercontent.com/122009563/228753455-1e757544-24c4-477b-91b4-c73185fce7f7.png)

# 실행결과
![image](https://user-images.githubusercontent.com/122009563/228753535-c267b6c2-85f2-4eca-89e7-d77c3f4923e3.png)

# 외부 조인(Outer Join)
두 테이블을 조인할 때, 1개의 테이블에만 데이터가 있어도 결과가 나오는것을 말한다.

# 설명
J-3) 사원정보(EMPLOYEE_ID, LAST_NAME, MANAGER_ID)와 사원의 직속 상관정보(EMPLOYEE_ID, LAST_NAME) 조회하시오.

# Java Cord
![image](https://user-images.githubusercontent.com/122009563/228765011-27667dc1-ea3c-4653-90ae-a1cad6f41bec.png)

# 실행결과
![image](https://user-images.githubusercontent.com/122009563/228764827-db8afdb0-7741-4290-b1fd-7822f8ed7d72.png)

