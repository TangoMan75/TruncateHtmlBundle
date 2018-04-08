Tangoman TruncateHtml Twig Service
==================================

**Tangoman TruncateHtml Twig Service** truncates html keeping tags.

How to install
--------------

With composer

```console
$ composer require tangoman/truncate-html-bundle
```

Enable the bundle
-----------------

Don't forget to enable the bundle in the kernel:

```php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new TangoMan\TruncateHtml\TangoManTruncateHtml(),
    );
}
```

You don't have to add **TangoMan CallbackBundle** to the `service.yml` of your project.
**twig.extension.truncate_html** service should load automatically.

How to use
----------

Inside your views:

```twig
    <p>
        {{ post.html|truncatehtml }}
    </p>
```

Note
====

If you find any bug please report here : [Issues](https://github.com/TangoMan75/TruncateHtml/issues/new)

License
=======

Copyright (c) 2018 Matthias Morin

[![License][license-MIT]][license-url]
Distributed under the MIT license.

If you like **TangoMan TruncateHtml** please star!
And follow me on GitHub: [TangoMan75](https://github.com/TangoMan75)
... And check my other cool projects.

[tangoman.free.fr](http://tangoman.free.fr)

[license-MIT]: https://img.shields.io/badge/Licence-MIT-green.svg
[license-url]: LICENSE
