使用事例：

require 'vendor/autoload.php';

use HeyShop\Token\HeyShopMultipass;

$customer_data = array(

    "mobile" => "133xxxx4252",
    "email" => "zy@xxxxxxxx.com",
    "full_name" => "OC",
    "remote_ip" => "127.0.0.1"
);

$multipass = new HeyShopMultipass('secret');

$token = $multipass->generate_token($customer_data);

var_dump($token);
