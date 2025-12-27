# AlKahf Construction — Laravel Experience

A Laravel-based corporate experience for **AlKahf Construction**, pairing the existing glassmorphic design, parallax motion, and role-aware CMS controls with a proper application skeleton.

## Features
- Apple-inspired glass aesthetic with parallax hero, services, projects, delivery method, and executive CTA panels.
- Client-side CMS controls (admin vs. basic roles) for categorized posts with inline publishing, filtering, and deletion.
- Laravel-ready structure with routing, configuration stubs, environment template, and cached storage paths to extend the experience into a full app.

## Getting started
1. Copy the environment template: `cp .env.example .env`.
2. Install dependencies (requires network access): `composer install`.
3. Generate the app key: `php artisan key:generate`.
4. Serve locally: `php artisan serve` then open `http://localhost:8000`.

> The front-end experience is rendered from `resources/views/home.blade.php`. Adjust it or layer server-driven data as needed.
