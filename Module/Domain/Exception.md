##Runtime Exception

There should not be many exceptions but, you can catalog them in a single class filled with Messages and Codes

```
namespace Tollwerk\Module\Domain\Exception;

use Tollwerk\Module\Domain\Contract\ModuleExceptionInterface;

class RuntimeException extends \RuntimeException implements ModuleExceptionInterface
{
    /**
     * Undefined method
     * @var int
     */
    public const METHOD_UNDEFINED = 1234;
    /**
     * Undefined method
     * @var string
     */
    public const METHOD_UNDEFINED_STR = 'Undefined method "%s"';
}
```
