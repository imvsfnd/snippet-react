# import 與 export
## ES6 版本開始才有

<code>

    // math.js

    const math = {
        double: x => x*2,
        square: x=> x*x,
        area: (w,h)=> w*h
    };

    // NAMED EXPORT
    export const PI = 3.1415;
    export const ROOT_2 = 1.414;

    // EXPORT DEFAULT
    export default math;
</code>
<code>

    // main.js
    
    //NAMEED IMPORT
    import { PI,ROOT_2} from './math';
    
    //IMPORT DEFAULT
    import math from './math';

    console.log(math.square(11));
</code>
<code>

    //兩種IMPORT方式可以混用寫成如下
    import math, {PI, ROOT_2} from './math';

    console.log(PI, ROOT_2);
    console.log(math.square(11));
</code>
<code>

    //可以重新命名IMPORT
    import m, {PI as P, ROOT_2 as RT} from './math';

    console.log(P, RT);
    console.log(m.square(11));    
</code>