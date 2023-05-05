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
$red = new textColor('red', 'yellow', 'bold');
$string = $red->getColoredString('Hello, world!');
echo $string;

// Print "Success" in green text
$success = new textColor('green');
$string = $success->getColoredString('Success');
echo $string;

// Print "Warning" in yellow text
$warning = new textColor('yellow');
$string = $warning->getColoredString('Warning');
echo $string;

// Print "Error" in red text
$error = new textColor('red');
$string = $error->getColoredString('Error');
echo $string;
```

## Credits
there is no credits
