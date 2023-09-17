## Next.js Laravel Chirper API Backend with Next.js Frontend

[The Laravel Bootcamp](https://bootcamp.laravel.com/) demonstrates three different ways to build a microblogging platform called Chirper, [with Blade](https://bootcamp.laravel.com/blade/installation), [with Livewire](https://bootcamp.laravel.com/livewire/installation), and [with JavaScript and Inertia](https://bootcamp.laravel.com/inertia/installation).

This project is trying to <b>use Laravel Chirper API as the backend and set up web display and authentication with Next.js as the browser frontend</b>.
The Laravel Chirper API includes Laravel Breeze API, a minimal, simple implementation of all of Laravel&apos;s authentication features, including login, registration, password reset, email verification, and password confirmation.
Laravel Sanctum is incorporated with Laravel Breeze to provide the authentication system.
In addition to API tokens, Sanctum offers a simple way to authenticate single-page applications (SPAs) that need to communicate with a Laravel-powered API.
For this, Sanctum uses Laravel&apos;s built-in cookie-based session authentication services.

This project basically follows the ideas of demonstrations in the Laravel Bootcamp, and some additional features as below are added: 
- Chirper displays are loaded with scrolling pagination.
- Periodically update the Chirper display following the page is loaded.
- Mechanisms for users to follow and unfollow other users.
- The Laravel Bootcamp demonstrations provide a mechanism to send email notifications when a new Chirp is created to every other user, in this project we restrict the email notifications to the user&apos;s followers only.

### Docker:
```
# Run the following two commands simutaneously with diffrent screen windows...

docker run -it -p 8000:8000 jglchen/chirper-api php artisan serve --host=0.0.0.0
docker run -p 3000:3000 jglchen/chirper-next
```

### Docker Compose:
```
# At the root of the /chirper-api-w-next folder...
docker compose up
```
### [App GitHub](https://github.com/jglchen/chirper-api-w-next)

