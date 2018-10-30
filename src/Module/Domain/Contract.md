##Contract Interfaces

In PHP you define an interface to define the skeletal structure of your classes. 
```
namespace Tollwerk\Module\Domain\Contract;

interface ControllerInterface
{
    public function exampleMethod(string $param);
}
```
Only when your project grows to a large application, will you need to organize the files in relation to their submodule. 

For example:
```
`-- src
    `-- <Module> 
        |-- Application
           |- Contract
        |-- Domain
           |- Contract
        |-- Infrastructure
           |- Contract
        |-- Ports
           |- Contract
        
```

But to start, you can throw all your interfaces in this directory.
