# Laravel-Collective-HTML

How to use code HTML in Laravel like on below: <br/><br/>
<code>
{!! Form::open(['route' => 'posts.store']) !!}
{!! Form::label('title', 'Title:') !!}
{!! Form::text('title', null, array('class' => 'form-control')) !!}
{!! Form::close() !!}
</code>


You can do it in laravel 5.5 in above.
<br/>
<strong>Step 1</strong>: Install from Command: composer require "laravelcollective/html":"^5.5"

<strong>Step 2</strong>: After install you have to add providers and aliases in config/app.php file, so let' follow bellow file how to add.
 
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
<br/><br/>
<strong>Step 3</strong>: After added above providers, you have to check on your project.

<strong>Step 4</strong>: Done.

Thanks.
