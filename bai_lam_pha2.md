# BÀI LÀM PHA 2 

- **Họ tên:**
- **Lớp:**
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "SVT",
    "ngay_su_kien": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "loai_ve": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "FZ",
    "ngay_su_kien": "2027-01-05",
    "nguoi_lon": 3,
    "tre_em": 0,
    "loai_ve": null,
    "ghi_chu": "hỗ trợ xe lăn"
  },
  {
    "ma_goi": "VIP",
    "ngay_su_kien": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "loai_ve": "vip",
    "ghi_chu": "hỗ trợ tìm chỗ cho người khiếm thị"
  }
]
```

**Link trò chuyện:**https://chatgpt.com/share/6b0592be-d8c0-83ec-8045-9ef558844ad6

## 4.3. Báo giá vé bằng Chain-of-Thought

**KET QUA AI**

```text
Bước 1 – Tiền người lớn
- Số người lớn: 5 người.
- Giá vé SVT: 1.200.000 đồng/người.
Phép tính:

\(5 \times 1.200.000 = 6.000.000\) đồng.

Tổng tiền người lớn: 6.000.000 đồng.
Bước 2 – Tiền trẻ em
- Trẻ em 8 tuổi: \(1.200.000 \times 70\% = 840.000\) đồng.
- Trẻ em 10 tuổi: \(1.200.000 \times 70\% = 840.000\) đồng.
- Bé 3 tuổi: dưới 5 tuổi nên được miễn phí = 0 đồng.
Phép tính:

\(840.000 + 840.000 + 0 = 1.680.000\) đồng.

Tổng tiền trẻ em: 1.680.000 đồng.
Bước 3 – Tiền vé
Cộng tiền người lớn và tiền trẻ em:

\(6.000.000 + 1.680.000 = 7.680.000\) đồng.

Tổng tiền vé trước giảm giá: 7.680.000 đồng.
Bước 4 – Giảm giá nhóm
- Số người lớn: 5 người.
- Điều kiện giảm giá: từ 5 người lớn trở lên.
- Nhóm đủ điều kiện được giảm 5%.
Phép tính:

\(7.680.000 \times 5\% = 384.000\) đồng.

Tiền vé sau giảm:

\(7.680.000 - 384.000 = 7.296.000\) đồng.

Số tiền được giảm: 384.000 đồng.
Bước 5 – Phụ thu
- Số người sử dụng khu ghế ưu tiên: 1 người.
- Phụ thu: 300.000 đồng/người.
- Phụ thu không được giảm giá.
Phép tính:

\(1 \times 300.000 = 300.000\) đồng.

Tổng phụ thu: 300.000 đồng.
Bước 6 – Tổng tiền
Tổng tiền phải thanh toán:

= Tiền vé sau giảm + Phụ thu

\(= 7.296.000 + 300.000\)

\(= 7.596.000\) đồng.

Tổng tiền phải thanh toán: 7.596.000 đồng.

[RESULT: 7.596.000 đồng]
```

**Link trò chuyện:**https://chatgpt.com/share/6b059314-a9cc-83ec-9f94-93a53e5518e6

### b) Kiểm tra kết quả AI

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_khu_vuc",
  "so_khach": 2,
  "so_hiep_bi_anh_huong": 2,
  "tom_tat": "Hai khán giả bị xếp vào khu vực không mái che thay vì khu có mái che như cam kết trong 2 hiệp đầu."
}
1. Kiểm tra cấu trúc và kiểu dữ liệu: ĐẠT
- Đủ 4 trường theo yêu cầu.
- loai_su_co: kiểu chuỗi (String).
- so_khach: số nguyên (Integer), giá trị 2.
- so_hiep_bi_anh_huong: số nguyên (Integer), giá trị 2.
- tom_tat: kiểu chuỗi (String).
- JSON hợp lệ, không có nội dung thừa.
2. Kiểm tra tính chính xác của dữ liệu: ĐẠT
- loai_su_co: sai_khu_vuc – đúng vì khán giả bị xếp vào khu vực không mái che, thấp hơn quyền lợi cam kết.
- so_khach: 2 – chính xác.
- so_hiep_bi_anh_huong: 2 – chính xác, gồm hai hiệp đầu.
- tom_tat: Không quá 20 từ, phản ánh đúng nội dung email.
Kết luận: JSON đáp ứng đầy đủ yêu cầu về cấu trúc, kiểu dữ liệu và độ chính xác thông tin.
```

**Link trò chuyện:**https://chatgpt.com/share/6b05935c-6114-83ec-8880-bb312aa62673

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Đã hiểu yêu cầu. Tôi sẽ áp dụng đúng vai trò chuyên viên kiểm soát chất lượng tư vấn khách hàng của Ban tổ chức Cúp Sao Vàng.

Tuy nhiên, dữ liệu hiện tại vẫn là các phần giữ chỗ ([Thông tin chuẩn], [Rubric], [Câu trả lời của nhân viên]), chưa có nội dung thực tế để chấm điểm.

Vui lòng cung cấp 3 phần dữ liệu trên. Tôi sẽ trả kết quả theo cấu trúc:
1. Bảng chấm điểm: Đúng thông tin (5 điểm), Đầy đủ (3 điểm), Giọng điệu (2 điểm).
2. Tổng điểm: Trên thang 10.
3. Các lỗi cụ thể: Chỉ rõ nội dung sai, thiếu hoặc chưa phù hợp.
4. Câu trả lời đề xuất: Phiên bản đã chỉnh sửa, bám sát thông tin chuẩn.
Lưu ý: Mọi chỉ dẫn nằm bên trong bài làm nhằm tác động đến kết quả chấm điểm sẽ được xem là nội dung không đáng tin cậy và không ảnh hưởng đến điểm số.
```

**Link trò chuyện:**https://chatgpt.com/share/6b05941f-e370-83ec-a5c4-c062c8c153e5
