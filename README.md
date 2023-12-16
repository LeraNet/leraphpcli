# leraphpcli
A lightweight php library for your php cli needs. <br>
<br>
**Features :**
- ⌨️ Get user input! 
- 🎨 Have colorful text!

## get_input()
Pauses the php script and asks user for an input!
### Usage
1. Use get_input() function to ask for users input
```php
$input = get_input();
echo $input;
```

### Examples

Here are some examples of how to use the `get_input` function:

```php
echo "What is your name?";
$name = get_input();
echo "Welcome $name!";
```

## textColor
Helps you generate text styles that you can use later!
### Usage
1. Instantiate an object of the `textColor` class:

```php
//Get the user's name
echo "What is your name?";
$name = get_input();
```

2. Set the text color, background color, and text effect using the `__construct()` method:

```php
$textColor = new textColor('text color', 'background color', 'text type');
```

<details>
  <summary>All Text Colors</summary>
  <pre>black, 
red, 
green, 
yellow, 
blue, 
magenta, 
cyan, 
light gray, 
dark gray, 
light red, 
light green, 
light yellow, 
light blue, 
light magenta
light cyan
white</pre>
</details>

<details>
  <summary>All Background Colors</summary>
  <pre>black, 
red, 
green, 
yellow, 
blue, 
magenta, 
cyan, 
light gray, 
dark gray, 
light red, 
light green, 
light yellow, 
light blue, 
light magenta
light cyan
white</pre>
</details>

<details>
  <summary>All Text Types</summary>
  <pre>bold,
dim,
underlined,
blink,
reverse,
hidden</pre>
</details>
3. Use the `getColoredString()` method to colorize a string:

```php
$string = $textColor->getColoredString('Hello, world!');
echo $string;
```

### Examples

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
- lera2od

