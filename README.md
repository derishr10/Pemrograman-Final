# Pemrograman-Final
web ini saya desain menggunakan PHP 7, apabila menggunakan PHP 8.
siapa tau muncul erorr seperti ini :
"fatal error: cannot redeclare str_contains() in C:xampp\htdocs\inventarisbarang\helpers\function.php on line 524"
ketika dijalankan.

untuk mengatasi hal tersebut jika menggunakan PHP 8, silahkan ubah C:xampp\htdocs\inventarisbarang\helpers\function.php on line 524

function str_contains($needle, $haystack)
{
	return strpos($haystack, $needle) !== false;
}

ubah menjadi 

error_reporting(0);
if(strpos($haystack,$needle)!== false){
echo";
}
