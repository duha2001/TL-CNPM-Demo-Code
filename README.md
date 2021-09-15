#CÁCH CÀI ĐẶT MÔI TRƯỜNG VÀ CHẠY VÍ DỤ "HELLO WORLD"

1. Đầu tiên các bạn cần cài đặt [Node.js](https://nodejs.org/en/) để tạo môi trường chạy React, việc cài đặt rất đơn giản và nhanh chóng.
2. Tạo 1 folder để chứa project React, vào trong folder đè shift nhấn chuột phải và chọn như hình.
![image](https://user-images.githubusercontent.com/59979503/133368284-f439ef1e-1a7f-42c5-ab93-5db56b051a46.png)
3. Tiếp theo gõ các dòng lệnh sau để tạo project
```ruby
npm install -g create-react-app
```
```ruby
create-react-app my-app
```
_NPM sẽ tự động tạo cho ta 1 project tên là my-app và install các module và lib cần thiết cho chúng ta._

4. Vào thư mục src xóa hết các file trong đây, lưu ý không xóa cả thư src mà chỉ xóa các file ở trong đó.
5. Sau đó tạo mới 2 file **Index.js** và **App.jsx**.

Trong **App.jsx** các bạn code như sau: import React from 'react'
```ruby
class App extends React.Component {
   render() {
      return (
         <div>
            Hello World!!!
         </div>
      );
   }
}
export default App;
```
Đây là React component đầu tiên của chúng ta, chúng ta sẽ tìm hiểu component là gì ở các bài sau, component này là App sẽ render Hello World ra màn hình. Tiếp theo trong **index.js** ta code:
```ruby
import React from 'react';
import ReactDOM from 'react-dom';
import App from './App.jsx';

ReactDOM.render(<App />, document.getElementById('root'));
```
6. Running the Server:
```ruby
cd my-app
```
```ruby
npm start
```
Và chúng ta có được sản phẩm React đầu tiên. Chúc mọi người học tốt.
![Screen Shot 2021-09-15 at 10 23 33](https://user-images.githubusercontent.com/59979503/133369366-5ceae325-9844-4924-89df-019011b5b6d0.png)
