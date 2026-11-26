# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 08
- **Họ tên:**Lê Quang Hào
- **Lớp:**CNTT1
- **Link repository Pha2:**https://github.com/phanthithuy012008-dot/CNTT1_PromptAI_H02_Pha1/blob/main/bai_lam_pha2.md
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**chatgpt

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt lịch khám ra JSON

**KET QUA AI**

```text
[
  {
    "ma_dich_vu": "TRAM",
    "ngay_hen": "2026-12-17",
    "nguoi_lon": 2,
    "tre_em": 1,
    "khung_gio": "chieu",
    "ghi_chu": null
  },
  {
    "ma_dich_vu": "CAOVOI",
    "ngay_hen": "2027-01-06",
    "nguoi_lon": 3,
    "tre_em": 0,
    "khung_gio": null,
    "ghi_chu": "1 người bị tiểu đường"
  },
  {
    "ma_dich_vu": "TAYTRANG",
    "ngay_hen": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "khung_gio": "sang",
    "ghi_chu": "1 người dị ứng thuốc tê"
  }
]
```

**Link trò chuyện:**https://chatgpt.com/share/6b07e5b8-a0a8-83ec-94fa-28fe651a4ec4


## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Bước 1: Tiền người lớn

6 người lớn × 350.000 = 2.100.000 đồng

Bước 2: Tiền trẻ em
- Trẻ 7 tuổi: 350.000 × 80% = 280.000 đồng.
- Trẻ 11 tuổi: 350.000 × 80% = 280.000 đồng.
- Bé 4 tuổi: Miễn phí = 0 đồng.
Tổng tiền trẻ em = 280.000 + 280.000 + 0 = 560.000 đồng.

Bước 3: Tiền vé = người lớn + trẻ em

2.100.000 + 560.000 = 2.660.000 đồng.

Bước 4: Giảm giá nhóm

Nhóm có 6 người lớn (đủ điều kiện từ 5 người lớn trở lên).

2.660.000 × 10% = 266.000 đồng.

Tiền dịch vụ sau giảm:

2.660.000 − 266.000 = 2.394.000 đồng.

Bước 5: Phụ thu chụp X-quang (không giảm giá)

3 phim × 150.000 = 450.000 đồng.

Bước 6: Tổng tiền

2.394.000 + 450.000 = 2.844.000 đồng.

[RESULT: 2.844.000 đồng]
```

**Link trò chuyện:**https://chatgpt.com/share/6b07e68a-5a8c-83ec-ac75-9ae9a34a1de7
### b) Kiểm tra kết quả AI


## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "tre_hen",
  "so_khach": 3,
  "so_hiep_bi_anh_huong": 2,
  "tom_tat": "3 khách phải chờ hơn 1 tiếng trong cả 2 lần hẹn; không phàn nàn về bác sĩ."
}

```

**Link trò chuyện:**https://chatgpt.com/share/6b07e72e-2120-83ec-98c2-b170017b618b

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Tiêu chí	Điểm	Minh chứng	Đề xuất sửa
Đúng thông tin (50%)	1/5	Sai giá: "Trám răng bên em 450k/răng thôi" trong khi giá chuẩn là 500.000 đồng/răng. Sai chính sách: "Bong sau 8 tháng thì em làm lại free cho anh nha." Vì tháng thứ 8 thuộc giai đoạn tháng 7–12, chỉ được giảm 50%, không được miễn phí.	Sửa thành: "Dịch vụ trám răng thẩm mỹ có giá 500.000 đồng/răng. Nếu miếng trám bong sau 8 tháng, anh được giảm 50% chi phí khi làm lại."
Đầy đủ (30%)	1/3	"Cần gì cứ inbox em ạ!" Chưa trả lời chính xác quyền lợi bảo hành và chưa mời khách cung cấp ngày thực hiện dịch vụ, số lượng răng cần trám để hỗ trợ đặt lịch.	Sửa thành: "Anh vui lòng cho em biết ngày muốn đến nha khoa và số lượng răng cần trám để bên em hỗ trợ đặt lịch ạ."
Giọng điệu (20%)	1/2	"450k/răng thôi, đẹp như răng thật luôn." Cách diễn đạt mang tính suồng sã, từ "free" và "inbox" chưa phù hợp với phong cách tư vấn chuyên nghiệp.	Sửa thành: "Dạ, Nha khoa Nụ Cười xin thông tin đến anh về dịch vụ trám răng thẩm mỹ. Rất mong được hỗ trợ anh ạ."
Tổng điểm	3/10	Nhân viên cung cấp sai giá, sai chính sách bảo hành và chưa đáp ứng đầy đủ yêu cầu tư vấn.	Cần sửa lại thông tin giá, chính sách bảo hành và cách tư vấn khách hàng.
```

**Link trò chuyện:**https://chatgpt.com/share/6b07e789-2024-83ec-abb5-fe94ddd0af40
