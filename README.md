# LibraryGridSys

## Thư viện Responsive với Grid System

**Cách để sử dụng thư viện Grid System**

Ta chỉ cần thêm class có các thuộc tính tương ứng vào các thẻ theo nguyên tắc

_Ví dụ:_
```
 <div class="grid wide container">
     <div class="row">
        <!-- Ví dụ ở đây muốn hiện thị 4 khóa học trên 1 chiều ngang
             Thì mặc định là 12 col mình chia cho 4 là bằng 3 thì mình
            chọn l-3 cho giao diện PC -->
         <div class="col l-3 m-6 c-6">
            <div class="course-item">
                   <h1>Course 1</h1>
             </div>
         </div>
```
**Nguyên tắc khi sử dụng thư viện**

_Luôn để link css của thư viện lên trên_
_Phải reset css và box-sizing: border-box_

- Class grid luôn là class bắt buộc khi bắt đầu hệ thống. Nó chính là lưới(thường là phần cha, chứa Row và Column)
- Sau class grid là class row chính là dòng(Dòng - chiều ngang, chứa Column)
- Sau class row là class column(ở thư viện đặt là col) chính là cột(chứa nội dung/ thành phần trên website)
  - Ngoài ra, còn có class wide: chiều ngang tối đa 1200px

**Vai trò của các class**

- Row có vai trò:
  - Chứa các columns, giúp các columns nằm theo chiều ngang
  - Khi tổng chiều ngàng columns vượt quá kích thước Row, cho column xuống hàng
  - Loại bỏ khoảng thừa do gutters tạo ra ở 2 phía
- Column có vài trò:
  - Chứa các thành phần trên website

**Column offset**

Là các class có o ở giữa ví dụ như: .c-o-1, m-o-2, l-o-5,...

Column offset có tác dụng đưa column chứa class đó đến vị trí mong muốn. Ví dụ: class m-o-2 sẽ đưa column đến cột thứ 2

**Ý nghĩa của các class bắt đầu bằng c, m, l**

- Class bắt đầu bằng c thì sẽ được dùng cho thiết bị mobile
- Class bắt đầu bằng m thì sẽ được dùng cho thiết bị Tablet
- Class bắt đầu bằng l thì sẽ được dùng cho thiết bị PC