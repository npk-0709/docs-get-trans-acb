Hướng Dẫn Sử Dụng API
POST: https://apikey.phukhuong79.com/libs/transACB.php
API này cho phép bạn lấy thông tin các giao dịch từ tài khoản của bạn.

Tham Số Yêu Cầu
Khi gửi yêu cầu POST đến API, bạn cần cung cấp các tham số sau:

username: Tên đăng nhập của bạn.
password: Mật khẩu của bạn.
account: Số tài khoản mà bạn muốn truy vấn.
row: Số lượng giao dịch mà bạn muốn lấy.

Định Dạng Phản Hồi
Phản hồi từ API sẽ là một đối tượng JSON chứa danh sách các giao dịch. Mỗi giao dịch bao gồm các thông tin sau:

ID: ID của giao dịch.
AMOUNT: Số tiền giao dịch.
TYPE: Loại giao dịch, có thể là "IN" (vào) hoặc "OUT" (ra).
DESCRIPTION: Mô tả của giao dịch.
CURRENCY: Đơn vị tiền tệ của giao dịch.
DATE: Ngày thực hiện giao dịch.
[
    {
        "ID": "123456789",
        "AMOUNT": 500000,
        "TYPE": "IN",
        "DESCRIPTION": "Salary payment",
        "CURRENCY": "VND",
        "DATE": "2024-06-13T10:00:00Z"
    },
    {
        "ID": "987654321",
        "AMOUNT": 200000,
        "TYPE": "OUT",
        "DESCRIPTION": "Electricity bill",
        "CURRENCY": "VND",
        "DATE": "2024-06-12T15:30:00Z"
    }
]
