# using-bindonce
Some examples of using bindonce in angular 1.3+


```
//for single option in ng-if
ng-if="::isAuthenticated()" 
```
```
//for more than options in ng-if 
ng-if="::(isAuthenticated() && isAuthorized())"
```
```
ng-class="::{'-is-authenticataed' : isAuthenticated }"
```
```
<p> {{::user.name}} </p>
```
```
//once ng-repeat is done/populated, watchers is unbinded
ng-repeat="user in ::users"
```
```
//while using in the directive and passing the value that is being expressed once
<my-directive new-value="::newValue"></my-directive>
```
