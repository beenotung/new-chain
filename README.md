## new-chain

Create chaining APIs from functions

## Install

```bash
$ npm install new-chain
```

## Usage

```js

Num(3).sum(10).sub(5).mul(2).val()
// => 16

function Num(x){

    var chain = newChain(sum, sub, mul)

    chain.val = val

    return chain

    function mul(n){
        x *= n
    }
    
    function sum(n){
        x += n
    }
    
    function sub(n){
        x -= n
    }
    
    function val(n){
        return x
    }

}


```

## Caveats

* Do not define functions with `var` statements. 

## Coded by [Machi](http://instagram.com/p/YcU60_kD0r/)

![](https://dl.dropboxusercontent.com/s/swyw3663x22pnwy/npmel_15.jpg)
