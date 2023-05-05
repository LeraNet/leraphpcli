# leraphpcli

This PHP script allows you to colorize terminal output with different text colors, background colors, and text effects.

## Usage

1. Instantiate an object of the `textColor` class:

```php
$textColor = new textColor();
```

2. Set the text color, background color, and text effect using the `__construct()` method:

```php
$textColor = new textColor('red', 'yellow', 'bold');
```

3. Use the `getColoredString()` method to colorize a string:

```php
$string = $textColor->getColoredString('Hello, world!');
echo $string;
```

## Examples

Here are some examples of how to use the `textColor` class:

```php
// Print "Hello, world!" in red text on a yellow background with bold text effect
$textColor = new textColor('red', 'yellow', 'bold');
$string = $textColor->getColoredString('Hello, world!');
echo $string;

// Print "Success" in green text
$textColor = new textColor('green');
$string = $textColor->getColoredString('Success');
echo $string;

// Print "Warning" in yellow text
$textColor = new textColor('yellow');
$string = $textColor->getColoredString('Warning');
echo $string;

// Print "Error" in red text
$textColor = new textColor('red');
$string = $textColor->getColoredString('Error');
echo $string;
```

## Credits

This script is based on the work of [Martin Angelov](https://tutorialzine.com/2013/10/terminal-in-php-via-sockets) and [zbrox](https://gist.github.com/zbrox/2948808).
