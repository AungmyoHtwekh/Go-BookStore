# Go-BookStore

Book Store Managent System needs to run with mysql to work.Book information can add,edit and delete into mysql db via REST APIs.

curl --location --request POST 'http://localhost:9091/book' \
  --header 'Content-Type: application/json' \
  --data-raw '{
      "name": "Harry Potter",
      "author": "J. K. Rowling",
      "publication": ""
  }'
  
  curl --location --request GET 'http://localhost:9091/book' \
  --header 'Content-Type: application/json' \
  
  curl --location --request GET 'http://localhost:9091/book/1' \
  --header 'Content-Type: application/json' \
  
  curl --location --request DELETE 'http://localhost:9091/book/1' \
  --header 'Content-Type: application/json' \
  
curl --location --request PUT 'http://localhost:9091/book/1' \
  --header 'Content-Type: application/json' \
  --data-raw '{
      "name": "Harry Potter",
      "author": "J. K. Rowling",
      "publication": ""
  }'
