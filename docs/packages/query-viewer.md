---
layout: default
title: Query Viewer
parent: Packages
---

# Query Viewer
{: .no_toc }

This package adds custom methods to eloquent and database query builder for getting sql query. (question marks replaced with values)
{: .fs-6 .fw-300 }

## Package Description

Laravel's `toSql()` method gives you sql query without bindings replaced. (see question marks below)
```php
\DB::table('users')->select('name')->where('id', 5)->toSql();

// select `name` from `users` where `id` = ? and `name` = ?
```

With this package you have `getSql()` method. Which gives you same result with bindings replaced.
```php
\DB::table('users')->select('name')->where('id', 5)->getSql();

// select `name` from `users` where `id` = 5 and `name` = 'laravel'
```

## Usage

Please see [README](https://github.com/laratoolbox/query-viewer) for details.
