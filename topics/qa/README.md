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