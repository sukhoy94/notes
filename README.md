# notes

multiple forms - each field should has different ids


# symfony

https://stackoverflow.com/questions/12998060/check-if-in-dev-mode-inside-a-controller-with-symfony

```
# app/config/services.yml
services:
    _defaults:
        autowire: true

    App\Controller\SomeController:
        arguments: ['%kernel.environment%']
        
        
        
namespace App\Controller;

final class SomeController
{
    /**
     * @var string
     */
    private $environment;

    public function __construct(string $environment)
    {
        $this->environment = $environment;
    }

    public function someAction()
    {
        $this->environment...
        // any operations you need
    }
}        
```


https://stackoverflow.com/questions/39841390/get-getenvironment-from-a-service


# useful links

- css to sass converter https://css2sass.herokuapp.com/
