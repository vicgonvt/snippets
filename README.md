# Sublime Text - Snippets

These are the snippets that I use in all of my installations of Sublime Text. Geared towards the person workin with Laravel and its environment.

# Installation

To install the snippets in your sublime, you will have to clone this repo into your own computer(s).

In your terminal, run the following command

```sh
cd Library/Application\ Support/Sublime\ Text\ 3/Packages/User/
git clone git@github.com:vicgonvt/snippets.git
```

This will create a directory called `snippets` which will contain all of the snippets. 

That's it! It's that easy.

Contributions and suggestions welcomed!!!


# What's in the box

## PHP Class Methods

#### Public Method
+ Shortcut: `met`

```php
public function [METHOD_NAME]()
{
    //
}
```

#### Private Method
+ Shortcut: `pmet`

```php
private function [METHOD_NAME]()
{
    //
}
```

#### Protected Method
+ Shortcut: `prmet`

```php
protected function [METHOD_NAME]()
{
    //
}
```

#### Public Static Method
+ Shortcut: `smet`

```php
public static function [METHOD_NAME]()
{
    //
}
```

#### Construct Method
+ Shortcut: `cmet`

```php
public function __construct()
{
    //
}
```

## PHP Helpers

#### Die & Dump
+ Shortcut: `dd`
For those of us that use Laravel, dd() is missed when working outside the framework. Here is a workaround.

```php
die(var_dump($[VAR]));
```

## Laravel Views

#### Blade Variable Echo

Quick helper for outputting variables in blade templates.

```php
{{ $var }}
```

## Laravel Relationships

Laravel relationships are easy to write and now they take a second or two. Big thank you to Adam Wathan for the original idea on these. Modified a little bit for my personal preference. I mostly label my relationships to make sense regardless of my model's name. There is a stop at the method name, a second, optional, stop for the model's name and in some cases another stop to specify the table's field name.

#### BelongsTo
+ Shortcut: `belt`

```php
public function relationship()
{
    return $this->belongsTo(Relationship::class, 'field_name');
}
```

#### BelongsToMany
+ Shortcut: `belm`

```php
public function relationship()
{
    return $this->belongsToMany(Relationship::class, 'field_name');
}
```

#### HasMany
+ Shortcut: `hasm`

```php
public function relationship()
{
    return $this->hasMany(Relationship::class, 'field_name');
}
```

#### HasOne
+ Shortcut: `haso`

```php
public function relationship()
{
    return $this->hasOne(Relationship::class);
}
```

### PHPUnit

#### Test Method

Quick helper for scaffolding a new test method.

```php
public function testName()
{
    //
}
```
