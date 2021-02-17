### Application structure:
* Application based on laravel framework which use MVC pattern.
* Models: And it exists in `App` directly.
* Views: And it exists in `resources/views` directory.
* Controllers: And it exists in `App/Http/Controllers` directory.
* Languages: And it exists in  `resources/lang`. directory

* And to validate any request we user, `Form Request` classes which exists in `App\Http\Requests`.
  
### Notes about view: 

* Central admin have master layouts that other modules layouts inherit it.
* Every module has 3 base files `index.blade.php` to list data, 
`grid.blade.php` to build grid for data, `form.blade.php` to edit or create new data.
* About javascript we us main javascript file `action.js` that contains ajax request using axios library,
this file exists in `public/assets/admin/js`.
* About css files we use 2 main files for languages like `style_en.css` for english, `styles.css` for arabic,
that exist in `public/assets/admin/css`.

### Common functions
* In common functions we use helpers that exist in `App\Helpers` that we can call up it in everywhere in application.
* We use `helper.php` file which contains some function like `currentLanguage()` which get current application
language, `getCurrentLocal()` which specific current application local whether it's `ar` or `en`, `languages()` to get application
languages.
* We also use ImageHelper class to upload files and resize images.
