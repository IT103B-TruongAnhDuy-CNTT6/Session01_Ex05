109800

**Phân tích lỗi & Lập bảng Test Cases (trình bày trong **`<strong>README.md</strong>`**):**

- Giải thích chi tiết tại sao biểu thức `rawBaseDeliveryFee + rawDeliveryDistance * 4000` lại sinh ra chuỗi `"1600012800"` thay vì con số `28800`.

Vì biến`rawBaseDeliveryFee` là kiểu dữ liệu chuỗi có giá trị là 16800.

Vì biến `rawDeliveryDistance` là chuỗi \* 4000 (number) => number = 12800

- Lập bảng 02 Test Cases đối chứng gồm các cột: `Trường hợp kiểm thử`, `Dữ liệu đầu vào`, `Kết quả sai thực tế`, `Kết quả đúng mong đợi`.

- [ ] | `Trường hợp kiểm thử`         | `Dữ liệu đầu vào`               | `Kết quả sai thực tế` | `Kết quả đúng mong đợi` |
      | ----------------------------- | ------------------------------- | --------------------- | ----------------------- |
      | Tính cước vận chuyển          | `rawBaseDeliveryFee` => string  | 1600012800            | 28800                   |
      | Quyết toán hóa đơn thanh toán | `rawDeliveryDistance` => string | 810001600012800       | 109800                  |
