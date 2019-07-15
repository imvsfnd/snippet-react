# Virtual DOM
## 組件裡組合起來的架構如下，稱之為Render Function, 將頁面上的資料(Model)透過以下組建的結構，把這一個頁面整個Render成實際DOM Tree結構
<code>
    
    <Chat /> --- <ChatList /> --- <CahtListItem />
                              --- <CahtListItem />
             --- <ChatInput />
             --- <ChatStatus />
</code>

> React把資料 (Model) 透過(Component Render Function) 專換成實際的(Dom Tree), 但其實React在(Component Render Function) 與 (Real Dom) 中間放入了一個(Virtual DOM)
- Model 
- Component Render Funciton 
- Virtual DOM 
- Real DOM

## Virtual DOM & MVVM的差異
### Virtual DOM
- 初始 render 快
- 大量更新快
- 容易實作Dom以外的Render, 如 React Native

### MVVM
- 小量更新快
- 要做若干優化, 大量更新才夠快
