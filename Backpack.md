## Backpack

### Содержание
* **Установка**
* **Подключение**


---

### Установка
   + **1.** - `composer require backpack/base`
   + **2.** - в **config/app.php** 
   ```php
   $providers = [
   ...
   /*
    * Backpack Service Providers...
    */
    Backpack\Base\BaseServiceProvider::class,
   ```
   + **3.** - 
   ```
   php artisan vendor:publish --provider="Backpack\Base\BaseServiceProvider" #publishes configs, langs, views and AdminLTE files
   php artisan vendor:publish --provider="Prologue\Alerts\AlertsServiceProvider" # publish config for notifications - prologue/alerts
   php artisan migrate #generates users table (using Laravel's default migrations)
   ```

