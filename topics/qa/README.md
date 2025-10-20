## MẪU QA

---
### Dạng không có data dẫn đến lỗi

> About this issue, we would like to confirm the following point.
>
> According to the design document, when the BFF login calls the login API but SQL001 of the API returns no data, the system will return a 404 error.
> Therefore, please prepare the necessary data and test again.
> 
> If the error still occurs, please provide us with the account and data you used so that we can investigate it.
> Thanks.

### Dạng cần quyền truy cập

> About this issue, we would like to confirm the following point.
> 
> According to the UI design document, to access this screen, the account needs to have both `univ_admission_passing` and `univ_preview`.  
> However, the account you provided does not have the `univ_preview` permissions.
> 
> Therefore, please prepare an account with the required permissions and test again.
> If the error still occurs, please provide us with the account and data you used so that we can investigate it.
> 
> Thanks.

Ngữ pháp mới:
> provide + someone + with + something

Nó có nghĩa là "cung cấp cho ai đó cái gì"

### Dạng xác nhận lỗi là đúng và cần sửa tài liệu

> About this issue, we would like to confirm the following point.
> 
> If the SQL001 query is missing `A.del_flg` and `B.del_flg`, the logically deleted data will be retuned.  
> Please confirm this point. If this is true, please update the design document and notify us once it is completed. 

Dạng câu bị động tương lai đơn (S + will be + V3/ed)

> the logically deleted data will be retuned.

Dạng bị động hiện tại đơn.
> Please notify us once it is completed.

### Dạng SQL trả về 1 vài field là null.

> About this issue, we would like to confirm the following point.
> 
> When calling the [get_general_info] API and executing SQL001, it returns two fields a and b, with null values.  
> Therefore, no data is displayed.
> 
> Please prepare the data and test again.

Return 1 field.
> When calling the [get_general_info] API and executing SQL001, it returns the field examId with a null value.  
> Therefore, the button is not displayed.

Nhiều field và cần liệt kê:
> When calling the [get_general_info] API and executing SQL001, the following fields are returned with null values:
> - examId
> - applicationId
> 
> Therefore, no data is displayed.

Ngữ pháp: rút gọn mệnh đề trạng ngữ
> Before: When you call the [get_general_info] API and execute SQL001.  
> After: When calling the [get_general_info] API and executing SQL001

When + V<sub>ing</sub>, S + V

### Dạng đã được trả lời ở 1 ticket khác và cần refer tới.
> This issue has already been addressed/fixed/confirmed/tested in ticket #123.  
> Please confirm.

Thì HTHT: S + has/have + been + V<sub>3/ed</sub> ...  
Dùng vì ticket đã xử lý nhưng vẫn còn liên quan tới hiện tại.

### Thiết kế selectOne nhưng data lại trả về nhiều row.

> About this issue, we would like to confirm the following point.
> 
> According to the design document of [general_info] API, the SQL001 query should return one record.  
> However, the current data returns multiple records, which causes an error.  
> Please confirm it.

### Dạng nếu thì, ngược lại thì.

> According to the design document, if the [Condition 1] is met, perform the split, if the [Condition 2] is not met, do not perform the split.  
> How should the other cases be handled?

> According to the design document, if the [Condition 1] is met, perform the split, if the [Condition 2] is not met, do not perform the split.  
> How should the cases below be handled?

> According to the design document:
> - If the [Condition 1] is correct, set `a = 1`.
> - If the [Condition 2] is correct, set `a = 3`.
> 
> What value should `a` have in the other cases?

### Hai câu SQL ra cùng 1 kết quả.

> We have tested the SQL001 and SQL002, and the data returned are almost the same.
> Please check.

### Bị thay đổi, nhưng tài liệu chưa thay đổi.

> According to ticket #123, it seems you changed the `function_code` from `univ_passing` to `univ_passing_status`.  
> However, according to the [general_detail] API, it still uses value `univ_passing`, which causes an error.  
> 
> Please check.

### Sai format.

> According to the design document of general_detail API, it returns a JSON value obtained from SQL001.  
> However, the JSON data stored in the database has an incorrect format (it does not include the key JP).  
> Therefore, the above error occurs.  
> 
> Please check.

### Cần vài field non-null.

> About this issue, we would like to the following point.
> 
> According to the UI design document, the BFF parent_001 must return two fields, userId and cognitoSub, as non-null values.  
> These two fields are obtained from SQL001 of the general_detail API.
> However, SQL001 returned no data, which caused the above error.
> 
> Please prepare the data and test again.

Câu gốc 2

According to the UI design document, the BFF a must return two fields, a and b, as non-null values.

Cấu trúc / thì: “must return” = modal + V (base form) → modal verb (must) biểu thị quy định / requirement / obligation ở hiện tại.

Tại sao dùng: câu này nêu quy tắc / đặc tả trong thiết kế (design doc). Quy tắc thường dùng present simple (hoặc modal) để diễn tả điều nên/thực tế phải xảy ra. “Must” nhấn mạnh đây là bắt buộc theo thiết kế.

Ghi chú: nếu muốn văn phong nhẹ nhàng hơn có thể dùng “should return” (recommendation), nhưng “must” phù hợp khi thiết kế bắt buộc.

Câu gốc 3

These two fields are obtained from SQL001 of the general_detail API.

Cấu trúc / thì: Present simple passive (“are obtained”) — động từ bị động ở hiện tại đơn.

Tại sao dùng: câu này nói một sự thật hiện tại / cách hệ thống hoạt động: giá trị của hai field lấy từ SQL001. Vì chủ thể (SQL001) là nguồn dữ liệu, ta dùng dạng bị động để nhấn vào “two fields” (đối tượng) chứ không nhấn vào ai/thứ lấy dữ liệu. Present simple phù hợp cho habitual fact / design fact (điều luôn đúng).

Ghi chú: có thể đổi thành active: “SQL001 returns these two fields.” — cũng đúng, nhưng passive hợp với style QA vì nhấn vào fields.

Câu gốc 4

However, SQL001 returned no data, which caused the above error.

Cấu trúc / thì: Past simple (“returned”, “caused”) + relative clause “which caused…”.

Tại sao dùng: đây mô tả sự kiện cụ thể đã xảy ra trong quá trình test (lần test/kiểm tra vừa rồi), tức là một hành động trong quá khứ → dùng past simple. “Which caused the above error” nối kết kết quả trực tiếp của hành động quá khứ.

Ghi chú: nếu muốn nhấn tính liên tục đến hiện tại (ví dụ SQL vẫn chưa trả data đến giờ), có thể dùng present perfect: “SQL001 has returned no data, which has caused the above error” — nhưng thông thường trong QA khi báo một kết quả test cụ thể, dùng past simple cho rõ ràng.

Câu gốc 5

Please prepare the required data and test again.

Cấu trúc / thì: Imperative (mệnh lệnh / đề nghị) bằng present simple.

Tại sao dùng: đây là yêu cầu/đề nghị hành động hướng tới người nhận — cấu trúc tiêu chuẩn là động từ nguyên thể đứng đầu (Please + V). Ngắn gọn, rõ ràng và lịch sự.

Ghi chú: có thể thêm “If the error persists, please provide …” để yêu cầu tiếp theo nếu vẫn có lỗi.

Tổng kết ngắn gọn — khi nào chọn dạng nào

Quy định / thiết kế → present (simple) hoặc modal (“must/should”) để diễn tả yêu cầu hiện tại.

Sự thật hệ thống / source of truth → present simple (thường passive nếu muốn nhấn vào dữ liệu).

Sự kiện test cụ thể đã xảy ra → past simple.

Yêu cầu / chỉ thị → imperative (Please + V).

Muốn lịch sự → “would like” thay cho “want”; “please” trước động từ cho mệnh lệnh lịch sự.

### 