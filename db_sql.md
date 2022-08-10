```mysql
DROP DATABASE IF EXISTS article_manager;
CREATE DATABASE article_manager;


CREATE TABLE article (
    id INT(10) UNSIGNED NOT NULL PRIMARY KEY AUTO_INCREMENT,
    regDate DATETIME NOT NULL,
    updateDate DATETIME NOT NULL,
    title CHAR(100) NOT NULL,
    `body` TEXT NOT NULL
);

DESC article;
SELECT *
FROM article;

INSERT INTO article
SET regDate = NOW(),
updateDate = NOW(),
title = '제목',
`body` = '내용';


```




