# node-interceptor PHP SDK

<!-- simple-start:start -->
Use node-interceptor from a PHP app.

**Start here.** Run `composer require titancsa/node-interceptor`, then try the short example below. Install the matching Windows driver separately.
<!-- simple-start:end -->

> [!IMPORTANT]
> **Get the driver without the one-hour demo limit**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about the full **Interceptor** driver for this SDK. TitanCSA shares purchase details privately.

`composer require titancsa/node-interceptor`

Windows x64 PHP8.2+; enable FFI extension and `ffi.enable=true`.

```php
require "vendor/autoload.php";
$client=new \TitanCSA\Products\NodeInterceptor\Client();
try {print_r($client->call("check", ["device" => 1]));} finally {$client->close();}
```

[API and operation schema](docs/API.md). Matching driver installed separately.
