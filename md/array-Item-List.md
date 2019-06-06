#### 把陣列ren成元素

<code>
index.js

    import React from 'react'
    import ReactDOM from 'react-dom'
    import List from './List'

    ReactDOM.render(<List />, document.getElementById('root'));

</code>

<code>
Item.js

    import React, { Component } from 'react'

    export default class Item extends Component {
    render() {
        return (
        <div>
            <li>{this.props.children}</li>
        </div>
        )
    }
    }

</code>

<code>
List.js

    import React, { Component } from 'react'
    import Item from './Item'

    const steps = [
        'Learn Javascript',
        'Learn CSS',
        'Learn React',
        'Learn pastell',
    ];
    class List extends Component {

        render() {
            return (
                <div>
                    {steps.map(text => <Item>{text}</Item>)}
                </div>
            )
        }
    }

    export default List


</code>

##### Reference 把陣列ren成元素  https://hiskio.com/courses/215/lectures/9128
