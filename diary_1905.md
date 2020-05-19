# Diary 19.05.2020

* prepared statements with bind_parameters:
```php
$sql = "INSERT INTO wiki_user (username, user_password, first_name, last_name, email) VALUES (?, ?, ?, ?, ?)";
$register = $con->prepare($sql);
$register->bind_param('sssss', $username, $password, $firstName, $lastName, $email);
$register->execute();
```
* it is also possible (ind PDO) to exchange the "?" in the sql statement with names. with ```:username```, then you can reference them easier when you bind parameters:
  ```php
  $register->bindParam(':username', $username);
  ```