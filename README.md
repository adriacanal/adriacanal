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
    
    public function getCurrentKnowledge(): array
    {
        return [
            Php::class,
            Laravel::class,
            TailwindCss::class,
            AlpineJs::class,
            Livewire::class
        ];
    }
    
    
    
    public function getInTouch():void
    {
        Mail::to('hello@adriacanal.dev')->send(new ContactMail());
    }
    
}

```
