Tutorial Jalankan docker<br/>
NOTE : Pastikan Composer dan npm sudah terinstall, .env juga disesuaikan<br/><br/>

jalankan : <br/><br/>

composer install<br/>
composer update<br/><br/>

/// build docker<br/>
docker-compose up --build<br/>
/// aplikasi dapat diakses di localhost:8000 dan phpmyadmin di localhost:8080, setup database di phpmyadmin jika perlu<br/><br/>

php artisan vendor:publish --tag=admin-core<br/>
php artisan migrate --seed --seeder=AdminCoreSeeder<br/>
php artisan storage:link<br/>
npm install<br/>
npm run dev<br/><br/>



Login Superadmin<br/>
Email - superadmin@example.com<br/>
Password - password<br/>