Prompt 1:
Tôi mới tìm hiểu về Git&HTML, hôm nay tôi đã bắt đầu sử dụng thẻ <fieldset>,...Tôi có bài toán sau: Đại lý vé máy bay SkyWay đang trong quá trình chuyển đổi số. Trước đây, nhân viên ghi chép thông tin khách hàng và lịch bay bằng sổ tay, dẫn đến việc thường xuyên nhập sai thông tin và khó tra cứu. Bộ phận Backend đã xây dựng xong hệ thống nhận dữ liệu, nhưng giao diện hiển thị (Frontend) do một thực tập sinh cũ làm lại quá sơ sài: Biểu mẫu thiếu các ràng buộc (khách hàng không nhập tên vẫn cho gửi, nhập sai định dạng email), còn bảng lịch bay thì lộn xộn, không phân định rõ tiêu đề và thân bảng.
Bạn hãy đóng vai trò là người dùng không rành công nghệ. Dựa trên các thuộc tính validation mặc định của HTML5 (như required, type=email, min, max, accept), hãy đưa ra 3 kịch bản nhập liệu sai phổ biến để tôi tự test xem form HTML thuần của tôi đã đủ sức chặn họ lại chưa?
Đây là code của tôi:
<h2>Đặt vé máy bay</h2>
<form method ="post">
    <fieldset>
        <legend> Thông tin đặt vé</legend>
        <label for="name">Tên: </label>
        <input type="text" name="name" id="name" required><br>
        <label for="sdt">Số điện thoại: </label>
        <input type="tel" name="sdt" id="sdt" required><br>
        <label for="email">Email: </label>
        <input type="email" name="email" id="email" required><br>
        <label for="ngaybay">Ngày bay: </label>
        <input type="date" name="ngaybay" id="ngaybay" required><br>
        Hạng ghế:
        <select name="cabin" id="cabin">
            <option value="hn">Hạng nhất</option>
            <option value="tg">Thương gia</option>
            <option value="ptdb">Phổ thông đặc biệt</option>
            <option value="pt">Phổ thông</option>
        </select>
    </fieldset>
    <button type="submit">Gửi Hồ Sơ</button>
</form>
<br><hr><br>

<h2>Lịch bay hôm nay</h2>
<table border="1">
    <thead>
    <tr>
        <td>Mã chuyến</td>
        <td>Hành trình</td>
        <td>Giờ bay</td>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>VN123</td>
        <td>Hà Nội - TP.HCM</td>
        <td>08:00</td>
    </tr>
    <tr>
        <td>VJ456</td>
        <td colspan="2">Hà Nội - Đà Nẵng (ĐÃ HỦY)</td>
    </tr>
    </tbody>
</table>

Prompt 2:
Tôi đã tối ưu lại code của mình, bạn hãy đóng vai trò là một khách hàng để trải nghiệm lại quá trình đặt vé nhé.