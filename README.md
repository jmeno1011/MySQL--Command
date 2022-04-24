# MySQL Command

## 테이블 생성 (create)

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

## 테이블 조회 (select)

```SQL

SELECT * FROM 테이블명;

SELECT * FROM 테이블명 WHERE 칼럼명 = "검색어";

SELECT * FROM 테이블명 ORDER BY 칼럼명;

-- 오름차순
SELECT * FROM 테이블명 ORDER BY 칼럼명 ASC;

-- 내림차순
SELECT * FROM 테이블명 ORDER BY 칼럼명 DESC;

```

## 테이블 데이터 입력 (insert)

```SQL

-- 테이블 칼럼 순서대로 값이 들어간다.
INSERT INTO 테이블명 VALUES(value1, value2, value3, ...);

-- 테이블 칼럼 입력한 순서대로 값이 들어간다.
INSERT INTO 테이블명(column1, column2, column3, ...)  VALUES(value1, value2, value3, ...);

```

## 테이블 데이터 업데이트 (update)

```SQL

UPDATE 테이블 SET column1 = "value1" WHERE 칼럼명 = "검색어";

```

## 테이블 데이터 삭제 (delete)

```SQL

DELETE FROM 테이블명 WHERE column1='value1';

```

## 테이블 컬럼 변경

```SQL

-- 새로운 칼럼 추가
ALTER TABLE 테이블명 ADD 컬럼명 자료형;

-- 새로운 칼럼 추가 하는데 위치는 지정칼럼명 다음 위치
ALTER TABLE 테이블명 ADD 컬럼명 자료형 AFTER 지정칼럼;

-- 컬럼명 변경
ALTER TABLE 테이블명 CHANGE 기존컬럼명 새컬럼명 자료형;

-- 컬럼 자료형 변경
ALTER TABLE 테이블명 CHANGE 컬럼명 컬럼명 바꿀자료형;

```
