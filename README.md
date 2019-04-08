# grego_composer

UPDATE
  books
SET
  books.primary_author = authors.name
FROM
  books
INNER JOIN
  authors
ON
  books.author_id = authors.id
WHERE
  books.title = 'The Hobbit'
