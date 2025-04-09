# ✅ Laravel Interview Questions and Answers Explatin

### Q1 - What is Laravel?
#### Ans- Laravel is a PHP web application framework with expressive, elegant syntax. It simplifies tasks like routing, authentication, sessions, and caching.
- Explain
````
Route::get('/', function () {
    return view('welcome');
});
````
### Q2 - What are the key features of Laravel?
#### Ans - Routing, Eloquent ORM, Middleware, Authentication, Blade, Artisan CLI.
- Explain
````
Route::get('/dashboard', function () {
    // Dashboard logic
})->middleware('auth');
````
### Q3 - What is Eloquent in Laravel?
#### Ans - It is Laravel’s ORM that interacts with the database using models.
- Explain
````
$users = App\Models\User::where('active', 1)->get();
````
## Q4 - Difference between get() and first()?
#### Ans - get() returns all matching results and first() returns only the first match.
- Explain
````
User::where('email', 'test@example.com')->get();    // Collection
User::where('email', 'test@example.com')->first();  // Single Model
````
## Q5 - What is a Service Provider?
#### Ans - A central place where Laravel bootstraps services.
- Explain
````
$this->app->bind('MyService', function($app) {
    return new \App\Services\MyService;
});
````
