# 取代var的let&const

<code>

    let age = 24;
    agt +=1
    age = 22


    const finger = 10;
    fingers += 2 (錯誤 const不能re-assign)
    fingers = 9 (錯誤 const不能re-assign)

    const point = {x:3, y:2};
    point.x =3 (可以修改物件其中的值)
    point = { x:2, y:3}; (錯誤 const不能re-assign)

</code>

## 作用域
> scope 變數的有效範圍 
> #### 從外而內繼承
> - function scope 函式作用域
> - global scope  全域作用域
> #### 從內而外繼承
> block
> {大括號} 括起來的範圍就叫做block，除了物件

## var的作用範圍是 scope
## let/const的作用範圍是 block 
