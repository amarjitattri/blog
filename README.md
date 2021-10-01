Usage Instructions

1. Clone the project
2. composer install
3. create .env file
4. php artisan key:generate
5. create a new database and add database credentials to .env file.
6. php artisan migrate --seed
	By Default seeder will create admin user. For admin user, you will see all permissions. but when you create a new user by register route. For these types of users have by default add and show the posts permission.
7. BROADCAST_DRIVER=pusher
8.  set env variables
	PUSHER_APP_ID=1275707
	PUSHER_APP_KEY=8abf281cfc818a9e98ff
	PUSHER_APP_SECRET=9a74b045671a6fecbc6d
	PUSHER_APP_CLUSTER=ap2
9. run "php artisan serve" to run the project
10. By default I set the schedular command to fetch post from API after 1 hour. If you want to run the command manually then hit this command "php artisan fetch:posts".
11. To run the test case create new .env.testing file and also create a new database for testing after that run this command "php artisan test".
