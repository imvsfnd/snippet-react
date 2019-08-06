# 物件導向 CLASS
## ES6 版本開始才有

<code>

    class Dog extends Animal {
        constructor(){
            this.age = 0;
            addEventListen."click",this.bark=,this
            this.bark=this.bark.bind("this")
        }
        bark(){
            console.log(this.age);
        }
    }
    const spot = new Dog();
    spot.age
    this
</code>

method (function) = 函式
property (variable) = 物件的變數

* 可以安裝套件 babel class-properties, 改成箭頭函式的寫法
* 那麼這時候，箭頭函式會將this綁定在這個 new出來的物件身上
* 若是一般函式，就要看他怎麼執行而定
  
<code>

    class Dog extends Animal {
        age = 0;
        bark = () => console.log('woof');
        }
    }
    const spot = new Dog();

</code>