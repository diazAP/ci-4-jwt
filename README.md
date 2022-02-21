# ci-4-jwt

## Reference

- https://www.binaryboxtuts.com/php-tutorials/codeigniter-4-json-web-tokenjwt-authentication/
- https://codeigniter.com/user_guide/index.html
- https://github.com/firebase/php-jwt

## Install

1. run composer install
2. Create DB name ci_4_jwt
3. run php spark migrate
4. run php spark serve
5. http://localhost:8080/api/register , http://localhost:8080/api/login , http://localhost:8080/api/users for testing (https://www.binaryboxtuts.com/php-tutorials/codeigniter-4-json-web-tokenjwt-authentication/#Screenshots)

## Tutorial Steps

1. Install CI4
2. env > .env. CI_ENVIRONMENT = development (check error) and setting DB
3. Create Model and Migration(for creating table on db)
4. Install jwt (composer require firebase/php-jwt) and create Constants (JWT_SECRET_PRIVATE & JWT_SECRET_PUBLIC) key from https://github.com/firebase/php-jwt - Example with RS256 (openssl)
5. Create Controller(Register,Login,User)
6. Create Filter(for auth & cors)
7. Register Routes
8. Run Apps & Testing
