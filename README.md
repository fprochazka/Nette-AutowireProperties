# Autowire Properties experiment for Nette Framework

**You shouldn't be using this, if you don't know what youre doing!**

discussion: http://forum.nette.org/cs/13084-presentery-property-lazy-autowire-na-steroidech#p93574


## Include in application


```php
abstract class BasePresenter extends Nette\Application\UI\Presenter
{
	use \Kdyby\AutowireProperties;

}
```


## Usage


```php
class ArticlePresenter extends BasePresenter
{
    /**
     * @autowire
     * @var App\ArticleRepository
     */
    protected $articleRepository;

    // ..
}
```
