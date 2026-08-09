# Tech Society ERP

Laravel 12 + PostgreSQL foundation for a configurable Housing / Cooperative Society ERP.

## Current milestone
This repository contains the initial implementation foundation and domain schema for v1.0 Office Operations.

Core domains:
- Societies, phases, blocks, properties
- Memberships and joint membership holders
- Property subdivision
- Property restrictions / encumbrances
- Ownership transfers
- Effective-dated maintenance tariffs
- Management Committee resolutions
- Credits / advances / adjustments
- Special assessments
- Configurable authorizations
- Audit trail

## Setup

1. Install PHP 8.3+, Composer, PostgreSQL and Node.js.
2. Copy `.env.example` to `.env` and configure PostgreSQL.
3. Run:
   composer install
   php artisan key:generate
   php artisan migrate
   npm install
   npm run build
   php artisan serve

The schema is intentionally designed to enforce the business rules at the application/service layer and through database constraints where practical.

## Important
This is the starting codebase, not a claim that every UI/workflow is finished. The next development milestone should implement authenticated admin screens and service-layer workflows around these migrations.
