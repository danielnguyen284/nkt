# Phụ lục PL06b - Cơ chế thị trường chứng khoán Việt Nam và sản phẩm tài chính (phần 2) (phần ngoài đầu tư)

> Trích từ [PL06b-thi-truong-chung-khoan-viet-nam-va-san-pham.md](../../bo-kien-thuc/phu-luc/PL06b-thi-truong-chung-khoan-viet-nam-va-san-pham.md) trong Bộ kiến thức NKT. Các mục dưới đây nói về kênh tài sản khác chứng khoán (tiền số, forex) nên đã chuyển sang folder này.

## Danh sách mục

1. NFT và đất ảo metaverse (Decentraland, The Sandbox)
2. Tiền mã hoá và blockchain: kỹ thuật cơ bản, cú sốc chính sách Trung Quốc, hawala và rửa tiền
3. Tiền số ngân hàng trung ương (CBDC, e-CNY, đô la số)

### NFT và đất ảo metaverse (Decentraland, The Sandbox)

**Thầy nhắc ở:** B6 00:55 - thầy nhắc như ví dụ của niềm tin ảo.

**Là gì:** NFT (non-fungible token) là mã định danh duy nhất ghi trên blockchain để chứng nhận quyền sở hữu một tệp số hoặc tài sản số, không thể thay thế qua lại như tiền mã hoá thông thường. "Đất ảo" là các ô đất trong thế giới ảo (Decentraland, The Sandbox) được bán dưới dạng NFT.

**Giải thích:**

- Cơ chế khan hiếm: khan hiếm nằm ở token, không ở tệp; ai cũng có thể sao chép hình ảnh, và NFT không tự động mang theo bản quyền. Tệp thường nằm ngoài chuỗi, token chỉ trỏ tới một địa chỉ web nên có thể hỏng liên kết. Một tác phẩm có thể có nhiều NFT cùng trỏ tới tệp giống nhau.
- Decentraland: bản đồ ban đầu có 90.601 ô đất (số lượng cố định do giao thức quy định, theo suy luận từ nguồn), mua bằng token MANA trên Ethereum. Khi ra mắt năm 2017, ô đất bán khoảng 20 USD; tháng 4/2021 trong đợt sốt NFT, ô đất bán 6.000 đến 100.000 USD; tháng 11/2021 một công ty mua một ô giá 2,43 triệu USD. Tháng 10/2022 DappRadar ghi nhận dưới 1.000 người dùng mỗi ngày có giao dịch tiền (có hôm chỉ 38), trong khi phía nền tảng nói trung bình 8.000 người dùng mỗi ngày tính theo ví blockchain.
- The Sandbox: tôi chưa mở được nguồn tốt cho số ô đất, giá và diễn biến. Từ khoá gợi ý: "The Sandbox LAND 166,464 supply", "The Sandbox LAND price 2022".
- Bùng nổ rồi sụp: giao dịch NFT tăng từ khoảng 82 triệu USD (2020) lên khoảng 17 tỷ USD (2021) theo nguồn trích trong Wikipedia; tác phẩm của Beeple bán 69 triệu USD tại Christie's tháng 3/2021. Đến tháng 5/2022 doanh số hằng ngày giảm 92% so với tháng 9/2021 và số ví hoạt động giảm 88% so với tháng 11/2021; một báo cáo tháng 9/2023 nói 95% NFT đã về giá trị bằng không (nguồn là một trang cờ bạc tiền mã hoá, cần cẩn trọng).
- Rủi ro: wash trading (tự mua bán bằng nhiều ví để tạo doanh số giả), gian lận mạo danh nghệ sĩ, rug pull (dự án thổi giá, bán hết rồi bỏ).

**Liên hệ với bài học:** Thầy dùng NFT và đất ảo như ví dụ giá dựa vào niềm tin. Nên phân biệt: cơ chế khan hiếm là thật, nhưng giá trị sử dụng và dòng tiền đứng sau thì không đảm bảo, và quá trình sụp 2022 đã kiểm chứng điều đó.

**Đọc thêm:** [Non-fungible token (Wikipedia)](https://en.wikipedia.org/wiki/Non-fungible_token); [Decentraland (Wikipedia)](https://en.wikipedia.org/wiki/Decentraland); [Wash trade (Wikipedia)](https://en.wikipedia.org/wiki/Wash_trade)

### Tiền mã hoá và blockchain: kỹ thuật cơ bản, cú sốc chính sách Trung Quốc, hawala và rửa tiền

**Thầy nhắc ở:** B6 00:57, B6 01:05, B6 01:07, B6 01:08 - thầy nhắc khi bàn cú sốc chính sách và rủi ro tiền số: mã hoá khoá công khai, chuỗi khối, Trung Quốc cấm đào năm 2021, rò rỉ dữ liệu người dùng, hawala.

**Là gì:** Tiền mã hoá là tài sản số dùng mật mã để bảo vệ giao dịch và vận hành trên mạng ngang hàng thay vì ngân hàng trung ương. Blockchain là danh sách các khối giao dịch nối với nhau, mỗi khối chứa mã băm của khối trước, nên sửa khối cũ đòi hỏi làm lại mọi khối sau đó.

**Giải thích:**

- Kỹ thuật cơ bản (theo mô tả Bitcoin): mỗi người có một khoá riêng và địa chỉ sinh ra từ khoá công khai tương ứng; giao dịch được ký bằng khoá riêng và mạng xác thực bằng khoá công khai. Mất khoá riêng là mất quyền truy cập, lộ khoá riêng có thể bị mất tiền. Khối mới tạo ra khoảng 10 phút một lần; thợ đào tìm một số nonce sao cho mã băm thấp hơn ngưỡng độ khó (bằng chứng công việc), khó tạo nhưng dễ kiểm tra.
- Trung Quốc: tháng 12/2013 Ngân hàng Nhân dân Trung Quốc cấm tổ chức tài chính dùng bitcoin và giá giảm sau thông báo; năm 2018 (theo Wikipedia) giá sụt sau lệnh cấm giao dịch toàn diện; tỷ trọng giao dịch bitcoin bằng nhân dân tệ giảm từ trên 90% (9/2017) xuống dưới 1% (6/2018). Đợt cấm đào và giao dịch năm 2021: tôi không mở được nguồn cho các mốc tháng và mức giảm giá; Wikipedia ghi cuối 2025 Trung Quốc vẫn chiếm 14% thị phần đào toàn cầu dù đã cấm năm 2021 và hiện Mỹ có thị phần pool đào lớn nhất. Từ khoá kiểm tra: "China bans crypto mining 2021 hash rate bitcoin price".
- Rò rỉ dữ liệu khoảng 17 GB: chưa tìm được nguồn đáng tin, không thể xác định tên dự án; từ khoá gợi ý: "rò rỉ 17GB dữ liệu người dùng tiền mã hoá".
- Hawala: hệ thống chuyển tiền phi chính thức dựa trên lòng tin giữa các "hawaladar". Người gửi đưa tiền cho một môi giới ở thành phố A kèm mật khẩu; môi giới này liên lạc với môi giới ở thành phố B, người nhận đọc mật khẩu và nhận tiền (trừ phí nhỏ). Hai môi giới thanh toán nợ với nhau sau, có thể bằng hàng hoá hoặc dịch vụ chứ không nhất thiết bằng tiền. Sau 11/9/2001, các cơ quan chống rửa tiền chú ý vì hệ thống này ẩn danh và thiếu giám sát.
- Việt Nam: theo hiểu biết của tôi (chưa đối chiếu nguồn trong lần tra cứu này, cần kiểm tra), tiền mã hoá không được công nhận là phương tiện thanh toán nhưng gần đây đã có khung pháp lý về tài sản số và cơ chế thí điểm thị trường; từ khoá: "Nghị quyết 05/2025/NQ-CP thí điểm thị trường tài sản mã hoá", "Luật Công nghiệp công nghệ số tài sản số".

**Liên hệ với bài học:** Thầy dùng tiền mã hoá làm ví dụ về cú sốc chính sách (một quyết định hành chính đổi giá trị tài sản trong vài ngày) và về rủi ro tài sản phi tập trung. Phụ lục không đánh giá giá trị đầu tư của loại tài sản này.

**Đọc thêm:** [Bitcoin (Wikipedia)](https://en.wikipedia.org/wiki/Bitcoin); [Bitcoin mining (Wikipedia)](https://en.wikipedia.org/wiki/Bitcoin_mining); [Hawala (Wikipedia)](https://en.wikipedia.org/wiki/Hawala)

### Tiền số ngân hàng trung ương (CBDC, e-CNY, đô la số)

**Thầy nhắc ở:** B6 01:04 - câu hỏi học viên.

**Là gì:** CBDC (central bank digital currency) là dạng số của tiền pháp định do ngân hàng trung ương phát hành, là nghĩa vụ nợ của ngân hàng trung ương giống như tiền mặt. Khác tiền mã hoá như Bitcoin ở chỗ có nhà nước phát hành và quản lý tập trung, không cần blockchain.

**Giải thích:**

- Khác tiền gửi ngân hàng: tiền gửi là nợ của ngân hàng thương mại, còn CBDC là nợ trực tiếp của ngân hàng trung ương. Rủi ro đáng bàn là người dân chuyển tiền từ ngân hàng sang CBDC, làm yếu nguồn vốn của ngân hàng; Wikipedia dẫn nghiên cứu của Ngân hàng Trung ương Anh cho rằng thiết kế phù hợp có thể xử lý rủi ro này.
- e-CNY (nhân dân tệ số): ngân hàng trung ương Trung Quốc bắt đầu nghiên cứu từ 2014, được mô tả là CBDC đầu tiên do một nền kinh tế lớn phát hành; ở thí điểm Thâm Quyến, phiếu có hạn dùng và 90% được tiêu ở cửa hàng.
- Đô la số: Wikipedia nêu nước Mỹ vẫn tranh luận; một đạo luật thông qua tháng 6/2026 (mục 1101 của "21st Century ROAD to Housing Act") cấm Cục Dự trữ Liên bang phát hành tài sản số công chúng là nghĩa vụ trực tiếp của Fed. Euro số: ECB chuyển sang giai đoạn chuẩn bị từ 10/2023.
- Tình trạng toàn cầu theo Wikipedia (số liệu giữa các phần lệch nhau): 9 nước cùng 8 đảo của Liên minh Tiền tệ Đông Caribe đã phát hành (ví dụ Bahamas "Sand Dollar", Nigeria e-Naira), 38 nước và Hồng Kông đang thí điểm, 67 nước và 2 liên minh tiền tệ đang nghiên cứu.

**Liên hệ với bài học:** Học viên hỏi để phân biệt tiền số của nhà nước với tiền mã hoá; điểm khác chính là bên phát hành và tính tập trung.

**Đọc thêm:** [Central bank digital currency (Wikipedia)](https://en.wikipedia.org/wiki/Central_bank_digital_currency)
