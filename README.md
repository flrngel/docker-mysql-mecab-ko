# docker-mysql-mecab-ko

Usage:

```
$ # change `MYSQL_ROOT_PASSWORD` below
$ docker run -p 3306:3306 --name mmk -e MYSQL_ROOT_PASSWORD=asdfasdf flrngel/mysql-mecab-ko
$ docker exec -it mmk mysql -p

mysql> CREATE FULLTEXT INDEX ft_index ON sexy_items (title,description,keywords) WITH PARSER mecab;
```

## Thanks to

[은전한닢 Project](https://bitbucket.org/eunjeon)

## References

- [MeCab Full-Text Parser Plugin](https://dev.mysql.com/doc/refman/5.7/en/fulltext-search-mecab.html)
- [mecab-ko-dic](https://bitbucket.org/eunjeon/mecab-ko-dic)
