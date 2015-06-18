PHP Library for the Optimus API
=======================
Lossless image compression API

More details about Optimus are available on [optimus.io](https://optimus.io/en/).

Please let us know if you got questions or feedback: [Optimus Support](https://www.keycdn.com/contacts)

## Requirements
- PHP 5.3 or above
- PHP Curl Extension

## Usage
```php
<?php

require '/path/to/src/optimus.php';

// create object and pass API license key
$optimus = new Optimus('<your_license_key>');

// optimize image
$result = $optimus->optimize('/path/to/image.jpg');

// save optimized image
file_put_contents('/path/to/image.jpg', $result);

...

?>
```

## Convert to WebP image format

```php
// optimize image and convert to webp
$result = $optimus->optimize('/path/to/image.jpg', 'webp');

// save optimized image with webp extension
file_put_contents('/path/to/image.webp', $result);
```
