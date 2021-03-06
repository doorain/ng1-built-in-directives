# Goal
Only show each red tooltip when the associated input box is focused/selected. See what you can come up with on your own before looking at the hints/solution below.

![Result](http://i.giphy.com/LWpxizi6xanja.gif)

## Directives You Might Use
| Name | Description |
| ---- | ----------- |
|`ng-blur`| Specify an expression to evaluate when an element loses focus |
|`ng-focus`| Specify and expression to evaluate when an element is focused |
|`ng-show`| If the expression is truthy then the element is shown or hidden respectively |
|`ng-hide`| If the expression is truthy then the element is shown or hidden respectively |

Basic examples of these directives have been included. If running these with live-server, run `live-server <name-of-file>`.

## Hint #1
Choose a variable for each input box and set this to true/false on blur/focus. 

## Hint #2
Show/hide the tooltips based on the variables you set to true/false. 

## Solution
```html
<div>
    User Name: <input class="form-control" type="text" ng-focus="userName=true" ng-blur="userName=false">
    <span style="color:red" ng-show="userName">Input your User name</span><br />
    Password: <input class="form-control" type="text" ng-focus="password=true" ng-blur="password=false">
    <span style="color:red" ng-show="password">Input your Password</span>
</div>
```

