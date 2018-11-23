# Ruby Style Guide
Ruby (on Rails) Style Guide for Sleekr Engineering.

## Use Rails Default Convention
In order to make our new engineer easy to onboard and make application maintenance easy, always follow Rails Default Convention.
For Example, Rails directory structure always follow <https://guides.rubyonrails.org/getting_started.html#creating-the-blog-application>

## Follow Rubocop, Rubycritic, and Brakeman If Possible
When Rubocop, Rubycritic, and Brakeman raise compalaints, don't disable it, but fix your code first if possible.

## Use Concern if Possible
When you want to make controller / model cleaner, put your code to Concern.

## Extend With Service Object and Lib
Put extended modules for Sleekr application in app/services if it's relate our MVC and put in lib directory for seeder, generator and tasks.

## Use Form Object when Our Form Does Not Have Table
Because we need to use model everywhere and make our new engineer easy to develop application, always put validation and logic our data inside model or model/concerns.
Only use Form object if we need to build form, but without database table.

## Helper if possible, use Presenter or Decorator if we need it.
If your view has logic, move to helper. If it's to complex you can use presenter or decorator.
