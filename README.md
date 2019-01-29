## Table of Contents

[![Join the chat at https://gitter.im/js-live-template/Lobby](https://badges.gitter.im/js-live-template/Lobby.svg)](https://gitter.im/js-live-template/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

1. [Description](#description)
1. [Documentation](#documentation)
1. [Installation](#installation)

## Description

An extensive set of Javascript [live templates](https://www.jetbrains.com/help/idea/2016.1/live-templates.html) for use
in JetBrains IDEs. These live templates are based off of https://atom.io/packages/es6-javascript.

![](http://i.imgur.com/vH7X7xf.gif)

## Documentation

<table>
    <thead>
        <tr>
            <th>Live Template Short Hand</th>
            <th>Description</th>
            <th>Template </th>
        </tr>
    </thead>
    <tbody>
            <tr>
            <td> v </td>
            <td> Declarations: var statement </td>
            <td>
                <pre>
var $name$;                </pre>
            </td>
        </tr>
            <tr>
            <td> ve </td>
            <td> Declarations: var assignment </td>
            <td>
                <pre>
var $name$ = $value$;                </pre>
            </td>
        </tr>
            <tr>
            <td> l </td>
            <td> Declarations: let statement </td>
            <td>
                <pre>
let $name$;                </pre>
            </td>
        </tr>
            <tr>
            <td> le </td>
            <td> Declarations: let assignment </td>
            <td>
                <pre>
let $name$ = $value$;                </pre>
            </td>
        </tr>
            <tr>
            <td> co </td>
            <td> Declarations: const statement </td>
            <td>
                <pre>
const $name$;                </pre>
            </td>
        </tr>
            <tr>
            <td> coe </td>
            <td> Declarations: const assignment </td>
            <td>
                <pre>
const $name$ = $value$                </pre>
            </td>
        </tr>
            <tr>
            <td> cos </td>
            <td> Declarations: const symbol </td>
            <td>
                <pre>
const $name$ = Symbol(&#39;$name$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> if </td>
            <td> Flow Control: if statement </td>
            <td>
                <pre>
if ($condition$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> el </td>
            <td> Flow Control: else statement </td>
            <td>
                <pre>
else {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> ife </td>
            <td> Flow Control: if else statement </td>
            <td>
                <pre>
if ($condition1$) {
  $then1$
} else {
  $then2$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> ei </td>
            <td> Flow Control: else if statement </td>
            <td>
                <pre>
else if ($condition$) {
  $end$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> fl </td>
            <td> Flow Control: for loop </td>
            <td>
                <pre>
for (let $index$ = 0; $index$ &lt; $iterable$.length; $index$++) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> fi </td>
            <td> Flow Control: for in loop </td>
            <td>
                <pre>
for (let $key$ in $source$) {
  if ($source$.hasOwnProperty($key$)) {
    $END$ 
  }
}                </pre>
            </td>
        </tr>
            <tr>
            <td> fo </td>
            <td> Flow Control: for of loop (ES6) </td>
            <td>
                <pre>
for (let $key$ of $source$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> wl </td>
            <td> Flow Control: while loop </td>
            <td>
                <pre>
while ($condition$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> tc </td>
            <td> Flow Control: try/catch </td>
            <td>
                <pre>
try {
  $try_body$
} catch ($error$) {
  $catch_body$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> tf </td>
            <td> Flow Control: try/finally </td>
            <td>
                <pre>
try {
  $try_body$
} finally {
  $finally_body$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> tcf </td>
            <td> Flow Control: try/catch/finally </td>
            <td>
                <pre>
try {
  $try_body$
} catch ($error$) {
  $catch_body$
} finally {
  $finally_body$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> f </td>
            <td> Functions: anonymous function </td>
            <td>
                <pre>
function ($arguments$) { $END$ }                </pre>
            </td>
        </tr>
            <tr>
            <td> iife </td>
            <td> Functions: immediately-invoked function expression (IIFE) </td>
            <td>
                <pre>
(($arguments$) =&gt; {
  $function_body$
})($passed_arguments$);                </pre>
            </td>
        </tr>
            <tr>
            <td> fa </td>
            <td> Functions: function apply </td>
            <td>
                <pre>
$fn$.apply($context$, $arguments$);                </pre>
            </td>
        </tr>
            <tr>
            <td> fc </td>
            <td> Functions: function call </td>
            <td>
                <pre>
$fn$.call($context$, $arguments$);                </pre>
            </td>
        </tr>
            <tr>
            <td> fb </td>
            <td> Functions: function bind </td>
            <td>
                <pre>
$fn$.bind($context$, $arguments$);                </pre>
            </td>
        </tr>
            <tr>
            <td> af </td>
            <td> Functions: arrow function (ES6) </td>
            <td>
                <pre>
($arguments$) =&gt; $statement$                </pre>
            </td>
        </tr>
            <tr>
            <td> afb </td>
            <td> Functions: arrow function with body (ES6) </td>
            <td>
                <pre>
($arguments$) =&gt; {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> gf </td>
            <td> Functions: generator function (ES6) </td>
            <td>
                <pre>
function* ($arguments$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> gfn </td>
            <td> Functions: named generator function (ES6) </td>
            <td>
                <pre>
function* $name$ ($arguments$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> fe </td>
            <td> Iterables:  forEach loop (chainable) </td>
            <td>
                <pre>
$iterable$.forEach(($item$)) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> map </td>
            <td> Iterables: map function (chainable) </td>
            <td>
                <pre>
$iterable$.map(($item$)) =&gt; {
  return $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> reduce </td>
            <td> Iterables: reduce function (chainable) </td>
            <td>
                <pre>
$iterable$.reduce(($previous$, $current$) =&gt; {
  return $body$
}, $initial$);                </pre>
            </td>
        </tr>
            <tr>
            <td> filter </td>
            <td> Iterables: filter function (chainable) </td>
            <td>
                <pre>
$iterable$.filter(($item$) =&gt; {
  // return true to remove item from collection
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> find </td>
            <td> Iterables: ES6 find function (chainable) </td>
            <td>
                <pre>
$iterable$.find(($item$) =&gt; {
  // return true to find single item if it is in the collection
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> c </td>
            <td> Objects and classes: class (ES6) </td>
            <td>
                <pre>
class $name$ {
  constructor($arguments$) {
    $END$
  }
}                </pre>
            </td>
        </tr>
            <tr>
            <td> cex </td>
            <td> Objects and classes: child class (ES6 syntax) </td>
            <td>
                <pre>
class $name$ extends $base$ {
  constructor($arguments$) {
    super($arguments$);
    $END$
  }
}                </pre>
            </td>
        </tr>
            <tr>
            <td> cf </td>
            <td> Objects and classes: class function (ES6 syntax) </td>
            <td>
                <pre>
$fn_name$($arguments$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> kv </td>
            <td> Objects and classes: key/value pair </td>
            <td>
                <pre>
$key$: $value$                </pre>
            </td>
        </tr>
            <tr>
            <td> m </td>
            <td> Objects and classes: method (ES6 syntax) </td>
            <td>
                <pre>
$method$($arguments$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> set </td>
            <td> Objects and classes: setter (ES6 syntax) </td>
            <td>
                <pre>
set $property$($value$) {
  $END$
}                </pre>
            </td>
        </tr>
            <tr>
            <td> proto </td>
            <td> Objects and classes: prototype method (chainable) </td>
            <td>
                <pre>
$class$.prototype.$method_name$ = function ($arguments$) {
  $END$
};                </pre>
            </td>
        </tr>
            <tr>
            <td> r </td>
            <td> Returning values: return </td>
            <td>
                <pre>
return $value$;                </pre>
            </td>
        </tr>
            <tr>
            <td> rth </td>
            <td> Returning values: return this </td>
            <td>
                <pre>
return this;                </pre>
            </td>
        </tr>
            <tr>
            <td> rn </td>
            <td> Returning values: return null </td>
            <td>
                <pre>
return null;                </pre>
            </td>
        </tr>
            <tr>
            <td> rt </td>
            <td> Returning values: return true </td>
            <td>
                <pre>
return true;                </pre>
            </td>
        </tr>
            <tr>
            <td> rf </td>
            <td> Returning values: return false </td>
            <td>
                <pre>
return false;                </pre>
            </td>
        </tr>
            <tr>
            <td> r0 </td>
            <td> Returning values: return 0 </td>
            <td>
                <pre>
return 0;                </pre>
            </td>
        </tr>
            <tr>
            <td> r-1 </td>
            <td> Returning values: return -1 </td>
            <td>
                <pre>
return -1;                </pre>
            </td>
        </tr>
            <tr>
            <td> rp </td>
            <td> Returning values: return Promise (ES6) </td>
            <td>
                <pre>
return new Promise((resolve, reject) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> S </td>
            <td> Types: String </td>
            <td>
                <pre>
String                </pre>
            </td>
        </tr>
            <tr>
            <td> N </td>
            <td> Types: Number </td>
            <td>
                <pre>
Number                </pre>
            </td>
        </tr>
            <tr>
            <td> O </td>
            <td> Types: Object </td>
            <td>
                <pre>
Object                </pre>
            </td>
        </tr>
            <tr>
            <td> A </td>
            <td> Types: Array </td>
            <td>
                <pre>
Array                </pre>
            </td>
        </tr>
            <tr>
            <td> D </td>
            <td> Types: Date </td>
            <td>
                <pre>
Date                </pre>
            </td>
        </tr>
            <tr>
            <td> Rx </td>
            <td> Types: RegExp </td>
            <td>
                <pre>
RegExp                </pre>
            </td>
        </tr>
            <tr>
            <td> tof </td>
            <td> Types: typeof comparison </td>
            <td>
                <pre>
typeof $source$ === &#39;$type$&#39;;                </pre>
            </td>
        </tr>
            <tr>
            <td> iof </td>
            <td> Types: instanceof comparison </td>
            <td>
                <pre>
$source$ instanceof $object$                </pre>
            </td>
        </tr>
            <tr>
            <td> p </td>
            <td> Promises: new Promise (ES6) </td>
            <td>
                <pre>
new Promise((resolve, reject) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> then </td>
            <td> Promises: Promise.then (chainable) </td>
            <td>
                <pre>
$promise$.then(($value$) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> catch </td>
            <td> Promises: Promise.catch (chainable) </td>
            <td>
                <pre>
$promise$.catch(($err$) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> ex </td>
            <td> ES6 modules: module export </td>
            <td>
                <pre>
export $member$;                </pre>
            </td>
        </tr>
            <tr>
            <td> import </td>
            <td> ES6 modules: module import </td>
            <td>
                <pre>
import $END$ from &#39;$module$&#39;;                </pre>
            </td>
        </tr>
            <tr>
            <td> ima </td>
            <td> ES6 modules: module import as </td>
            <td>
                <pre>
import $exposed$ as $name$ from &#39;$module$&#39;;                </pre>
            </td>
        </tr>
            <tr>
            <td> imn </td>
            <td> ES6 modules: named module export </td>
            <td>
                <pre>
import { $name$ } from &#39;$module$&#39;;                </pre>
            </td>
        </tr>
            <tr>
            <td> desc </td>
            <td> BDD testing (Mocha, Jasmine, etc.): describe </td>
            <td>
                <pre>
describe(&#39;$description$&#39;, () =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> ita </td>
            <td> BDD testing (Mocha, Jasmine, etc.): asynchronous &#34;it&#34; </td>
            <td>
                <pre>
it(&#39;$description$&#39;, (done) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> bef </td>
            <td> BDD testing (Mocha, Jasmine, etc.): before </td>
            <td>
                <pre>
before(() =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> befe </td>
            <td> BDD testing (Mocha, Jasmine, etc.): before each </td>
            <td>
                <pre>
beforeEach(() =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> after </td>
            <td> BDD testing (Mocha, Jasmine, etc.): after </td>
            <td>
                <pre>
after(() =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> afte </td>
            <td> BDD testing (Mocha, Jasmine, etc.): after each </td>
            <td>
                <pre>
afterEach(() =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> cl </td>
            <td> Console: console.log </td>
            <td>
                <pre>
console.log(&#39;$title$&#39;, $value$);                </pre>
            </td>
        </tr>
            <tr>
            <td> cll </td>
            <td> Console: console.log (text only) </td>
            <td>
                <pre>
console.log($END$);                </pre>
            </td>
        </tr>
            <tr>
            <td> ce </td>
            <td> Console: console.error </td>
            <td>
                <pre>
console.error($END$);                </pre>
            </td>
        </tr>
            <tr>
            <td> cw </td>
            <td> Console: console.error </td>
            <td>
                <pre>
console.warn($END$);                </pre>
            </td>
        </tr>
            <tr>
            <td> st </td>
            <td> Timers: setTimeout </td>
            <td>
                <pre>
setTimeout(() =&gt; {
  $END$
}, $delay$);                </pre>
            </td>
        </tr>
            <tr>
            <td> si </td>
            <td> Timers: setInterval </td>
            <td>
                <pre>
setInterval(() =&gt; {
  $END$
}, $delay$);                </pre>
            </td>
        </tr>
            <tr>
            <td> sim </td>
            <td> Timers: setInterval </td>
            <td>
                <pre>
setImmediate(() =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> ae </td>
            <td> DOM specifics: addEventListener </td>
            <td>
                <pre>
$document$.addEventListener(&#39;$event$&#39;, function(e) {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> gi </td>
            <td> DOM specifics: getElementById </td>
            <td>
                <pre>
$document$.getElementById(&#39;$id$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> gc </td>
            <td> DOM specifics: getElementByClassName </td>
            <td>
                <pre>
Array.from($document$).getElementsByClassName(&#39;$class$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> gt </td>
            <td> DOM specifics: getElementByClassName </td>
            <td>
                <pre>
Array.from($document$).getElementsByTagName(&#39;$class$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> qs </td>
            <td> DOM specifics: querySelector </td>
            <td>
                <pre>
$document$.querySelector(&#39;$selector$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> qsa </td>
            <td> DOM specifics: querySelectorAll </td>
            <td>
                <pre>
$document$.querySelectorAll(&#39;$selector$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> cb </td>
            <td> Node.js specifics:  Node.js style callback </td>
            <td>
                <pre>
(error, $value$) =&gt; { $END$ }                </pre>
            </td>
        </tr>
            <tr>
            <td> re </td>
            <td> Node.js specifics:  require a module </td>
            <td>
                <pre>
require(&#39;$module$&#39;);                </pre>
            </td>
        </tr>
            <tr>
            <td> em </td>
            <td> Node.js specifics:  export member </td>
            <td>
                <pre>
exports.$name$ = $value$;                </pre>
            </td>
        </tr>
            <tr>
            <td> me </td>
            <td> Node.js specifics:  module.exports </td>
            <td>
                <pre>
module.exports = $name$;                </pre>
            </td>
        </tr>
            <tr>
            <td> on </td>
            <td> Node.js specifics:  attach an event handler (chainable) </td>
            <td>
                <pre>
$emitter$.on(&#39;$event$&#39;, $arguments$) =&gt; {
  $END$
});                </pre>
            </td>
        </tr>
            <tr>
            <td> us </td>
            <td> Miscellaneous: use strict </td>
            <td>
                <pre>
&#39;use strict&#39;;                </pre>
            </td>
        </tr>
            <tr>
            <td> fn </td>
            <td> Functions: named function </td>
            <td>
                <pre>
function $name$($arguments$) {
  $END$
}                </pre>
            </td>
        </tr>
    </tbody>
</table>

## Installation

### macOS

There are two ways to install:

#### Using settings.jar

1. File > Import Settings
1. Select the settings.jar file
1. Check Live templates in the Select Components to Import dialog
1. Click ok in the Select Components to Import dialog
1. Click ok when prompted to restart

#### Copying es6.xml

Put `es6.xml` inside of the following directory:

```bash
~/Library/Preferences/<intellij-product-install>/templates
```
