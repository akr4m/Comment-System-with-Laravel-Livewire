## Comment System with Laravel Livewire

- Laravel
- Livewire
- Tailwind
- AlpineJs

Demo Project of A Comment System with TALL Stack

### Routes

```php

Route::get('/', function () {
    return view('welcome');
});

Route::get('/dashboard', function () {
    return view('dashboard');
})->middleware(['auth'])->name('dashboard');

Route::get('/articles/{article:slug}', ArticleController::class);
Route::get('/episodes/{episode:slug}', EpisodeController::class);

require __DIR__.'/auth.php';

```
