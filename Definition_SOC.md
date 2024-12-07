# auth.log
Tệp `auth.log` ghi lại cả lần đăng nhập thành công và thất bại, hành động sudo và su cũng như các quy trình liên quan đến xác thực khác. Trên hệ thống Debian/Ubuntu, nhật ký này được lưu trữ tại `/var/log/auth.log`, trong khi trên hệ thống RedHat/CentOS, nó được lưu trữ tại `/var/log/secure`. 

# wtmp
## Define
Tệp wtmp là một trong ba tệp được sử dụng để ghi nhật ký các sự kiện đăng nhập và đăng xuất trên hệ thống Linux:

- `/var/run/utmp`: Theo dõi người dùng hiện đang đăng nhập.
- `/var/log/wtmp`: Lưu giữ bản ghi lịch sử về các sự kiện đăng nhập và đăng xuất.
- `/var/log/btmp`: Ghi lại những lần đăng nhập không thành công.

## View file
File này là định dạng binary nên phải dùng tool mới đọc được

![image](https://hackmd.io/_uploads/HJduoXzEyl.png)

- For btmp, the `who` (or w) command will display its contents.
- The `last` command can be used to view wtmp.
- The `lastb` command is for examining btmp.
