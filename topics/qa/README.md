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