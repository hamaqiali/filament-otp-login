# Changelog

All notable changes to `filament-otp-login` will be documented in this file.

## v2.0.0 - 2025-01-28

### 🚀 Major Update - Filament v4 & Laravel 11 Support

This is a major version release with breaking changes for upgrading to Filament v4 and Laravel 11.

#### ⚡ What's Changed

* **Upgraded to Filament v4** (from v3) - now requires `filament/filament: ^4.0`
* **Upgraded to Laravel 11** (from Laravel 10) - via Filament v4 dependencies
* **Upgraded to Tailwind CSS v4** - using Filament's built-in Tailwind v4 support
* **PHP 8.2+ required** (from PHP 8.1)
* Updated all dev dependencies for compatibility:
  - `nunomaduro/collision` to v8
  - `orchestra/testbench` to v9
  - `pestphp/pest` to v3
  - All pest plugins to v3
* Simplified build configuration - removed unused Tailwind build scripts (plugin uses Filament's built-in styles)
* Migrated configuration files to ES modules for v4 compatibility

#### 🔄 Breaking Changes

* **Minimum PHP version: 8.2+**
* **Requires Filament v4** - not compatible with Filament v3
* **Requires Laravel 11** - not compatible with Laravel 10

#### ✅ Compatibility

All existing functionality remains the same:
- OTP login flow
- Email notifications
- Rate limiting
- Direct login bypass with `CanLoginDirectly`
- Custom OTP input component

No code changes required in your implementation - only update your `composer.json` to require v2.

#### 📦 Upgrade Guide

```bash
composer require afsakar/filament-otp-login:^2.0
```

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.4.0...v2.0.0

## v1.4.0 - 2025-05-28

### What's Changed

* Bump dependabot/fetch-metadata from 2.2.0 to 2.3.0 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/16
* Bump aglipanci/laravel-pint-action from 2.4 to 2.5 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/17
* Bump dependabot/fetch-metadata from 2.3.0 to 2.4.0 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/19
* Allow custom notification class for people who would like to use othe… by @maukoese in https://github.com/afsakar/filament-otp-login/pull/18
* Add reset otp input event and method to blade

### New Contributors

* @maukoese made their first contribution in https://github.com/afsakar/filament-otp-login/pull/18

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.6...v1.4.0

## v1.3.6 - 2024-10-18

Add loading indicator to login form submit button

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.5...v1.3.6

## v1.3.5 - 2024-09-03

* Update for customized Login Page, now you can add custom pages for every panel.

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.4...v1.3.5

## v1.3.4 - 2024-08-06

### What's Changed

* Now you can ignore specific users from OTP Login and they login directly without OTP #9
* Bump dependabot/fetch-metadata from 2.1.0 to 2.2.0 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/7

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.2...v1.3.3

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.3...v1.3.4

## v1.3.2 - 2024-07-05

- Fixed a bug where the paste action was not working on firefox. #6
- Fixed Otp Code's "public" status to "private" which caused a security vulnerability. (*Thank to @alex-r-redfern* )
- Added notes about prunable to README.

## v1.3.1 - 2024-06-15

Fixed automatic login when sending OTP notification.

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.3.0...v1.3.1

## v1.3.0 - 2024-06-09

### What's Changed

* Bump aglipanci/laravel-pint-action from 2.3.1 to 2.4 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/2
* Bump dependabot/fetch-metadata from 2.0.0 to 2.1.0 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/3
* Changing the logic of the checkCredentials method by @leonardyrj in https://github.com/afsakar/filament-otp-login/pull/4

### New Contributors

* @leonardyrj made their first contribution in https://github.com/afsakar/filament-otp-login/pull/4

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.2.0...v1.3.0

## v1.2.0 - 2024-04-07

- Added OtpInput Component

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.1...v1.2.0

## v1.1 - 2024-03-24

**Full Changelog**: https://github.com/afsakar/filament-otp-login/compare/v1.0.0...v1.1

## v1.0.0 - 2024-03-24

### What's Changed

* Bump dependabot/fetch-metadata from 1.6.0 to 2.0.0 by @dependabot in https://github.com/afsakar/filament-otp-login/pull/1

### New Contributors

* @dependabot made their first contribution in https://github.com/afsakar/filament-otp-login/pull/1

**Full Changelog**: https://github.com/afsakar/filament-otp-login/commits/v1.0.0

## 1.0.0 - 202X-XX-XX

- initial release
