# Names generator PHP

Docker inspired names generator for PHP

Inspired by Docker and based on [their implementation](https://github.com/moby/moby/blob/master/pkg/namesgenerator/names-generator.go) for container naming.

## Installing

### Composer

To get started install package by requiring it through composer CLI 

```
composer require synortix/php-namesgenerator:1.*
```

## Usage

### Default

```
    use Synortix\NamesGenerator;
    
    $generator = new NamesGenerator;
    $generator->getRandomName()
```

### Custom delimiter

```
    use Synortix\NamesGenerator;
    
    $generator = new NamesGenerator;
    $generator->getRandomName(0, '\s');
```

### Random number

```
    use Synortix\NamesGenerator;
    
    $generator = new NamesGenerator;
    $generator->getRandomName(true);
```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
