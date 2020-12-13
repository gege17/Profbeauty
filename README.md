<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 1500 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).









profbeauty პროექტი ადმინისტრირების პანელით, აუთენტიპიკაციით და სხვადასხვა ფუქნციონალით, შეიცავს CRUD ოპარეციებს, one to many რელაციას, ძალიან ბევრ custom ელემენტს, მათ შორის ვალიდაციებს. ჩაშენებული javascript datatable პლაგინის ჩემ მიერ გაქართულებული ვერსიით, ყურადღება მივაქციე ადმინ პანელის ვიზუალურ მხარესაც. რაც შეეხება permission-ს გვაქვს ორი ტიპის user, admin და user. დეფოლტად ბაზაში მომხმარებელს რეგისტრაციისას გადაეცემა user permission. მას არ აქვს ადმინ პანელში შესვლის უფლება, მხოლოდ დატაბაზიდან შეიძლება permission ის შეცვლა და გადაგვყავს admin-ზე. რაც შეეხება არსებულ მარკაპთან ინტეგრაციას რომელიც welcome view როუტით გვაქვს წარმოდგენილი, საჭიროებს დახვეწას, ფრონტ-ენდ დეველოპერისა და ბექენდ-დეველოპერის უკუკავშირს ერთმანეთთან და კომუნიკაციას. 

რაც შეეხება პროექტის დაყენებას:

1)დაკლონეთ
2)env.example ფაილი გადააკოპირეთ და ჩასვით ახალ .env ფაილში და მონაცემთა ბაზას დაუკავშირეთ(მონაცემთა ბაზა უნდა იყოს ცარიელი).
3)გაუშვით composer install ბრძანება ტერმინალში მოცემულ პროექტზე
4)გაუშვით php artisan key:generate ბრძანება ტერმინალში მოცემულ პროექტზე
5)გაუშვით php artisan migrate --seed ბრძანება ტერმინალში მოცემულ პროექტზე (წესით ბაზის მონაცემები უნდა გადავიდეს).
6)ტერმინალში მოცემული პროექტის მისამართზე დააინსტალირეთ npm შემდეგი კომანდით - npm install
7)მისი ინსტალაციის შემდეგ კი გაუშვით ბრძანება - npm run dev
8)გაუშვით პროექტი ლოკალურად php artisan serve

თუ ჩემი ბაზის მონაცემები გადასულია, ვგულისხმობ აქაუნთს, რომელიც user table ში უნდა გამოჩნდეს(მეილი: gegechkori647@gmail.com და პაროლი: 12345678)
შეგიძ₾იათ ამით გადახვიდეთ ადმინ-პანელში დაამატეთ ლოკალურად გაშვებული პროექტის URL-ს /dashboard ამის შემდეგ მოგახვედრებთ ავტორიზაციის გვერდზე, ჩაწერთ მოცემულ მეილს და პაროლს და გადახვალთ ადმინზე.

თუ არ არის გადასული მონაცემები, ვიმეორებთ იგივეს, ანუ გადახვალთ ადმინის გვერდზე საიდანაც გადაგამისამართებთ ავტორიზაციის გვერდზე, იქიდან მარტივად დარეგისტრირდებით, შემდეგ გახსნით ბაზას თქვენ მიერ შექმნილი აქაუნთს, რომელიც უკვე აისახება ბაზაში, ექნება permission გრაფა, სადაც ეწერება user და მას ჩავანაცვლებთ admin-ით. ამის შემდეგ თქვენ უკვე ადმინის უფლებებით ისარგებლებთ და შეძლებთ /dashboard - ზე გადასვლას.

გმადლობთ ყურადღებისთვის!
