# Laravel-environment
Fast installation of laravel, laradock and all dependencies on the server.

<h2>Set up the server environments</h2>
<ul>
  <li> <b>Copy paste</b> laradock and laravel project files </li>
  <li> <b>Check</b> sure that project structure is
  /var/www/project_name/laravel/ and
  /var/www/project_name/laradock/ </li>
  <li> <b>Install</b> docker </li>
  <li> <b>Check</b> working email in laradock/caddy dirictories </li>
  <li> <b>Run</b> a command <code>docker-compose build workspace </code></li>
  <li> <b>Run</b> a command <code>docker-compose up -d mysql caddy </code></li>
  <li> For workspace <b>run</b> <code>docker-compose exec workspace bash</code> </li>
</ul>
<h2>Project set up</h2>
<ul>
  <li><code>composer install</code></li>
  <li><code>sudo chgrp -R www-data storage bootstrap/cache</code></li>
  <li><code>sudo chmod -R ug+rwx storage bootstrap/cache</code></li>
  <li><code>npm install</code> </li>
  <li><code>php artisan migrate</code></li>
  <li><code>php artisan db:seed</code> </li>
  <li><code>php artisan sleepingowl:install</code></li>
  <li><code>php artisan vendor:publish --tag=assets --force</code></li>
</ul>
<h2>Others</h2>
<ul>
  <li><i>guide for all laradock https://github.com/LaraDock/laradock/issues/225</i></li>
  <li><i>fix problem with mysql db and users https://github.com/laradock/laradock/issues/950</i></li>
</ul>
