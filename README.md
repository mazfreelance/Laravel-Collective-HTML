# Laravel-Collective-HTML

How to use code HTML in Laravel like on below: 
<code>
{!! Form::open(['route' => 'posts.store']) !!}
{!! Form::label('title', 'Title:') !!}
{!! Form::text('title', null, array('class' => 'form-control')) !!}
{!! Form::close() !!}
</code>


You can do it in laravel 5.5 too. Step 1: Install from Command: composer require "laravelcollective/html":"^5.5"

Step 2: After install you have to add providers and aliases in config/app.php file, so let' follow bellow file how to add.
 
<code>
<?php

'providers' => [

    // ...

    Collective\Html\HtmlServiceProvider::class,

    // ...

  ],

'aliases' => [

    // ...

      'Form' => Collective\Html\FormFacade::class,

      'Html' => Collective\Html\HtmlFacade::class,

    // ...

  ],
</code>
Step 3: After added above providers, you have to check on your project.

Step 4: Done.

Thanks.
