# Nobelium
Nobelium source, MPL-2.0.

A web server for older versions of the Rocorp client. **[Here's a tl;dr of the license.](https://tldrlegal.com/license/mozilla-public-license-2.0-(mpl-2))** Fork and PR away! There is no specific code style because the project is already messy.

This repo contains zero copyrighted-by-Rocorp code. It's like rAthena, but for that one game made by them! Uses Laravel 5.3.

http://nobelium.xyz

-------------------

**How to compile:**

Requirements:
1. Windows (and linux i think)
2. php 7 for windows (https://windows.php.net/download#php-7.4)
3. Composer (https://getcomposer.org/download/)
4. A MySql server (You can use the XAMPP one)

Steps:

(cd to the nobelium source directory)

1. Run composer upgrade
2. Rename .env.example to .env and edit it to what you prefer.
3. Run mkdir bootstrap/cache
4. Run php artisan cache:clear
5. Run php artisan config:cache
6. Run php artisan migrate
7. Run php artisan key:generate
8. Run php artisan cache:clear
9. Run php artisan config:cache
10. start the webserver by running php artisan serve
