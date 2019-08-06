# Nodejs與npm與webpack
### 如果不想依賴瀏覽器的JS環境，想要在本機端執行就需要安裝Node.js
[Nodejs](https://nodejs.org/en/)
[npm](https://www.npmjs.com/)

> node.js的權限比瀏覽器還高，可以讀取電腦的檔案系統，在瀏覽器中使用別人的程式會用到cdn，在node.js中，則需要npm的幫忙
> npm = node package manager，可以幫我們從npm下載需要的程式並且安裝起來，放在node_modules資料夾中
> webpack 在我們要發佈時，需要一個工具幫我們把檔案轉成瀏覽器看得懂的格式，這時候就需要webpack，這是一個在node.js底下運行的程式，可以使用npm安裝它，只要我們寫好它的設定，它就會幫我們把各模組做組合，轉換語法，最後生成一個檔案讓使用者讀取

* node -v 
  > v8.12.0
* npm install -S react
  > +react@6.6.0
* npm install -S webpack
  > 
