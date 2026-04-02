```php

<?php

namespace AdriaCanal;

class About extends Me
{
    public static array $PRONOUNS = ['He', 'Him'];
    
    public function getCurrentWorkplace(): array
    {
        return [
            'workplace' => [
                'company' => 'GNA Hotel Solutions',
                'position' => 'Backend Developer'
            ]
        ];
    }

    public function currentlyLearning(): array
    {
        return [
            'AWS',
            'Systems Architecture',
            'CI/CD Pipelines',
        ];
    }
    
    public function getStack(): array
    {
        return [
            'backend'  => [Php::class, Laravel::class],
            'frontend' => [TailwindCss::class, Livewire::class],
            'tooling'  => [Docker::class],
        ];
    }

    public function offCode(): array
    {
        return ['Father of two 👶👶', 'Vegan 🌱'];
    }
    
    public function getInTouch():void
    {
        Mail::to('hola@adriacanal.com')->send(new ContactMail());
    }
    
}

```
