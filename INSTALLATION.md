# Manual Installation

##### Clone this project into your directory.

- If you're using **laragon** clone into `C:\laragon\www\` directory.
- If you're using **xampp** clone into `C:\xampp\htdocs\` directory.

##### Install dependencies.

```bash
composer install
```

and

```bash
npm install
```

##### Create a copy of .env file

```bash
cp .env.example .env
```

then, in the .env file fill the `DB_HOST`, `DB_PORT`, `DB_DATABASE`, `DB_USERNAME`, and `DB_PASSWORD` to match the credentials of the database you just created. Don't forget to create your database.

##### Generate app encryption key

```bash
php artisan key:generate
```

##### Migrate the database

```bash
php artisan migrate
```

##### Run the project

```bash
php artisan serve
```
