# Arrow Function 箭頭函式
## 一般函式與箭頭函式

### 一般函式
<code>

    function double(x){
        return x * 2;
    }

    var double = function(x){
        return x * 2;
    }
</code>

### 箭頭函式
- 把一般函式中的function移除，並在 ( ) 後加入 => 
- 
<code>

    const double = (x) => {
        return x * 2;
    }
</code>

- 簡寫的規則：當函式只有一個參數的時候，可以省略兩邊的小括號。**只有在一個參數的時候可以省略**
- 
<code>

    const double = x => {
        return x * 2;
    }
</code>

- 簡寫的規則：當函式只有一行，而且是return一個值的時候，可以省略大括號還有return關鍵字，直接把要return的關鍵字接在箭頭後面。
- 
<code>

    const double = x =>  x * 2;
</code>

- 一般函式與箭頭函在This上的差異
> 動作與情境會影響This所代表的意義

> 箭頭函式沒有自己的情境，所以取決於宣告時的情境就等於箭頭函式中的This情境所代表的對象

## 一般函式的This上的差異
- 以下這個函式的內容是固定的，但這個this是代表什麼，就要看這個函式是怎樣的去執行而定
  
<code>

    function jump(){
        console.log(this);
    }
</code>

> Javascript函示執行，基本上可以分為三種 
- *直接執行* > this = global || window
- 
<code>

    function jump(){
        console.log(this);
    }
    jump();  //Output Window
</code>
> -  *作為物件的方式去執行* > this = 這個物件
<code>

    function jump(){
        console.log(this);
    }
    
    const a = {};
    a.jump = jump;
    a.jump();  //Output 是一個物件，裡面剛好有一個jump, 他就是這個a
</code>

> -  *作為DOM的偵聽函示執行* > this = 這個DOM
<code>

    function jump(){
        console.log(this);
    }
    
    btn.addEventListener('click',jump)  //Output 是一個物件，裡面剛好有一個jump, 他就是這個a
</code>

## 箭頭函式的This
<code>

    const jump = () =>{
        console.log(this);
    }
    const a = {}
    a.jump = jump;
    a.jump()
    
    //Output window
</code>