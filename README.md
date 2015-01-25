# laraveltest

----Create Migration

php artisan migrate:make create_users_table

----Agregar campos en la table

	Schema::create('users', function(Blueprint $table)
		 {
			$table­>increments('id'); 
			$table­>string('email')­>unique(); 
			$table­>string('password', 60); 
			$table­>rememberToken()­>index(); 
			$table­>timestamps();
		});

----Migrate Database

php migrate database




