<?php

$host = 'localhost';
$user = 'root';
$pass= '';

/*  Connection in database usind PDO
*/

try {

	$conn = new PDO("mysql:host=$host", $user , $pass);

    $sql = "CREATE DATABASE testdb";

    $conn->exex($sql);

    echo "Database is created";

} catch (Exception $e) {

	echo "Database not created, something went wrong!";
}

?>
DATABASE 
