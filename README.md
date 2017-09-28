# Polyfill Libsodium

A simple Polyfill for giving libsodium compatibility when having sodium installed.

The new sodium extension has been accepted and will be distributed with PHP >= 7.2.  
This will have a few breaking changes:

- No more `\Sodium\` namespace. Everything must be in the global namespace.
- The extension will be renamed to `sodium`. 

So the current namespaced functions will not work anymore. So we created a polyfill for this.

Reference: https://github.com/jedisct1/libsodium-php

# Installation

**Using Composer:**  

The easiest way to install is to require the polyfill-libsodium library with Composer.  
`composer require mollie/polyfill-libsodium`

After installation of the package the bootstrap.php file will be autoloaded.

**Manual installation:**  
Checkout or download all the files and include them manually into your project.

Include the bootstrap file in your project  
`require /path/to/vendor/polyfill-libsodium/bootstrap.php` 

# License
This software is licensed under the [MIT License](LICENSE)

© 2017 Mollie
