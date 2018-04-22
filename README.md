
**Kích hoạt tài khoản**
----
  Kết quả trả về định dạng Json

* **URL**

  /create

* **Phương thức:**

  `POST`
  
*  **Tham số đầu vào**

   **Bắt buộc:**
 
   `project=[integer]  Giá trị: 2. Kế hoạch giáo dục cũ, 3. Quản lý mầm non`
   `unit=[string]  Mã đơn vị của tài khoản kích hoạt`
   `limit=[integer]  Số ngày hoạt động. Giá trị: 3, 7, 30, 90, 180, 365 ngày`
   `user=[string]  Tài khoản muốn được kích hoạt`
   `admin=[string]  Tài khoản quản trị thực hiện thao tác tạo tài khoản - tài khoản đang đăng nhập`

* **Thành công:**

  * **Code:** 200 <br />
    **Content:** `{"status":true,"inserted":1}`
 
* **Lỗi thiếu tham số đầu vào:**

  * **Code:** 200 <br />
    **Content:** `{"status":false,"messages":["Tham số sai"]}`

  HOẶC

  * **Code:** 200 <br />
    **Content:** `{"status":false,"messages":["Không thành công"]}`

------------------------
<br/>
<br/>
<br/>


**Kiểm tra tài khoản**
----
  Kết quả trả về định dạng Json

* **URL**

  /check

* **Phương thức:**

  `POST`
  
*  **Tham số đầu vào**

   **Bắt buộc:**
 
   `project=[integer]  Giá trị: 2. Kế hoạch giáo dục cũ, 3. Quản lý mầm non`
   `username=[string]  Tài khoản muốn kiểm tra`

* **Thành công:**

  * **Code:** 200 <br />
    **Content:** `{"status":"1","username":"admin","expired":"2018-05-19 00:00:00","email":"khgd@vietec.com.vn","license":"KHGDIKMwqz************************************"}`
 
* **Lỗi thiếu tham số đầu vào:**

  * **Code:** 200 <br />
    **Content:** `{"status":false,"messages":["Tham số sai"]}`

  HOẶC

  * **Code:** 200 <br />
    **Content:** `{"status":false,"messages":["Tài khoản không hợp lệ"]}`

------------------------
<br/>
<br/>
<br/>
