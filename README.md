Tutorial Jalankan docker
NOTE : Pastikan Composer dan npm sudah terinstall, .env juga disesuaikan

jalankan : 

composer install
composer update

/// build docker
docker-compose up --build
/// aplikasi dapat diakses di localhost:8000 dan phpmyadmin di localhost:8080, setup database di phpmyadmin jika perlu

php artisan vendor:publish --tag=admin-core
php artisan migrate --seed --seeder=AdminCoreSeeder
php artisan storage:link
npm install
npm run dev



Login Superadmin
Email - superadmin@example.com
Password - password