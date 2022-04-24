# MySQL Command

## 테이블 생성

```SQL
CREATE TABLE 테이블명
(
칼럼명(ex: \_id) AUTO_INCREMENT,
칼럼명 INT,
칼럼명 VARCHAR(25),
칼럼명 DATE,
PRIMARY KEY(칼럼명)
);
```

## 테이블 조회

```SQL
SELECT * FROM 테이블명;
SELECT * FROM 테이블명 WHERE 칼럼명="검색어";
SELECT * FROM 테이블명 ORDER BY 칼럼명;
-- 오름차순
SELECT * FROM 테이블명 ORDER BY 칼럼명 ASC;
-- 내림차순
SELECT * FROM 테이블명 ORDER BY 칼럼명 DESC;
```

## 테이블 데이터 입력

```SQL
-- 테이블 칼럼 순서대로 값이 들어간다.
INSERT INTO 테이블명 VALUES(value1, value2, value3, ...);
-- 테이블 칼럼 입력한 순서대로 값이 들어간다.
INSERT INTO 테이블명(column1, column2, column3, ...)  VALUES(value1, value2, value3, ...);
```

## 테이블 데이터 삭제

```SQL
DELETE FROM 테이블명 WHERE column1='value1';
```
