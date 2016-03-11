# Twig for CodeIgniter 3

## Description
This is a simple library that enables you to use the power of Twig templating engine in your CodeIgniter project.

## Requirements
- [CodeIgniter 3] (https://www.codeigniter.com/)
- [Twig] (https://github.com/twigphp/Twig)

## Installation

1. Place **TwigLoader.php** into the 'libraries' folder of your CodeIgniter project *(usually application/libraries)*
2. In **Controller.php** in system/core folder find the following line: `$this->load =& load_class('Loader', 'core');`
3. Replace it with `$this->load =& load_class('TwigLoader', 'libraries');`
4. Done!

### Note
By default the 'twig' file extension is used, so you must name your view files as *filename.twig*. You can change the file extension by passing the third argument to *load_class* method (e.g. `$this->load =& load_class('TwigLoader', 'libraries', 'php');`