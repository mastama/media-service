# media-service

1. generate folder media-service
    express --no-view media-service
2. npm install
3. membuat file .env dan .gitignore
4. ubah var pada file didalam folder routes dan file app.js menjadi const agar lebih modern

<!-- set up sequelize dan sequelize-cli -->
1. npm install sequelize sequelize-cli(untuk menggunakan command" sequelize) --save
2. check apakah sudah terinstall dan untuk mengecek command yang ada pada sequelize: npx sequelize
3. initialize project: npx sequelize init:
    - config
    - models
    - migrations
    - seeders
4. ubah file config.json ke config.js lalu sesuaikan value nya

<!-- Membuat migration dan model -->
1. npx sequelize migration:generate  --name=create-table-media
2. sesuaikan value nya
3. npx sequelize db:migrate
4. npm install mysql2 --save
5. npx sequelize db:migrate:undo (gunakan ini jika ingin membatalkan generate sebelumnya)
6. membuat model secara manual