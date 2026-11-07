# My Dhaka Shop

This repository contains the foundational Laravel e-commerce application for My Dhaka Shop, designed for a Bangladeshi multi-product online store with wallet, checkout, admin dashboard, and deployment documentation.

## Stack

- Laravel 11
- PHP 8.2+
- MySQL
- Tailwind CSS
- Google OAuth via Laravel Socialite
- NobabPay integration-ready service layer
- cPanel deployment ready

## Notes

This initial codebase provides the project structure, core migration foundation, admin/customer routes, models, seeders, and the main storefront layout. Additional production integrations such as full NobabPay live callback verification and advanced admin UI logic can be completed in the next iteration after credentials are supplied.

## Setup

1. Copy `.env.example` to `.env`
2. Configure database and credentials
3. Run `composer install`
4. Run `php artisan key:generate`
5. Run `php artisan migrate --seed`
6. Run `php artisan serve`

## Important

- Never commit live payment credentials.
- Store NobabPay, Google OAuth, and wallet secrets in `.env`.
- Use server-side verification for all payment callbacks.
