FPDF for use with Symfony2
==========================

Uses FPDF 1.7, tested in Symfony 2.5

Setup
-----

Execute the command below:

composer require "royopa/fpdf-symfony2"

Please provide a version constraint for the royopa/fpdf-symfony2 requirement: 

enter dev-master

And those to `app/autoload.php`:


```php
$classMap = array(
    'Fpdf_' => __DIR__.'/../vendor/royopa/fpdf-symfony2/lib/FPDF/FPDF.php',
    'Fpdi_' => __DIR__.'/../vendor/royopa/fpdf-symfony2/lib/FPDF/FPDI.php'
);
$loader->addClassMap($classMap);    
```

Usage
-----

```php
  $pdf  = new \FPDF_FPDF();
  $pdi  = new \FPDF_FPDI();	
```

FPDF
-----
FPDF is a PHP class which allows to generate PDF files with pure PHP, that is to say without using the PDFlib library. FPDF is a open source project: you may use it for any kind of usage and modify it to suit your needs.

- http://www.fpdf.org/

On the fpdf homepage you will find links to the documenation, forums and so on.
