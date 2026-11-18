# Phân tích kỹ thuật

> Thuộc Bộ kiến thức NKT. Tổng hợp từ các buổi: B1, B2, B3, B4, B7, B9, B10, B11, B12, B13, B14, B15, B17. Nên đọc cùng: [Dòng tiền, bảng điện và hành vi tay to](07-dong-tien-bang-dien-va-hanh-vi-tay-to.md), [Binh pháp 36 kế](08-binh-phap-36-ke.md), [Tâm lý đầu tư](09-tam-ly-dau-tu.md), [Quy trình đầu tư và chọn cổ phiếu](11-quy-trinh-dau-tu-va-chon-co-phieu.md), [Chu kỳ kinh tế và chỉ báo](01a-chu-ky-kinh-te-va-chi-bao.md).

## Mục lục

1. Bức tranh lớn
2. Phân tích kỹ thuật ghi nhận gì và trả lời câu hỏi nào
3. Nến Nhật và OHLC
4. Khối lượng và quan hệ giá - khối lượng
5. Xu hướng, kênh giá, hỗ trợ, kháng cự, nền giá và tích luỹ
6. Đường trung bình và các chỉ báo thông dụng
7. Mẫu hình giá và giới hạn của chúng
8. Chu kỳ giá và thời gian
9. Fibonacci: nguồn gốc, tỷ lệ vàng và cách dùng như phép đo
10. Sóng Elliott
11. Độ rộng thị trường, luân chuyển ngành và đối chiếu liên thị trường
12. Beta, hồi quy, kiểm thử và giới hạn của mô hình chuỗi thời gian
13. Thuật toán lọc, bảng tín hiệu scan và phần mềm
14. Thực hành đọc biểu đồ qua các ví dụ trong lớp
15. Cách luyện tập
16. Thứ tự kết hợp phân tích cơ bản với phân tích kỹ thuật
17. Quy trình áp dụng
18. Sai lầm thường gặp
19. Bối cảnh lúc ghi hình
20. Câu hỏi tự kiểm tra
21. Liên quan

## 1. Bức tranh lớn

1. Theo thầy, đáp án gọn nhất cho câu hỏi "phân tích kỹ thuật (TA) phản ánh cái gì" là **tâm lý của thị trường** (thầy chấm 10 điểm). TA ghi lại dấu vết cảm xúc và hành động của mọi người tham gia, cả người hiểu lẫn người không hiểu phân tích cơ bản (FA). Giá là tâm lý. (B4 02:34; B9 02:06)
2. Sách định nghĩa TA là nhìn quá khứ để dự báo giá tương lai. Thầy phản bác: không có dự báo máy móc nào đứng vững; thứ duy nhất đọc được là trạng thái tâm lý và ý đồ của bên dẫn giá, cùng tâm lý của đám nhỏ lẻ đu theo. (B9 02:07-02:10)
3. Phải đọc giá cùng khối lượng. Không thể nói "giá không", phải có volume; theo thầy khối lượng đi trước và quan trọng hơn giá, giá là thứ được dùng để tác động tâm lý nhà đầu tư. (B10 00:21; B13 02:16)
4. Chỉ báo, giao cắt, mẫu hình chỉ là "biến số". Cái khó là dịch biến số ra "thế trận": cung cầu đang đánh nhau ra sao, ai có lợi ích, vì sao lúc này có người sẵn sàng mua hoặc bán. Thầy gọi đó là "tâm pháp" của TA: đọc vị, đọc thế. (B10 00:23-00:25)
5. Mẫu hình phổ biến vừa là thứ đám đông tin, vừa là thứ bên làm giá có thể vẽ ra để dẫn dắt. Cái gì đám đông cùng tin thì đó là chỗ dễ bị "dắt mũi". Theo thầy, tên mẫu hình chỉ là tên gọi, phải học đọc tâm lý chứ không học thuộc tên hình. (B9 01:46-02:12; B10 00:47; B15 00:03)
6. Theo thầy, "sóng gì thì sóng, sóng không quan trọng bằng chu kỳ". Mỗi chu kỳ là một trận đánh. Hai thứ nên nắm: vòng chu kỳ và cách vận dụng Fibonacci (cả trên trục giá lẫn trục thời gian). (B10 00:45, 00:52)
7. Fibonacci chỉ là phép đo để ước vùng, không phải để bắt một điểm. Kết quả phụ thuộc hoàn toàn vào việc chọn đầu mút đoạn đo, và đầu mút chỉ chọn đúng khi đã đoán được người tạo giá đang ở đâu trong quy trình đè, gom, đẩy, xả. (B10 00:53, 02:05-02:09)
8. Cạm bẫy lớn nhất của người học sóng: bám vào sóng nhỏ, thiếu tầm nhìn tổng thể, chỉ nhảy vào nhảy ra. Người nhìn sóng lớn thì tỉnh hơn, nhìn cấp cao nữa thì còn hơn. (B11 01:20-01:22)
9. Vẽ càng ít càng tốt. Thầy chỉ vẽ đường cản và đường tương lai, "chấm hết"; muốn đọc nhanh thì xem thật nhiều biểu đồ, vẽ tay, ghi kịch bản và đối chiếu diễn biến thật. (B9 02:53; B10 02:20; B15 02:14, 02:20)
10. TA đứng một mình khiến chiến lược nhảy vào nhảy ra, biên lợi nhuận mỏng, dễ bán sớm. Vai trò đúng của TA: bổ trợ quy trình, chọn thời điểm hành động sau khi đã hiểu nền tảng doanh nghiệp. (B4 01:59-02:00)

## 2. Phân tích kỹ thuật ghi nhận gì và trả lời câu hỏi nào

### 2.1. Câu hỏi mở đầu và đáp án "tâm lý"

Thầy mở bài TA ở buổi 10 bằng ba câu hỏi cho lớp: TA là gì, có những phương pháp TA nào mọi người quan tâm, và ý nghĩa của TA là gì. Trên bảng thầy vẽ khung "PTKT" với mũi tên sang "tương lai", rồi thêm P (giá) và V (khối lượng) nối sang "Tâm lý", cùng các chữ Entry, Exit, game, đọc vị. (B10 00:18)

Học viên thứ nhất trả lời: TA dựa vào lịch sử giá một mã để dự đoán tương lai. Thầy chốt hai mốc quá khứ (history) và tương lai (future): quan sát đã có dùng để lập giả thuyết về xu hướng hoặc vùng giá, diễn biến sau đó cho biết giả thuyết còn giữ hay phải sửa. (B10 00:20)

Ở buổi 4, thầy đặt câu hỏi: FA giúp xác định nền tảng và giá trị, vậy TA hỗ trợ chỉ ra điều gì. Các đáp án ban đầu gồm điểm mua - điểm bán, lời lỗ, cung cầu, xu hướng, dòng tiền. Thầy cho rằng các ý này có phần đúng nhưng chưa bao quát, chúng là biểu hiện hoặc một phần của bức tranh lớn. Thầy chấm các đáp án để lớp cảm nhận độ sát (thang điểm chỉ biểu thị độ gần với ý thầy, không phải thang đo định lượng của TA). (B4 02:30-02:31)

| Đáp án của lớp | Phản hồi của thầy |
|---|---|
| Điểm mua/bán, cung cầu, xu hướng, dòng tiền | Có phần đúng, nhưng chưa bao quát nhất |
| Ý tưởng của đội lái / ý chí của nhà tạo lập | Gần hơn, khoảng 8 điểm |
| Cá tính cổ phiếu | Còn mơ hồ, khoảng 4 điểm |
| Đường phát triển của doanh nghiệp | Lệch câu hỏi, gần 0 điểm (thuộc lớp nền tảng của FA) |
| Chu kỳ | Là một phần, khoảng 5 điểm |
| Sự quan tâm của nhà đầu tư | Chưa phải ý tổng quát nhất |
| Tâm lý thị trường | Đáp án thầy chốt, 10 điểm |

Thầy viết chữ "TÂM LÝ" rất lớn trên canvas. Cách nhìn này là nền tảng của khoá học: nó nối cung cầu, xu hướng, điểm mua bán, dòng tiền, sự quan tâm, kỳ vọng vào cùng một khung lý giải. Nó không tạo ra điểm mua bán tự động. (B4 02:34)

Phân vai: FA trả lời lớp câu hỏi về doanh nghiệp, tài sản, dòng tiền và giá trị nền tảng; TA trong cách giảng này giúp quan sát dấu vết tâm lý qua giá. Một người có thể hiểu giá trị nhưng vẫn tham gia vì tâm lý, chấp nhận giá vượt xa mức mình từng định. Vì vậy biết công thức chỉ báo hoặc đặt tên một chu kỳ chưa đồng nghĩa hiểu hành vi thị trường. (B4 02:34)

Một học viên ở buổi 9 diễn đạt: TA là phân tích tâm lý đám đông, tức hành động cùng lúc của đám đông; các ngưỡng kỹ thuật là ngưỡng tâm lý nơi cả đám đông cùng hành động. Thầy xác nhận: em đang hiểu dần câu "giá cả là tâm lý". (B9 02:06)

### 2.2. TA có dự báo được không

Sách vở định nghĩa TA là nhìn quá khứ để dự báo biến động giá, giúp xác định điểm đảo chiều, điểm vào lệnh (entry), hỗ trợ, kháng cự. Thầy phản bác thẳng: "chả có dự báo nào được cả", ai áp dụng máy móc các khái niệm đó thì "ăn đạn hết". (B9 02:07)

Một học viên khác nêu góc nhìn công bằng hơn: TA chỉ ghi lại chuyển động giá trong khoảng thời gian mình chọn (một giờ, một ngày). Đường trung bình MA20 lấy giá đóng cửa của 20 cây nến trước để ra giá trị cho cây thứ 21, về bản chất là một dạng dự báo. Dự báo nào cũng có sai số, và kể cả dự báo tốt thì khi điều kiện bên ngoài (kinh tế) đổi, dự báo hỏng. (B9 02:08)

Theo thầy, điều duy nhất dự báo được là **trạng thái tâm lý và ý đồ của nhà cái**. Muốn vậy phải đọc vị ba thứ trên cùng một đồ thị: giá; tâm lý và ý chí của đội lái; tâm lý của nhỏ lẻ đu theo. Thầy nói đây mới là cái khó. (B9 02:10)

Lập luận của thầy: một đường giá muốn đi thì buộc phải có hai thành phần, một bên to là "lái chính" và phần còn lại là những người "đu bám". Khi bên lái dẫn giá, họ buộc phải tạo dựng các trạng thái, sơ đồ, hình thù trên đồ thị. Mọi mẫu hình là do con người tạo ra, tức do tâm lý. (B9 02:10, 02:12)

### 2.3. Đọc thế trước, tìm điểm vào sau

Thầy gọi "tâm pháp" của TA là "đọc vị, đọc thế". Thế là cục diện cung và cầu, hai bên "đánh nhau" ra sao. Trình tự theo thầy: đọc được thế trận, rồi hiểu tâm lý, rồi đọc được vị thế các bên, khi đó mới biết điểm vào (entry) và điểm ra (exit). "Học PTKT mà không đọc được thế trận là thua." (B10 00:23)

Hệ quả: chỉ báo hay điểm mua bán chỉ có nghĩa sau khi đã đọc được "thế" và logic tâm lý. Điểm mua điểm bán ra sau khi đã phán đoán xong chu kỳ, vị thế, tâm lý, "chứ không phải phân tích kỹ thuật là ra mua". Đặt cùng một chỉ báo lên mọi đoạn giá như nhau là sai, vì điều kiện tạo tín hiệu ở mỗi pha khác nhau. (B10 02:29)

Thầy mô tả đường giá có "hồn" và "hơi thở": người chỉ thuộc quy tắc bên ngoài giống người hát đúng kỹ thuật mà chưa có hồn, khác người cảm được nhịp điệu bên trong. Một học viên kể khi vẽ đường giá, trực giác đôi khi làm tay tự đi theo một hướng; thầy đồng tình và nói cảm giác của thầy chính xác "gần 99,99%" (tự đánh giá cá nhân, không có sổ giao dịch hay mẫu thống kê kiểm chứng, không phải xác suất thắng của một phương pháp). Để tăng cảm nhận, thầy khuyên quan sát và luyện nhiều, đừng chỉ lệ thuộc tên phương pháp hay tín hiệu. (B14 01:11-01:12)

Câu hỏi đúng khi nhìn một đồ thị: lượng giao dịch bao nhiêu, lượng hàng sẵn có trên thị trường còn bao nhiêu, và hai thứ đó khớp hay không khớp với giả thuyết đang theo. Điều quan sát được trên biểu đồ là nhịp giá và khối lượng; ý đồ là phần phải suy luận. Một lời giải tốt phải nêu cả dữ kiện đang dựa vào lẫn tình huống nào sẽ làm kịch bản gom, phân phối hay hồi phục không còn đúng. (B13 02:18; B15 02:19)

### 2.4. Đặc thù thị trường quyết định cách đọc

Không thể bê nguyên cách đọc chart từ thị trường này sang thị trường khác mà bỏ qua cơ chế khớp lệnh, biên độ giá cho phép và thanh khoản. Theo thầy (bối cảnh cuối 2021), ở Việt Nam chỉ cần chất lệnh mua lớn ở giá trần là coi như khoá phiên, người khác không mua được, ai bán ra thì lại chất thêm. Ở thị trường nước ngoài khó làm vậy vì khi giá bị đẩy quá mức sẽ có lực bán khống đối ứng nên luôn có thanh khoản. (B4 02:45)

Ở Mỹ không có bảng ba giá như Việt Nam; thay vào đó có Market Profile, sổ lệnh (order book) kèm độ sâu thị trường (depth), bảng giá và khối lượng. (B17 02:29)

Một hệ thống mẫu của thầy chia chỉ báo kỹ thuật thành ba nhóm theo quy ước: Trend (xu thế), Momentum (động lượng), Volatility (biến động). Thầy cho rằng dùng máy không bảo đảm hiệu quả dự báo, nhất là khi bê một phương pháp từ thị trường khác về mà chưa xét dữ liệu và tập quán địa phương. Nên đọc các nhóm tín hiệu theo mục đích và kiểm xem chúng có đo đúng hiện tượng đang quan tâm. (B7 03:51)

### 2.5. Hạn chế của việc chỉ dùng TA

Theo thầy, chỉ dùng TA khiến chiến lược thành liên tục nhảy vào nhảy ra theo nhịp, hiệu quả thấp, biên lợi nhuận mỗi lần rất mỏng; dễ bán quá sớm rồi không dám mua lại, trong khi có cổ phiếu sau đó tăng gấp 3-4 lần. Gốc vấn đề là không có cơ sở về giá trị và hoạt động doanh nghiệp để giữ vị thế qua các nhịp rung. (B4 01:59)

Vai trò đúng của kỹ thuật theo thầy: bổ trợ cho quy trình, giúp chọn thời điểm sau khi đã hiểu nền tảng doanh nghiệp; không phải lớp phân tích đứng một mình. (B4 02:00; xem chương 16)

Thầy còn nói trong tay bên mạnh, đồ thị và giá sàn là công cụ doạ nạt tâm lý chứ không chỉ là dữ liệu trung tính. (B12 00:39)

### 2.6. Thái độ với sách

Thầy khuyên vẫn đọc nhiều sách, nhưng đọc xong phải "thoát khỏi sách", biết các hạn chế và chỗ sai của tư duy trong đó. Ở buổi 12, thầy nói khi đã dạy "tâm pháp" thì các phương pháp trong sách nên bỏ, đọc nhiều mất thời gian mà không hiệu quả; thầy sẵn sàng cho cả nghìn cuốn nếu ai thích. Ở buổi 13, thầy phê phán nặng sách và trường phái PA (price action): "PA là không đáng đọc luôn", vì các cách đọc kỹ thuật áp máy móc không phản ánh được trận thế đang diễn ra; phải hiểu mỗi công cụ đang trả lời câu hỏi nào. Một học viên kể từng theo học CMT hai năm trước rồi ngẫm sâu mà bỏ. Thầy nói thêm: chỉ báo và sách kỹ thuật "sách nào cũng có, ai cũng dạy", nhìn bảng giá và chỉ báo rồi phản ứng thì không thành công; thứ làm đổi cách đánh là nhìn ra trận pháp và hành vi đứng sau. (B9 02:16; B12 01:09; B13 02:57, 02:50)

Thầy cũng nói thẳng với lớp: ông sẽ chia sẻ cách lồng phương thức TA vào mô hình chuỗi thời gian để phát hiện điểm đảo chiều, cách mà theo thầy không có trong sách vở và là kinh nghiệm TA của riêng thầy chứ không dạy theo sách. (B2 00:37; B4 04:09)

## 3. Nến Nhật và OHLC

### 3.1. Định nghĩa theo cách của thầy

Thầy nói định nghĩa nến không lấy từ sách: nến Nhật phản ánh biên độ dao động giá trong một phiên và "lưu vết lực tác động qua lại của hai bên cung cầu" trong phiên đó. Một nến có bốn mức giá: Open (mở), High (cao nhất), Low (thấp nhất), Close (đóng). Thân nến nối mở với đóng, bóng nến kéo tới cao nhất và thấp nhất. Biên độ cả kỳ = High - Low. Màu thân cho biết đóng cao hay thấp hơn mở. (B10 00:31)

Dù dùng phần mềm nào thì bố cục cũng na ná nhau: một vùng đồ thị giá và một vùng chỉ báo hoặc khối lượng; vị trí bố trí tuỳ phần mềm, không quan trọng. (B10 00:30)

### 3.2. Bài tính một nến

Phiên có Open 40, High 43, Low 39, Close 42. (biên soạn tính lại) (B10 00:32)

| Phần của nến | Cách tính | Kết quả |
|---|---|---|
| Biên độ toàn phiên | 43 - 39 | 4 |
| Độ dài thân | 42 - 40 | 2 |
| Bóng trên | 43 - 42 | 1 |
| Bóng dưới | 40 - 39 | 1 |
| Lợi suất đóng so với mở | (42 - 40) / 40 | 5% |

Nến ngày không cho biết giá chạm cao trước hay thấp trước. (B10 00:32)

### 3.3. Cách thầy dùng nến

- Nến vẫn là cách hiển thị dữ liệu thầy dùng (cho thấy mở, cao, thấp, đóng), nhưng thầy KHÔNG dùng các mô hình nến Nhật như Hanging Man (người treo cổ), Hammer (cây búa) và các mẫu tương tự: "đừng có dùng". Cần phân biệt cách hiển thị với việc suy kết luận từ hình dạng một cây nến. (B10 02:35)
- Đọc một cây nến riêng lẻ chỉ nắm được ý tưởng biên độ của phiên đó ("nến để nhìn cho vui"); muốn dùng được phải so nhiều nến với nhau, tức đọc cả cụm nến qua một khoảng thời gian. (B10 00:32)
- Thầy nói rất thẳng: "nến là vứt", trong các mô hình thì mẫu nến không có ý nghĩa gì, "ai theo nến là thất bại 100%" (cách nói của thầy). Thầy kể đã kiểm định các mô hình dựa trên mẫu nến Nhật trên thị trường Việt Nam và kết quả "thất bại hết"; ai sa đà đọc nến thì bị thị trường "cho ăn rồi bắt chạy như vịt". Nguồn không nêu bộ mẫu, tham số, thời kỳ hay chi phí của các lần kiểm thử này. (B9 02:15; B10 01:37)
- Ở buổi 11, thầy nói nến "ngu ngốc", không bao giờ chơi. Nhưng nếu làm app hay phần mềm thì vẫn phải đưa vào, vì đám đông tin; cũng như sóng, Fibonacci, hỗ trợ: phải hiểu để biết đám đông tin ở điểm nào nên họ sẽ phản ứng ở điểm đó, "đánh ở những điểm hợp lý". Đây là ẩn ý để hiểu đám đông, không phải tin vào đó để hành động; thầy nói "những cuốn sách đó nên đốt" vì dễ bị dẫn dắt, luôn phải tỉnh táo. (B11 03:23)

### 3.4. Đọc cụm nến đi ngang bằng ngôn ngữ tâm lý

Cụm nến dao động trong vùng hẹp, chưa rõ hướng, thầy gọi là "lưỡng lự". Chỉ nói "sideway" thì ai cũng thấy và vô nghĩa; người dịch được ra chữ "lưỡng lự" mới nắm được yếu tố tâm lý. Muốn biết lưỡng lự vì cái gì thì kéo trục thời gian nhìn về bên trái, xem vùng giá trước đó, biên cũ, và cách giá thoát ra hoặc quay lại vùng. (B10 00:33)

## 4. Khối lượng và quan hệ giá - khối lượng

### 4.1. Vì sao phải có khối lượng

Thầy nhấn: "không thể nói giá không mà phải có volume". Giá cho biết mức khớp và hướng thay đổi, khối lượng cho biết lượng giao dịch đi kèm; phải hỏi một biến động giá đi với lượng lớn hay nhỏ so với trước đó. (B10 00:21)

Theo thầy, khối lượng còn quan trọng hơn giá: thầy viết V, mũi tên sang P, và chữ "TÂM LÝ" dưới phía giá. Volume đi trước và quyết định, giá (P) là thứ được dùng để tác động tâm lý nhà đầu tư. Người học kỹ thuật chỉ nhìn các điểm giá mà không hỏi "có hàng để tích luỹ hay không" là sai trọng tâm. Thầy nói đa số người chơi không chú ý khối lượng, còn ông "cực kỳ chú ý vol" vì vol cho biết động thái tâm lý và cách đánh của người đang đánh. (B13 02:16; B10 00:59)

Dấu vết của sự chuẩn bị và việc đổi người cầm hàng nằm trong khối lượng, còn giá có thể tạo cảm giác tâm lý rất mạnh; khi đọc phải giữ giá và lượng trong cùng bối cảnh, không dùng một phía để kết luận. (B13 03:16)

Khối lượng cũng dùng để kiểm định cách đọc: hai đoạn giá giống nhau về hình dáng nhưng khác thanh khoản thì diễn giải khác nhau. (B10 00:59)

### 4.2. Hai loại đường giá

Theo thầy, mã có dòng tiền và tâm lý đám đông dẫn dắt thì đường giá "có ý chí", đi ra đường nào rõ đường đó, thường đi kèm khối lượng rất cao. Mã không có dòng tiền thì giá nhấp nhô vô hướng, "không có ý chí gì", thường kèm khối lượng thấp. (B10 01:52)

Cách lọc thầy tiết lộ: chạy hồi quy xu hướng cho chuỗi khối lượng, cần độ dốc dương và càng lớn càng tốt (khối lượng tăng dần), đồng thời độ dốc của chuỗi giá cũng dương. Cả hai cùng dương thì cổ phiếu đang uptrend "quá rõ" (xem chương 12). (B10 01:53)

Trường hợp giá tăng nhưng khối lượng giảm hoặc thấp: theo thầy vẫn là xu hướng tăng và còn là dạng "ngon" nhất, gọi là tăng trong trạng thái khoá hàng, siết hàng: nguồn cung đã bị gom hết, hoặc cổ đông không chịu bán vì giá chưa vừa ý. Ai đang giữ đúng mã này thì "ngồi rung đùi". (B10 01:54)

### 4.3. Bài suy luận khối lượng sau vùng tích lũy

Cách học thầy chọn ở buổi 11: không mở biểu đồ có sẵn mà vẽ trên trang trắng, học viên tự tưởng tượng và tự vẽ tiếp để tăng độ cảm nhận. Đề bài: một mã đã hoàn tất phần gom, được đẩy lên 2 phiên; đặt mình vào vai người có vốn lớn đã gom nhiều thì sẽ làm gì tiếp. Học viên trả lời: rũ, đạp xuống, đẩy tiếp. (B11 01:23)

**Nguyên tắc 1.** Khi đã gom đủ rồi đẩy thì khối lượng không nên tăng nhiều, không tăng liên tục. Nếu đẩy 2 phiên, sang phiên thứ 3 khối lượng vẫn tăng, hàng vẫn cứ ra, thì nghĩa là bên ngoài vẫn còn nhiều hàng, chu trình gom chưa hoàn thành, hoặc có người bất ngờ bán ra mà tạo lập không lường được vì thị trường "vô hình". Khi đó tạo lập chắc chắn không đẩy tiếp mà đạp xuống gom thêm; trong lúc đè gom lại thì khối lượng tăng lên. (B11 01:25)

**Nguyên tắc 2.** Nếu đẩy ngày 1, ngày 2, sang ngày sau khối lượng co lại (cột ngắn lại) thì tạo lập tự tin đẩy tiếp, vì đồng nghĩa bên ngoài không còn hàng để bán. Cách giải thích khác cho cùng hiện tượng: các cổ đông đoàn kết, hoặc cổ đông biết giá trị thật của doanh nghiệp nên không chịu bán rẻ. Khi xác định khối lượng bán ra nhỏ, hàng bên ngoài đã cạn, thì tạo lập chắc chắn đánh lên, có thể siết trần mà không sợ ai đạp vì lượng bán rất ít. (B11 01:26, 01:28)

Hệ quả cho nhà đầu tư nhỏ: không đọc được vị thế này thì bị "dắt mũi", thấy đạp là sợ bỏ chạy, nhảy lung tung và mất hàng. Nếu hiểu là tạo lập đang gom, có người bán ra nên phải đè tiếp, thì cứ nằm chờ cho họ gom xong. (B11 01:27)

| Quan sát | Cách thầy giải thích | Điều còn phải kiểm tra |
|---|---|---|
| Vừa thoát nền, giá nhích lên, khối lượng lớn và tăng tiếp sang phiên 3 | Bên ngoài còn nhiều hàng, gom chưa xong, dễ bị đạp xuống gom tiếp | Giá có giữ được không, ai tạo ra lượng bán |
| Giá tăng, khối lượng co lại | Hàng bên ngoài đã cạn, tạo lập tự tin đẩy tiếp | Có đủ cầu mới hay chỉ là ít người giao dịch |
| Giá nằm nền lâu, khối lượng biến thiên | Đang đè gom, hấp thụ cung | Có phải chỉ là mã không ai quan tâm |
| Gần vùng cao, khối lượng đột biến, giá giật mạnh nhưng không tiến | Vùng đỉnh, đang phân phối | Vị trí trong cả chu kỳ, phản ứng các phiên sau, định giá cơ bản |

(biên soạn tổng hợp, B11 01:25)

Lưu ý bổ sung từ bảng tra nhanh cuối buổi 11: dấu hiệu cảnh báo vùng cao là volume lớn lặp lại nhưng giá tiến ít, không giữ được mức cao; volume thấp khi giá tăng chưa chắc tốt vì có thể ít cung nhưng cũng có thể thiếu cầu. (B11 01:38, 01:26)

### 4.4. Đọc khối lượng đúng theo giai đoạn

- **Trong nền gom** có thể cộng hoặc quan sát volume của cả đoạn tích lũy rồi so với các cột mới. Một học viên bị hai cột volume lớn làm lo mà quên nhìn lượng giao dịch và vùng hấp thụ đã xảy ra từ trước; cách đúng là xem cả đoạn tích lũy rồi mới so với hai cột mới, không lấy riêng hai cột đó để suy ra đã phân phối xong. Phép cộng này chỉ là cách ước lượng quá trình, không phải phép quy đổi ra số cổ phiếu nằm trong tay một chủ thể. (B13 03:16)
- **Khi giá đã vào giai đoạn chạy** thì không thể cộng volume theo cách của nền gom, vì lượng lúc này luân chuyển qua nhiều nhịp (cùng một cổ phiếu đổi tay nhiều lần), nên tổng giao dịch không còn thể hiện đơn giản lượng hàng gom một chiều. Cách diễn giải một đại lượng phải đổi theo giai đoạn vận động. Thay cho phép cộng, thầy chuyển trọng tâm sang "cách đánh": đọc cách đi lệnh, diễn biến giá và phản ứng ngay lúc đó của nhịp (nhận định của thầy, không có thuật toán định lượng thay thế). (B13 03:21-03:22)
- Một cột khối lượng có ý nghĩa khác khi nằm trong nền lâu tháng so với khi nằm ở cuối nhịp dựng mạnh; thầy không đưa ngưỡng số, đây vẫn là phép đọc theo kinh nghiệm, cần đặt cạnh điều kiện doanh nghiệp và thị trường chung. (B13 03:33)
- Cột volume lớn trong phiên hồi chưa chắc là gom: cột lớn có thể chứa cả mua mới lẫn người bán cần tiền; không gọi tất cả là gom và cũng không mặc định lượng lớn khi giá hồi là phân phối đã kết thúc. (B13 03:42)
- Cột khối lượng chỉ cho biết có giao dịch, tự nó không tách được bao nhiêu là giao dịch nội bộ (chuyển giữa các tài khoản của cùng một nhóm) và bao nhiêu là hàng thật đổi chủ từ người ngoài; không coi tổng volume một phiên là số hàng một bên đã thu được. (B15 02:03)
- Cột volume phải đọc theo đúng vị trí thời gian của giá chứ không đọc rời. (B15 02:02)
- Khi phần khối lượng gần như không có cột đáng kể (ví dụ CPH), biểu đồ giá không còn nói lên khả năng giao dịch: phải hỏi về lượng đối ứng trước khi nói tới tỷ lệ tăng kỳ vọng. (B15 02:32)

### 4.5. Dấu hiệu giá và khối lượng theo thầy

| Dấu hiệu | Mô tả | Lưu ý |
|---|---|---|
| Nghi phân phối trong chuỗi giảm - hồi - giảm | Giá đạp xuống, được đỡ thành một hai nhịp hồi không vượt bền, rồi giảm tiếp; các ngày đạp sâu có cột đỏ cao vọt. Theo thầy, bán lớn ở các ngày ấy cho thấy người sẵn hàng (cổ đông lớn) tranh thủ nhả, không phải vài nhà đầu tư lẻ bán bất chợt | Đọc cả chuỗi, không tách riêng một nến tăng (B15 02:18) |
| "Đảo hàng" của đội chuyên nghiệp | Giá không được kéo dứt khoát một mạch mà nhấp nhả từng nhịp, có đoạn phân phối, nhả hàng rồi quay lại kiểm tra (test), hàng sang tay nhiều | Không biến chữ "test" thành lý do coi mọi nhịp hồi là điểm vào lại (B15 02:14) |
| Hàng cô đặc | Giá tăng kiểu bậc thang, nhiều nền nhỏ nối tiếp, nến hẹp. Theo thầy đó là cổ phiếu nằm gần hết trong tay doanh nghiệp hoặc cổ đông lớn, họ "tự diễn" | Chuỗi nến lên đều không chứng minh rủi ro thấp (B15 02:21) |
| "Giữ nhịp" trong nền tích luỹ | Các cột volume nổi bật cách nhau khá đều, giá giữ tương đối cân bằng. Thầy gọi là đội "nắn": hàng về thì đỡ, rồi xả, rồi kéo lại | Là chuỗi hành động theo thời gian, một cột cao đứng riêng không đủ kết luận (B15 02:25) |
| Gom dài có ngày mua vọt | Giai đoạn gom rất dài vẫn có ngày mua vọt rất mạnh (ai bán lượng lớn là bị mua hết); bên có chủ đích chấp nhận giá sau đó còn bị đạp và "chịu nhiệt" lâu để thu thêm hàng | Mua xong giá chưa tăng không tự phủ định ý định tích luỹ (theo thầy) (B15 02:25) |

Hai lưu ý nữa: sự đều đặn của đường giá không cho biết độ sâu cung cầu ngoài thị trường (lượng nhỏ giao dịch được nhưng lượng lớn có thể thiếu người đối ứng khi cần thoát); và phải phân biệt một nhịp hồi giúp bớt kẹt với việc cấu trúc đã thực sự đổi. (B15 02:22-02:23)

Thầy cũng nhận xét lối kéo giá quá thốc có thể gây khó khi muốn ra một lượng hàng lớn, vì bảng giá lên cao chưa bảo đảm có đủ người mua đối ứng để chuyển hết vị thế thành tiền. (B13 03:40)

### 4.6. Sổ lệnh, độ sâu và phổ khối lượng

- Kinh nghiệm của học viên tên Quân: nhìn lệnh chặn trên và chặn dưới. Ví dụ có khối lượng đặt mua rất lớn ở giá 10; sau đó một số lệnh nhỏ chất bán ở giá 11; rồi xuất hiện một lệnh mua giá 11 khớp đúng bằng khối lượng đang bán ở 11. Học viên coi đó là tín hiệu có bên chủ động. Thầy nhận xét: kinh nghiệm này khó áp dụng, chỉ nhận ra khi mọi thứ đã khá rõ nét nên tỷ suất ăn được không cao. (B9 02:20, 02:22)
- Nhà đầu tư đọc sách thường chỉ nhìn tín hiệu kỹ thuật, ngưỡng hoặc đường cắt nhau rồi lao vào, hầu như không ai "dòm lệnh"; dùng công cụ kỹ thuật phải đi kèm quan sát lệnh và cách giá đáp trả. (B15 00:50)
- **Phổ khối lượng (Volume Profile).** Chọn đoạn bắt đầu và kết thúc, công cụ vẽ phân bố khối lượng theo từng mức giá trong đoạn, để biết giá hiện tại nằm đâu so với "lực lượng thị trường" (vùng giao dịch tập trung). Chọn đoạn khác thì phân bố đổi. Thầy nói có chỉ báo sẵn nhưng muốn xem theo từng đoạn có thể phải cài thêm (tên chỉ báo chưa xác nhận); người quen rồi thì nhìn mã là có ấn tượng về vùng giá, không cần vẽ phổ nữa. Một số công cụ có sẵn trong AmiBroker. (B17 02:29-02:30)
- Phân biệt: độ sâu sổ lệnh là các lệnh đang chờ tại các mức giá ở thời điểm mở sổ; khối lượng theo giá tổng hợp giao dịch đã khớp tại từng vùng giá trong khoảng đang xét. Hai thứ trả lời hai câu hỏi khác nhau. (B17 02:29)

## 5. Xu hướng, kênh giá, hỗ trợ, kháng cự, nền giá và tích luỹ

### 5.1. Xu thế là tiêu chí lọc số một

Khi thầy hỏi "lọc bằng cái gì", một học viên đáp: xem giá so với MA50, MA200 và khối lượng. Thầy nhận xét đó là trả lời theo sách vở. Thứ phải nhìn trước tiên là trend, tức xu thế: "xu thế là bạn". MA và khối lượng chỉ là công cụ; trước khi dùng phải nói được mình tìm loại xu thế nào, ở khung thời gian nào. (B10 01:17)

Thầy tự nhận là người chuyên đầu tư theo xu thế và cho rằng đây là chiến lược hiệu quả nhất ở bất cứ thị trường nào, "sẽ tồn tại mãi mãi" (theo thầy). (B10 01:18)

Thầy nói thích thị trường có xu hướng rõ (tăng hoặc giảm), "không chơi" vùng giằng co: ở vùng biên các phe phái khác nhau cùng vào nên xung đột lợi ích rất mạnh, giá qua lại rất khó. Trong pha giảm vẫn có nhịp hồi ngược chiều, như pha tăng có nhịp lùi; phải xác định cấp độ và bối cảnh trước khi gọi là xu hướng mới. (B11 02:17, 02:16)

### 5.2. Đường xu thế và kênh giá

Đường xu thế, kênh xu thế (nối các đáy, các đỉnh rồi kéo dài) rất dễ vẽ, nhưng theo thầy "vẽ này là vẽ quá khứ, mà quá khứ thì nhìn đâu chẳng đúng". Cái cần học là đọc được trạng thái hiện tại và dựng kịch bản phía trước. Nên ghi lại các mốc đã dùng để vẽ, để sau này kiểm xem mình có dời đường cho khớp kết quả hay không. (B10 00:37)

Khi nghi một điểm ngoặt, đừng chỉ kéo dài đường cũ: ghi rõ biến nào đổi hướng, đổi lúc nào, biến nào xác nhận. Một nhịp hồi của một đường khác với sự đổi hướng kéo dài của cả nhóm chỉ tiêu. (B2 00:36)

Trên hình vẽ đối chiếu, một đường dao động nhanh, ngắn hạn có thể lên xuống nhiều lần quanh một đường xu hướng chậm hơn; phải phân biệt nhịp ngắn với hướng đi dài, không kỳ vọng thực tế trùng khít một nét vẽ đơn giản. (B4 04:05)

### 5.3. Hỗ trợ và kháng cự

- Theo thầy, đường hỗ trợ là thứ người ta hay dùng để tạo dựng niềm tin cho nhà đầu tư ("cứ rớt xuống đây là có hỗ trợ"); thực chất có hỗ trợ nghĩa là có lực marketing hoặc big boy không muốn cho giá về thấp hơn. (B11 01:55)
- Thầy khuyên không nên chơi những mã kiểu "giữ không cho xuống sâu nhưng không bao giờ tăng cao": nếu bên giữ giá đủ sức giữ thì họ đã đánh lên, họ chỉ giữ chứng tỏ "cũng chả cần" đẩy. Sách kỹ thuật nói "những mảng tốt bền vững nên nắm" nhưng khi thị trường chung xuống thì mã đó cũng xuống theo; hỗ trợ chỉ đúng trong một đoạn. Quá khứ "chưa thủng" không bảo đảm tương lai "không thể thủng". (B11 01:56)
- Các mức hỗ trợ và ngưỡng kỹ thuật mà nhiều người tin là nơi có nhiều người chờ mua (bắt đáy). Bên phân phối canh đúng các ngưỡng đó để kéo rồi nhả, vì ở đó có sẵn đối tác nhận hàng. Phải phân biệt một ngưỡng vẽ từ quá khứ với lực cầu thực sự duy trì ở đó về sau. (B15 00:37)
- Ở đoạn kéo kích, đội lái vận dụng hết các điểm kỹ thuật mà đám đông nhìn (Fibonacci, đỉnh cũ, MACD), thậm chí cố ý kéo vượt luôn vùng cản để loại những người tin vào kháng cự và kích lòng tham đuổi theo. (B9 02:30)
- Slide "Support level" (ví dụ in sẵn, MetaStock): đồ thị có bốn mũi tên chỉ các lần giá chạm vùng hỗ trợ, chú thích "Notice how the price has a difficult time falling below the support of $51.25". Đây là ví dụ của bộ slide, không phải giá VNM; chữ VNM là thầy thêm khi liên hệ miệng. (B11 01:55)

### 5.4. Đọc đồ thị dài hạn: đỉnh cũ, vòng đánh cũ và vòng mới

Phải kéo đồ thị về quá khứ đủ dài. Câu thầy nhấn: cổ phiếu "có ghi nhớ", lịch sử giá có ghi nhớ; đỉnh cũ là nơi đội lái từng đánh và họ có thể đánh lại. (B9 02:26)

Cách đọc một vòng đã xong: ở vòng trước đội lái kéo lên và đã ra hết hàng; sau đó giá xoay quanh vùng thấp nhiều năm và đội lái không nắm gì. Đó là dấu hiệu họ đã thoả mãn, đánh xong một vòng. (B9 02:28)

Kiểm chứng giả thuyết gom lại bằng khối lượng: nếu đội lái gom thật thì vùng đó khối lượng phải tăng lên, vì họ phải ăn hàng ở đó bằng mọi giá. Các nhịp kéo lên rồi đạp xuống quanh nền là để hàng đổi chủ về tay họ. (B9 02:29)

Cùng một vùng đi ngang sau khi tăng, có người gọi là phân phối, có người (học viên) đọc là chưa phân phối. Tên gọi phải đi kèm tiêu chí: khối lượng, tiến trình trước và sau. (B9 02:25)

Một học viên ở buổi 17 dùng mô hình "alo": tìm đỉnh trong 12 tháng, so với giá hiện tại; khoảng cách (gap) lớn thì chọn mua vì cho rằng giá có chu kỳ và "trí nhớ" ở các mức từng lên (nghe thầy dạy). Khoảng cách này chỉ là đầu vào suy luận, chưa cho biết xác suất quay về đỉnh. (B17 01:45)

### 5.5. Phân biệt đi ngang (sideway) và gom

Học viên hỏi làm sao phân biệt vùng đi ngang (SW) với vùng gom để biết khi nào vào. Một học viên đáp: sideway thì khối lượng không giảm dần, còn gom thì khối lượng càng ngày càng giảm; thầy nói "chưa đúng". (B11 02:00)

Giải thích của thầy: ở vùng đi ngang thuần, khối lượng không biến động lớn, chênh lệch giữa các phiên không nhiều. Ở vùng gom, khối lượng "đột biến": có phiên rất ít, có phiên cực nhiều; đồng thời giá bị đạp (có phiên tăng mạnh, có phiên rơi mạnh) nhưng xoay quanh một biên độ giá nhất định và cứ giữ, giá không về sàn; tham chiếu rồi đỏ chút, hôm sau lên hơn tham chiếu 1-2% rồi lại đỏ. Phải kẹp đủ điều kiện này (khối lượng thất thường, giá giật nhưng giữ biên) mới là gom, không chỉ nhìn hai đường ngang. Hình viết tay "SW # Gom" là định tính, không có ngưỡng volume. (B11 02:01)

Mục tiêu của gom theo thầy: gom phải kín đáo nhưng phải tác động tâm lý để nhà đầu tư sợ hãi ném hàng ra. Cách làm: gom nhẹ nhàng, lệnh mua rất ít rồi đạp sàn, nhà đầu tư sợ hãi bán hết, toàn bộ "gà vịt" chạy qua đây. Khi gom xong ("cất vó"), kéo giá lên thì hầu như không còn hàng để bán vì người sợ đã chạy hết. (B11 02:02)

Lượng gom: người ngoài không biết chính xác thời điểm lái nghĩ là đủ. Thông thường (theo thầy) lái phải gom khoảng 3-5% số cổ phiếu trôi nổi (lưu hành tự do) thì mới đánh được; có mã gom dưới 5%, hiếm khi quá 10%. Những lái lớn "tự làm cho chính mình" (chủ doanh nghiệp tự lái cổ phiếu mình) thì hàng đã của họ, không cần gom. Nhãn "gom" chỉ là giả thuyết quan sát từ hành vi giá, không đọc được tài khoản hay kế hoạch của người khác. (B11 02:03)

Bài luyện 13 (biên soạn): lập ba cột: (1) điều nhìn thấy: biên giá, tiến triển giá, volume; (2) giả thuyết: tích lũy, thiếu quan tâm hay cân bằng tạm thời; (3) dấu hiệu phân biệt ở các phiên sau. Nếu cột (2) dài mà cột (1) trống thì lời giải thích đang đi trước dữ liệu. (B11 02:04)

### 5.6. Sửa cách gọi "tích luỹ" và đọc vùng gom thật

Sửa cách gọi "tích luỹ" (ví dụ cổ phiếu Mỹ): đoạn giá đã tăng từ 8 lên 21 không phải tích luỹ mà là đã đẩy xong một nhịp. Vùng gom hàng thật là đoạn đi ngang trước đó cho tới chân sóng, nơi khối lượng bắt đầu tăng dần. (B9 02:36)

Thầy phản biện quy trình của một học viên (tìm cổ phiếu tích luỹ đi ngang dài; khi giá đột biến kèm khối lượng đột biến và MACD cắt lên thì đưa vào danh sách; xem thông tin hỗ trợ; có điểm vào tốt thì mua): quy trình này "vẫn sai và sách vở" vì không đọc được ý đồ đằng sau đồ thị. Nó không trả lời được ba câu: đội lái đang gom hàng, hay đang tích luỹ ở nền thấp, hay đã nâng nguyên một nền và đang giữ để tạo mặt bằng giá mới. Ba trạng thái này nhìn đều giống "đi ngang". Nếu đợi tới khi giá và khối lượng đột biến thì đó là lúc họ đánh kích lên, giá trần, "có hàng đâu mà mua"; người vào theo tín hiệu đó vào đúng lúc rủi ro đã khác hẳn. (B9 02:18-02:20)

Nhóm các mã theo cấu trúc quan sát được (nhịp tăng, nền giá, kiểu điều chỉnh, lực giao dịch) giúp tìm ví dụ kiểm một quy tắc; cần giữ riêng đặc điểm đo được và giả thuyết về người tham gia phía sau. (B9 02:50)

Thầy cho rằng không chỉ báo hay phương pháp kỹ thuật phổ thông nào lọc được đúng vùng cổ phiếu đang bị đè để gom (vùng sớm của câu chuyện); chỉ có cách đọc hành vi kết hợp hiểu doanh nghiệp mới nhận ra. Ở giai đoạn cuối sóng, hình mẫu kỹ thuật đẹp còn được tay to dùng để giăng bẫy người mua đuổi. (B4 02:52, 03:14)

Thầy đề nghị học viên tự nghiệm lại: mọi sai lầm đều nằm ở chỗ những mã đang bị đè gom, tích lũy thì không bao giờ mua, cứ xăm xăm lao vào mã đang tăng và đu vào. Người khôn chơi ngược lại: thấy vùng gom thì vào nằm chờ, khi "thằng bự" đánh lên thì mình lên theo. (B11 01:32)

### 5.7. Tăng bậc thang, rơi nhanh và bất đối xứng thời gian

Thầy vẽ sơ đồ đường tăng từng bậc rồi rơi rất nhanh. Ví dụ: muốn tăng 50% có thể mất gần 3 tháng, còn rơi 50% có khi chỉ một tuần, 5 phiên, thậm chí một ngày (ở Mỹ). Giai đoạn đánh lên mất 2-3 tháng, giai đoạn rơi nhiều khi chỉ 2 tuần là về lại điểm cũ. Nhịp hồi sau giảm thường chỉ khoảng mười mấy phần trăm ("giỏi lắm" tới 32%; con số nói nhanh, nguồn chưa rõ), và không về lại đỉnh. Thầy dùng sơ đồ này để nói nhịp giảm nhanh hơn nhịp tăng. (B11 02:15)

Bài tính 14 (biên soạn tính lại): tăng 50% rồi giảm 50% không bù nhau. (B11 02:17)

| Giá đầu | Giá sau | Mức thay đổi |
|---|---|---|
| 100 | 150 | +50% |
| 150 | 75 | -50% |
| 50 | 100 | +100% để hồi về |
| 70 | 100 | +42,86% để hồi về (100/70 - 1) |

Một loại hình cần tránh: mã đi ngang hoặc giảm kéo dài nhiều năm, các lần hồi không tạo được bước tiến bền (ví dụ VNM từ 2018) là loại hình không hợp với mục tiêu đầu cơ theo nhịp, vì vào dễ bị chôn vốn. Nhận xét này về nhịp giá, không phải kết luận doanh nghiệp xấu. (B15 02:30)

## 6. Đường trung bình và các chỉ báo thông dụng

### 6.1. SMA là gì, tính thế nào

Đường trung bình đơn giản (SMA) lấy trung bình giá đóng cửa của N kỳ gần nhất. MA20 lấy giá đóng cửa 20 cây nến trước để ra giá trị cho cây thứ 21. Dưới đây là hai bài tính (biên soạn tính lại).

**Bài tính SMA20.** Tổng 20 giá đóng cửa là 400 thì SMA20 = 400 / 20 = 20. Phiên sau thêm giá mới 23, loại giá cũ 18, tổng mới 405, SMA20 = 20,25. Đường trung bình đi lên chỉ vì giá mới cao hơn giá bị loại; nó mô tả quá khứ, không hứa hẹn tương lai. Khung thời gian khác nhau làm ý nghĩa 20 kỳ khác nhau. (B9 02:08)

**Bài tính SMA5.** Năm giá đóng cửa 20, 21, 19, 22, 23 cho SMA5 = (20 + 21 + 19 + 22 + 23) / 5 = 21. Kỳ sau đóng 24, cửa sổ bỏ 20 thêm 24: SMA5 = (21 + 19 + 22 + 23 + 24) / 5 = 21,8. Đường MA tăng vì số thêm vào cao hơn số bị bỏ ra. (B10 00:29)

Khi đổi khung nến thì một "kỳ" của MA đổi nghĩa: khung ngày thì MA(50) là 50 phiên, khung tuần thì là 50 tuần. (B10 00:28)

Câu tự kiểm tra gắn với bài này: nếu giá hiện tại giữ nguyên mà giá cũ bị loại khỏi cửa sổ thì MA có thể đổi hướng không. (B10 02:47)

### 6.2. Vì sao là 50 và 200

Một học viên kể quy tắc hay dùng: kiểm tra MACD và đường bình quân, xem đường ngắn có "ngóc đầu lên" so với đường dài không; tham số thường chọn 50 (trung hạn) và 200 (dài hạn). (Chú giải: MACD tạo từ chênh lệch của các đường trung bình hàm mũ, khác với MA; 50 và 200 là độ dài cửa sổ của MA.) (B10 00:26)

Thầy hỏi ngược: vì sao lại là 50 và 200. Theo thầy, đó là "sách nói", các con số tự thân "không có ý nghĩa gì", do người dùng chọn; ai dùng mà không lý giải được tham số thì không khám phá được "bí mật" phía sau, và bí mật đó là **chu kỳ** (bài vĩ mô đã dạy: mọi thứ đều có chu kỳ). Tham số phải đặt cạnh chu kỳ đang nghiên cứu. (B10 00:27)

Phép quy đổi thầy nêu: mỗi tuần khoảng 5 phiên nên 50 phiên xấp xỉ 10 tuần, tương đương khoảng 3 tháng nếu trừ ngày nghỉ; 200 phiên xấp xỉ 40 tuần, thầy nói "khoảng sáu tháng". Biên soạn tính lại: 40 tuần là khoảng 9 tháng lịch chứ không phải 6 tháng, lời thầy ở đây không khớp. Ý chính của thầy: người ta gọi 50 là trung hạn, 200 là dài hạn chỉ vì gần các mốc quý, nửa năm, chứ không có cơ sở sâu hơn. (B10 00:28)

Các đường MA 12, MA 50, MA 200 cũng nằm trong số những thứ thầy nêu khi phê bình việc coi tên chỉ báo hoặc một ngưỡng đơn lẻ là quyết định cuối cùng. (B4 02:47)

### 6.3. Chỉ báo chỉ phản ánh lớp đã biểu hiện

Ví dụ thầy nêu: RSI lên vùng 70 (là ngưỡng chỉ số 70, không phải lãi 70%), MACD dương hoặc phân kỳ, các đường MA. Theo thầy các chỉ báo này chỉ phản ánh một lớp xu hướng đã biểu hiện rồi, chỉ nên tham khảo, không cho biết ý đồ của người tạo ra xu hướng. (B4 02:47)

| Tên hoặc giá trị thầy nhắc | Vai trò trong lời giảng |
|---|---|
| RSI và ngưỡng 70 | Ví dụ của việc đọc một ngưỡng đơn lẻ |
| MACD dương, phân kỳ | Ví dụ gắn nhãn tín hiệu mà bỏ bối cảnh |
| MA 12, MA 50, MA 200 | Các đường trung bình người học quen dùng |
| Cơ chế giá trần và thanh khoản | Phải hiểu đặc thù thị trường khi đọc đường giá |

Bộ công cụ một nhóm học viên kể đang dùng để lọc mã: mẫu nền giá, thứ tự sắp xếp các đường MA, khối lượng giao dịch, dải Bollinger (co hẹp hay mở rộng), Ichimoku. Thầy không giảng cách dùng từng công cụ khúc đó, mà phê bình việc học công cụ rời rạc mà không hiểu nguyên lý: điểm chính là phải xác định TA đang phản ánh cái gì trước khi dùng nó để ra quyết định. (B4 01:41, 02:30)

Về các công cụ như đường trung bình, Bollinger, Ichimoku, thầy nói "học cho vui thôi". Ichimoku (mây) và nến chỉ là tài liệu tham chiếu. (B9 02:11; B10 01:00)

### 6.4. MACD và RSI trong một nhịp thử cung

Thầy nêu MACD và RSI có thể đổi hướng ngay trong một nhịp hạ hoặc nhúng (thử cung), khiến người chỉ bám tín hiệu đó rời vị thế đúng lúc nhịp thử diễn ra (nhận xét trên ví dụ này, không phải kiểm định rằng MACD hay RSI luôn sai). (B13 03:13)

Một học viên kể trước đây đợi chỉ báo phát tín hiệu rồi mới mua; sau khi học thì tập nhìn sự vận động của dòng tiền và điều kiện hình thành tín hiệu, nên khi dấu hiệu quen thuộc hiện rõ thì đã có vị thế từ trước, không còn mua đuổi chỉ báo. Bài học: phải phân biệt sự việc đang diễn ra với chỉ báo phản ánh sự việc đó (chỉ báo đi sau). (B15 00:01)

Thầy dặn đừng học TA kiểu máy móc, bật hết MA, Fibonacci, MACD lên đồ thị; càng dùng nhiều chỉ báo càng phụ thuộc, càng rối mắt và càng "lừa" độ nhạy cảm của chính mình. Đọc được giá và volume rồi thì "đâu cần chỉ số gì", ngày xưa thầy cũng bám chỉ báo "như thằng ngốc". (B10 01:04; B15 02:26)

### 6.5. Ngưỡng quá mua

Giá vừa bước vào nhịp tăng thì chỉ báo đã báo quá mua và khuyên thoát, trong khi bối cảnh mới còn đẩy giá đi rất xa. Chỉ báo loại này chỉ đo khoảng cách so với mức gần đây, không biết một chu kỳ đã hoàn tất hay chưa. Thầy gọi các thuật toán kiểu này là "vớ vẩn", dù các trường lớn sùng bái và ai học tiến sĩ vẫn phải học để lấy bằng. (B10 02:00)

## 7. Mẫu hình giá và giới hạn của chúng

### 7.1. Mẫu hình trong sách

Bảng dưới là danh mục mẫu hình thầy chiếu ở buổi 11 cùng nhãn in trên slide. (B11 01:50)

| Tên trên slide | Cấu trúc | Nhãn trên slide |
|---|---|---|
| Ascending triangles (tam giác tăng) | Biên trên nằm ngang, đáy nâng dần | Trong uptrend, bullish |
| Descending triangles (tam giác giảm) | Biên dưới nằm ngang, đỉnh thấp dần | Trong downtrend, bearish |
| Falling wedges (nêm giảm) | Hai biên cùng dốc xuống và hội tụ | Bullish, cả trong uptrend lẫn downtrend |
| Rising wedges (nêm tăng) | Hai biên cùng dốc lên và hội tụ | Bearish, cả trong uptrend lẫn downtrend |
| Flags (cờ) | Đoạn đi nhanh (cán cờ) rồi vùng nghỉ dạng kênh nhỏ | Bullish trong uptrend, bearish trong downtrend |
| Pennants (cờ đuôi nheo) | Đoạn đi nhanh rồi vùng nghỉ hội tụ dạng tam giác nhỏ | Bullish trong uptrend, bearish trong downtrend |
| Rectangles (chữ nhật) | Giá đi ngang giữa hai biên rồi tiếp diễn xu hướng cũ | "found in uptrends" bullish; "found in downtrends" bearish |
| Head and shoulders (vai đầu vai) và dạng đảo ngược | Vai trái, đầu, vai phải, đường viền cổ (neckline) | Đảo chiều trong uptrend, bearish; dạng ngược đảo chiều trong downtrend, bullish |

Mô tả thêm về vai đầu vai: một đỉnh giữa cao, hai đỉnh hai bên thấp hơn. Gọi tên mẫu hình chỉ là ghi một giả thuyết; mẫu chỉ được xác nhận bằng các phiên về sau (xem độ cao tương đối các đỉnh, vùng đáy nối giữa các đỉnh, phản ứng khi giá về vùng đó). Slide không cung cấp quy tắc đặt lệnh hay đo mục tiêu. (B10 00:40; B11 01:55)

Menu công cụ vẽ trên phần mềm biểu đồ thầy mở có: Mô hình Tam giác, Mô hình vai đầu vai, Sóng đẩy Elliott, Sóng Elliott Tam giác, Các đường chu kỳ, Mô hình ABCD. Thầy khoanh nhóm này và nói ông hầu như chỉ thích dùng "các đường chu kỳ", công cụ ông thấy rất ít người dùng. (B10 00:51)

### 7.2. Vì sao thầy không tin vào mẫu hình

- **Mẫu hình là cái đám đông cùng tin.** Thầy nói thẳng là ông "không tin lắm" vào các mẫu hình phổ biến (tam giác, vai đầu vai, sóng Elliott), vì đám đông tin tất cả các mẫu này nên nhà cái, người lái sẽ "vẽ" đồ thị sao cho đám đông tin. Mẫu hình phải được đọc qua phản ứng thực tế của thị trường (được hưởng ứng hay thất bại), không phải xem hình có "đúng sách" không. (B10 00:47)
- **Chiến lược "dắt mũi".** Bên nắm cuộc chơi lừa nhà đầu tư bằng chính sự hiểu biết của đám đông. Ai đi học cũng được nhồi cùng bộ kiến thức: mô hình giá, MACD phân kỳ dương, RSI ở vùng 50 đang hướng lên 70 là vùng hấp dẫn để mua. Big boy, "đạo diễn" vẽ đúng các tín hiệu đó cho nhà đầu tư tin; nhà đầu tư bị kéo đi vì chính niềm tin và kiến thức đã học. Thầy gọi các đội lái là "nghệ sĩ". Đám đông tin mô hình nào (breakout, trendline, vùng cản) thì họ tạo đúng cái đó. (B9 01:46-01:47)
- **Hệ quả thực hành:** đừng hành động theo cái mình tin sẵn; khi thấy tín hiệu đẹp phải đoán mình đang bị dắt về hướng nào và vị trí đó nguy hiểm ra sao. (B9 01:49)
- **Mọi mô hình nhà cái vẽ được hết**, "thích loại gì vẽ ra loại đó". Lớp đùa ngành đầu tư có nghề "hoạ sĩ tài chính"; ở Việt Nam còn có đường rắn, đường nhảy cầu, mô hình thác nước, dòng suối. Bitcoin vừa tạo ra kiểu bơm xả mới mà không sách kỹ thuật nào có, vài năm sau sách mới cập nhật. (B9 02:11)
- **Ví dụ giả định ABC.** Nếu một mô hình ABC được phổ biến rộng và ai cũng tin tới một vùng hay một cấu trúc nhất định thì nên mua, bất kỳ tay to nào cũng sẽ cố tình tạo diễn biến trông đúng quy tắc ABC để đám đông tin và mua vào. Khi mọi người cùng chờ một tín hiệu thì hành vi của họ dễ đoán, tức là "lộ địa hình": đối phương biết đám đông sẽ đặt lệnh ở đâu và dùng chiêu thức biến hoá để tiêu diệt. Đối phương "dùng chính tâm pháp" của mình: mình tin vào điều gì thì bị đánh đúng vào điều đấy. Vì vậy phải kiểm tra hoàn cảnh và động cơ phía sau, không coi tín hiệu là quy luật tự thực hiện. (B15 00:04-00:05)
- **Trong vùng phân phối** (theo thầy): nếu bên làm giá điều khiển nhịp giá khéo thì các mô hình TA quen thuộc bị vô hiệu; thầy nói mạnh là áp đủ loại mô hình ở đoạn này thì "100% sai" (cách nhấn mạnh, không có thống kê; ý rút ra là phải xét hành động tạo nên mô hình). Sách TA dạy sau đà tăng, đoạn chững lại là giai đoạn nghỉ (tích luỹ) trước khi tăng tiếp; chính cách đọc này khiến người có hàng tiếp tục giữ và mua thêm đúng ở vùng bên kia đang phân phối. (B15 00:36-00:37)
- **Học thuộc "bách khoa mẫu hình".** Học viên và thầy phê bình thói quen học thuộc cả cuốn bách khoa mẫu hình rồi tin ai nhìn ra hình nhanh hơn thì thắng. Nhớ nhiều hình vẽ không có nghĩa là hiểu cơ chế làm giá và quan hệ cung cầu phía sau. Một sai lầm khác là cố ép đồ thị cho giống một mẫu có sẵn; câu hỏi cần đổi từ "nó giống hình gì" thành "điều kiện và hành động nào đang tạo nên hình này". (B15 00:01-00:02)
- **Tín hiệu phải dẫn đến việc tìm nguyên nhân**, không dẫn thẳng tới phản xạ mua hoặc bán đã học thuộc. Thầy kể chính thầy từng ngồi suy nghĩ lại rất kỹ vì nhận ra cách hiểu cũ có thể sai; từ khi đổi cách tiếp cận thì cơ hội thắng cao hơn (kinh nghiệm cá nhân, không phải số đo xác suất). Hai câu thầy luôn tự nhắc: vì sao hiện tượng đó xuất hiện, và vì sao bên kia cố tình làm vậy để mình tin. (B15 00:00, 00:03)
- Câu ôn tập: vì sao thuộc mẫu hình chưa đủ để hiểu TA? Vì hình chỉ là biểu hiện; phải giải thích được lực cung cầu, thông tin và hành động tạo nên hình, đồng thời xét xem có ai đang dựa vào niềm tin phổ biến ấy để tác động ngược lại mình hay không. (B15 00:00)

### 7.3. Cách thầy đọc lại các mẫu hình

- **Điểm mua theo mẫu hình là "điểm chết".** Khi mẫu đã hiện rõ thì phần lợi còn lại rất nhỏ, không đáng đặt cược. Với cờ và cờ đuôi nheo, lúc nhận ra thì giá đã "bu lên" rồi. Thầy nói đã tự kiểm nghiệm cách đánh theo mẫu hình và kết luận học theo một phương thức như vậy là sai. (B11 01:51)
- **Đọc lại cùng một hình:** đoạn đầu là gom, đoạn giữa là đẩy, đoạn nghỉ là điều chỉnh (tạo thanh khoản). Điều chỉnh là chỗ để người ngoài vào, nhưng vào đó chỉ ăn phần sau. Phần lợi lớn nhất là đoạn từ nền gom đi lên; cái giá để có nó là thời gian nằm vùng khó chịu lúc đè gom. (B11 01:51)
- **Cách sách vở dạy mà thầy phê phán:** thấy ra hình tam giác đi lên thì mua, thấy tam giác hay nêm đi xuống thì bán chạy. Thầy vẽ thêm lên slide để chỉ giá hoàn toàn có thể bị đạp xuống ngay trong đoạn nền của mẫu, hoặc có biến cố đột xuất, nên không thể đinh ninh mẫu hình đi đúng hướng sách vẽ. (B11 01:50)
- **Mẫu chữ nhật (đi ngang):** theo thầy vùng ngang giữa xu hướng là quá trình tạo lập tạo thanh khoản, tạo sức hút; trong vùng đó tạo lập "thích đạp thì đạp, thích đẩy thì đẩy", gặp yếu tố bất ngờ là đạp, chứ không phải cứ vào vùng ngang là giá sẽ lên. Hình dạng ngang chưa xác nhận quá trình gom. (B11 01:53, 01:58)
- **Các bài phân tích kiểu "đang sideway, đang tạo nền, vượt lên là có thể mua"** không tính đến điều kiện của tạo lập. Tạo lập bo được hàng thì mới đánh lên; không bo được thì vứt luôn. Chỉ cần một big boy khác bán ra, hoặc chủ tịch, cổ đông lớn công bố xả hàng, là người đang đánh không có lý do gì đánh tiếp, họ nhả ra và đứng xem. (B11 01:54)
- **Vai đầu vai:** theo thầy "có khác gì mô hình Fibonacci đâu", chỉ là cùng một quá trình đè gom, đẩy, xả được vẽ thành một hình khác; dạng ngược là quá trình tạo đáy (đánh xong thì tạo đỉnh). Một cụm biến động nhỏ có thể "đổi vai" khi nhìn ở khung lớn: nếu sau đó có một đợt đánh lớn hơn vượt đỉnh cũ thì cả cụm vai đầu vai nhỏ trước đó chỉ còn là một cái vai (vai trái) hoặc một nhịp nhỏ trong cấu trúc lớn. Ngược lại nếu lực giữ giá hết thì mẫu không cần hoàn thành mà rơi thẳng. (B11 01:55; B10 00:42)
- **Mọi mẫu chỉ là tên gọi bề mặt, cái ẩn bên dưới là chu kỳ.** Cốc tay cầm, vai đầu vai đều như vậy; cùng một cụm nến có thể giống một mẫu ở khung nhỏ nhưng thuộc nhịp khác ở khung lớn. Một cụm vai, đầu, vai (và vai đầu vai ngược) tự nó là một chu kỳ nhỏ đã hoàn tất, nhưng gộp lại chỉ là một phần của chu kỳ lớn. (B10 00:45, 00:52)
- **Hai cách đọc cùng đoạn giá** (B10 00:57): cách một đánh dấu riêng từng nhịp ngắn (lên, nhả, đánh lại một quả ít nhất bằng đỉnh cũ rồi nhả dần); cách hai bỏ qua nhịp nhỏ để thấy hình lớn. Nếu nhịp tiếp theo có lực kích lên vượt vùng dự kiến thì cái từng gọi là "vai" phải đọc lại thành một phần của nhịp đánh tiếp; diễn biến sau đó quyết định cách đọc nào còn đúng.
- Thầy tuyên bố các môn mẫu hình này "không có giá trị" nếu dùng riêng; vẫn chiếu để chỉ ra cái sai nằm ở đâu. (B11 01:53)

### 7.4. Lọc theo mẫu hình khó hơn lọc theo chỉ báo

Thầy nhấn: lọc theo tín hiệu chỉ báo thì "bình thường", lọc theo mẫu hình mới khó vì "định nghĩa hình cực khó". Một học viên có lập trình xác nhận chỉ "đi ngang" đã khó định nghĩa. (B12 02:53; xem chương 13)

## 8. Chu kỳ giá và thời gian

### 8.1. Vì sao giá có chu kỳ: các câu trả lời của lớp

Thầy đặt câu hỏi gốc trước khi dạy Fibonacci và sóng: các quy luật về giá có một quỹ đạo riêng chi phối bởi tạo hoá hay không; vì sao thị trường và giá cổ phiếu có chu kỳ. Thầy muốn người học hiểu cơ chế sinh ra chu kỳ chứ không học thuộc hình vẽ. (B11 00:21)

| Học viên | Câu trả lời |
|---|---|
| 1 | Giá chỉ có giá trị trong một chu kỳ; hết chu kỳ thì thị trường lập mặt bằng giá mới |
| 2 | Giá phụ thuộc tâm lý, tâm lý có chu kỳ nên giá có chu kỳ theo tâm lý |
| 3 | Tính mùa vụ: ở Mỹ có "Sell in May", từ tháng 5 đến 8, 9 khối lượng thường rất thấp; cuối năm bán rồi sang năm mua lại để giảm thuế; các "đội lái" nhỏ và lớn phối hợp cũng tạo chu kỳ; khảo sát thấy trung bình 18-20 năm chứng khoán sập một lần (con số áng chừng, nguồn chưa rõ) |
| 4 | Ví với bốn mùa miền Bắc: tích lũy là mùa đông, kéo dần là xuân rồi hạ; cuối hạ sang thu là lúc hưng phấn nhất, giá tăng mạnh nhất; sau đó đi ngang rồi quay lại mùa đông. Liên hệ "tâm pháp" đè, gom, đẩy của thầy |
| 5 | Mọi thứ có chu kỳ: tuần 7 ngày có nghỉ để tái tạo năng lượng; kinh tế và thời tiết cũng vậy |
| 6 | Giá phụ thuộc tâm lý; tâm lý phụ thuộc tài chính cá nhân, văn hoá, chu kỳ kinh tế (gần Tết cần chi tiêu thì rút tiền khỏi các kênh đầu tư) |
| 7 và 8 | Cảm giác có chu kỳ nhưng không ước lượng được đang ở vùng cao hay thấp; giống cung cầu, âm dương, lên đỉnh thì phải xuống; năm đó tiền "chạy ngoài đường" phải chảy vào tài chính vì logistics và ngành khác chưa bắt kịp (bối cảnh 2021-2022) |

(B11 00:22-00:30). Nhận xét của thầy: ai cũng nêu được ý nhưng chưa ai truy tới quy luật của vũ trụ, của tự nhiên, tức nguồn gốc sinh ra chu kỳ. (B11 00:27)

### 8.2. Cách thầy lý giải nguồn gốc chu kỳ

Thầy tự nhận: "đây là cách lý giải của tôi thôi". Lý do thầy mở bài bằng vũ trụ: nếu chỉ đưa tiền đề "mọi thứ đều có chu kỳ" mà không giải thích vì sao thì rất khôi hài; phải lý giải được nguồn gốc thì người học mới có niềm tin vào quy luật. (B11 00:37)

1. **Quỹ đạo khép kín sinh ra lặp lại.** Hình vẽ Mặt Trời ở giữa, Trái Đất trên một vòng quỹ đạo, ký hiệu T là chu kỳ. Trái Đất vừa tự quay vừa quay quanh Mặt Trời, còn có Mặt Trăng và các hành tinh khác. Đã quay theo quỹ đạo khép kín (elip, tạm gọi là vòng tròn) thì chắc chắn quay lui quay tới, đó là chu kỳ, nên vạn vật có quy luật lặp lại. (B11 00:31)
2. **Bốn mùa và sản lượng.** Vị trí trên quỹ đạo chia bốn giai đoạn xuân, hạ, thu, đông; cây cối nảy mầm, ra hoa, rụng lá, trơ trụi rồi lại nảy mầm. Từ đó sinh ra chu kỳ sản lượng: nông nghiệp, hàng hoá theo mùa vụ. Tương tác của các hành tinh khác thêm các chu kỳ khác chồng lên. (B11 00:33)
3. **Âm dương, thuỷ triều, từ trường.** Phía được Mặt Trời chiếu là dương, phía tối là âm (Việt Nam sáng thì Mỹ tối), sự luân chuyển tạo dịch chuyển các luồng khí; Mặt Trăng tác động thuỷ triều, con nước và tâm lý; lõi sắt từ bên trong Trái Đất chuyển động sinh cực từ, từ trường này có lúc thay đổi và theo thầy cũng ảnh hưởng trạng thái tâm lý, cũng có quy luật. (B11 00:37)
4. **Vết đen và bão Mặt Trời** (hình ghi "sun spots"): một học viên nói chu kỳ bão Mặt Trời trùng năm 2020, năm đó có nhiều hiện tượng lạ (mùng Một Tết miền Bắc có mưa rào, mưa đá). Thầy giải thích: điểm đen là nơi năng lượng Mặt Trời bùng nổ, thổi bức xạ về Trái Đất; bình thường từ trường cản được, vụ nổ quá mạnh thì bức xạ lấn vào, gây bão từ, thời tiết đổi, con người nóng bức khó chịu (theo thầy). (B11 00:40)
5. **Mỗi người là một ăng-ten.** Mỗi người là một "ra-đa", "ăng-ten" có tần số dao động f riêng: 7 tỷ người là 7 tỷ ăng-ten. Mỗi hành tinh quay phát bức xạ, sóng điện từ tần số riêng tác động lên con người; mỗi người là tổng (ký hiệu sigma, từ 1 đến vô cực) của mọi tác động đó, như tổng hợp dao động trong vật lý, tạo thành "sóng riêng". Hệ quả: đám đông không đồng nhất, mỗi người phản ứng khác nhau trước cùng một thông tin. (B11 00:41)
6. **Chuỗi truyền dẫn:** quy luật của vũ trụ (tự nhiên) -> quy luật đời sống kinh tế xã hội -> quy luật kinh tế -> quy luật chứng khoán. (B11 00:39)

Kết luận của thầy cho chứng khoán: giá cả là tâm lý; các quy luật tự nhiên tác động lên tâm lý nên giá gần như chắc chắn cũng có quy luật chu kỳ. Giá là tổng hợp của tất cả các đám đông; đám đông hưng phấn, lạc quan là do nền kinh tế thuận lợi. Thầy đảo cách nghĩ thông thường: không phải chúng ta nỗ lực mà tạo ra kết quả, thực ra quy luật chu kỳ đang dẫn dắt chúng ta; ai nắm quy luật thì dùng nó để dự đoán. (B11 00:47)

Phần liên hệ với chu kỳ kinh tế: chu kỳ nền kinh tế có quy luật cỡ 10 năm; chu kỳ của đường giá chứng khoán chỉ là chu kỳ tương đối. (B2 02:05, 02:11; xem [Chu kỳ kinh tế và chỉ báo](01a-chu-ky-kinh-te-va-chi-bao.md))

### 8.3. Fractal và nén khung thời gian

Theo lý thuyết fractal các mẫu hình lồng nhau ở nhiều thang, nên phải thu nhỏ để nhìn mẫu hình trong bức tranh nền kinh tế chung thì mới ráp được. (B2 02:11)

Nguyên lý fractal áp vào thực hành (thầy gọi là phương pháp hạn chế nhiễu): khi khảo sát trong một tập mẫu hẹp, người xem bị rung theo dao động của tập đó; phải nén dữ liệu nhỏ lại (xem khung rộng hơn) thì quy luật tổng thể mới hiện ra và nhiễu giảm. Thực hành: đối chiếu đồ thị ngày với tuần, tháng; hướng lớn còn rõ thì nhịp nhỏ chỉ là đường đi bên trong. (B2 02:14)

Nhịp giá ngắn phải luôn đặt trong ngữ cảnh chu kỳ nền: nó thuộc đoạn đang lên, đang xuống hay đi ngang của nhịp lớn hơn. Khi đổi khung ngày, tuần, tháng phải nói rõ đang nói nhịp hồi ngắn hay xu hướng chính. (B2 02:10; B10 00:52)

Khung thời gian: biểu đồ ban đầu ở khung tháng, đổi sang D (ngày), đổi sang nến, thêm volume; phải biết mình đang quan sát khung nào trước khi đếm sóng. Thu phóng khác nhau cũng có thể đổi cách đánh dấu giai đoạn (ví dụ C4G ở cửa sổ giá thu nhỏ). (B11 02:35; B12 02:13)

### 8.4. Công cụ đường chu kỳ và cách đếm chu kỳ

Nguyên tắc của thầy: "sóng gì thì sóng, sóng không quan trọng bằng chu kỳ". Mỗi chu kỳ là "một trận đánh". Nếu nhìn ra được các giao điểm giữa các chu kỳ (chỗ kết thúc chu kỳ này, mở chu kỳ sau) thì đọc đồ thị rất hay. (B10 00:45)

**Cách chia chu kỳ trên một đồ thị:** tìm điểm khởi đầu của quá trình gom hàng; kéo đường chu kỳ tới chỗ hoàn tất chu kỳ gom; chu kỳ kế tiếp là đoạn kéo giá, điểm bán gần như ngay đỉnh ở cuối chu kỳ đó; sau đó phối hợp thêm vài tín hiệu để "mạo hiểm gom lần hai nếu có". Một đầu mút chu kỳ chỉ rõ sau khi đã đủ dữ liệu. (B10 00:46)

**Cách kéo đường chu kỳ (theo thầy).** Chỉ kéo chính xác được khi người ta đã hoàn tất một chu kỳ. Muốn biết đoạn tích luỹ đã hoàn tất thì phải chờ giá đánh lên 2-3 ngày tăng sau đó mới nhận ra; không ai nhìn ra ngay tại đáy. Khi đã thấy "ông này tích luỹ xong rồi" thì đặt công cụ từ đầu này sang đầu kia của đoạn tích luỹ. Công cụ chiếu ra các đường chu kỳ kế tiếp; thường các điểm đổi nhịp của giá rơi sát các đường này. (B10 01:07)

**Cách dùng đường chiếu.** Khi giá chạm mốc chu kỳ mới nhất thì bán. Chỉ khi xác nhận được tín hiệu là họ vẫn tiếp tục đánh thì mới theo lên đường chu kỳ thứ hai. (B10 01:08)

**Cách đánh số.** Đoạn gốc (đoạn tích luỹ dùng để đo) là chu kỳ 0; đoạn trước gốc là âm 1; các đoạn sau là 1, 2, 3. Kinh nghiệm của thầy: thông thường người ta không đánh quá ba chu kỳ. Ai không muốn mệt thì hết hai chu kỳ là nên ra cho nhẹ đầu, vì càng về chu kỳ sau xác suất rủi ro càng cao. Bản thân thầy thường chỉ đánh hai chu kỳ, "hàng ngon xong rồi thì đi làm hàng khác". (B10 01:08)

Hỏi đáp: học viên hỏi làm sao xác định khoảng chu kỳ, hay chỉ phán đoán theo chu kỳ tâm lý? Thầy: có cách tính, công thức sẽ dạy ở buổi thứ hai về TA; buổi này chỉ dạy ý tưởng, cố ý không đưa công thức. (B10 01:05)

**Bài thực hành HQC (B9).** Thầy cho học viên mở một mã bất kỳ, gõ mã vào phần mềm rồi tự tập; câu hỏi giữ nguyên hình biểu đồ và nói có mấy "vòng vận động", buộc người xem chỉ ra ranh giới chu kỳ và dữ kiện nhận diện thay vì dùng một tên mẫu. Trên HQC (Địa ốc Hoàng Quân), học viên nêu đã vào từ nhịp vùng giá rút gọn 5-6 (nghìn đồng), trả lời có ba hiệp (ba chu kỳ). Thầy diễn giải: đội này đánh chu kỳ một xong thì hoàn tất, thấy thời cơ thì đánh chu kỳ hai, rồi chu kỳ ba "do ông chủ xóc mã" (nguồn nhận dạng nhiễu). Muốn kiểm số nhịp phải thống nhất mốc bắt đầu, kết thúc và xem có gộp sóng nhỏ trong chu kỳ lớn hay không. Slide HQC: nhiều lần giá nhô khỏi vùng thấp, điều chỉnh, đi ngang rồi một nhịp tăng dốc bên phải; đường trung bình ngắn phản ứng nhanh và sát giá hơn đường dài; mức ngang đỏ đi qua các nền cũ; cột lượng lớn hơn ở các nhịp biến động rõ. (B9 02:46-02:48)

Mỗi cổ phiếu có cách vận động riêng; mô tả hiệu quả ở mã này có thể kém ở mã khác hoặc khi giai đoạn đổi. Quy trình học: nêu đặc điểm đang thấy, dự kiến diễn biến hợp với nó, và quan sát nào buộc phải sửa nhận định. (B9 02:49)

## 9. Fibonacci: nguồn gốc, tỷ lệ vàng và cách dùng như phép đo

### 9.1. Vì sao thầy thích Fibonacci

Thầy thích công cụ chu kỳ vì nó dựa trên một quy luật tự nhiên là Fibonacci. Ẩn dụ: bộ rễ hoặc tán cây, nhánh mẹ đẻ nhánh con, lan toả mãi, và mọi nhánh đều theo một quy luật chung của toán học Fibonacci. Theo thầy, đường giá cũng như nhánh cây: vận động theo quy luật phát triển, lan toả và có yếu tố chu kỳ. (B10 00:48)

Hai tính chất thầy rút ra từ hình nhánh cây: (1) tính chu kỳ; (2) tính đệ quy, tức các lớp nhánh con nằm ẩn trong nhánh lớn và lặp lại cùng cấu trúc, nên hiểu quy luật một nhánh nhỏ thì gần như suy ngược về gốc, và nhìn một vùng nhỏ có thể gợi cấu trúc tương tự ở khung lớn. (B10 00:50)

Theo thầy, ai biết vận dụng yếu tố chu kỳ theo Fibonacci thì "gần như đoán được tương lai" và đó là bí quyết xác định điểm ra, điểm vào. Muốn dự báo tầm khoảng 1 năm thì bắt buộc lồng ghép Fibonacci theo trục thời gian; điều này hầu như ít người làm. (B10 00:50; B2 02:15)

"Bí mật" theo thầy: phải tin vào quy luật, và tin được vì thấy nó tương đồng, được dẫn ra từ quy luật tự nhiên. Khi hiểu gốc thì mới biết sửa công cụ theo cách riêng, điều chỉnh và sáng tạo kỹ thuật riêng; còn dùng phần mềm kéo một phát ra các mức "thì ai chả làm được". Thầy phê bình cách dạy phổ biến "đi học 100 khoá, khoá nào cũng dạy kiểu đó": bảo kéo thước từ điểm này đến điểm kia rồi đọc các mức như sách. Người học kiểu đó không tự hỏi "vì sao tôi phải tin điều này", nên cực kỳ mệt, không biết cách điều chỉnh khi thị trường khác đi. (B11 00:53)

### 9.2. Leonardo Fibonacci và bài toán thỏ

Slide: Leonardo Fibonacci, còn gọi Leonardo of Pisa, 1170 - khoảng 1250, nhà toán học người Ý. (B11 00:55)

Bài toán thỏ theo lời thầy: ban đầu có một cặp thỏ đực cái (thầy gọi là âm dương), sau một khoảng thời gian chúng sinh sản và cứ thế tiếp diễn. Fibonacci thống kê tổng số cặp qua từng đời, khảo sát nhiều lần và thấy một quy luật; ông tự hỏi tiếp có hay không quy luật tương tự của tự nhiên áp dụng cho các loại hình khác, rồi quan sát tiếp; từ đó tính ra một tỷ số gọi là tỷ lệ vàng. (B11 00:57)

| Thế hệ | Số cặp thỏ |
|---|---|
| 1 | 1 |
| 2 | 1 |
| 3 | 2 |
| 4 | 3 |
| 5 | 5 |
| 6 | 8 |

Quy tắc: mỗi số bằng tổng hai số liền trước, F(n) = F(n-1) + F(n-2), vì số cặp kỳ này gồm các cặp đã có cộng số cặp mới do các cặp trưởng thành sinh ra. Slide: 1+1=2; 1+2=3; 2+3=5; 3+5=8; 5+8=13; 8+13=21. Biên soạn tính lại: thế hệ 7 = 13, thế hệ 8 = 21, thế hệ 9 = 34, thế hệ 10 = 55. (B11 00:58)

Slide "The Fibonacci/Golden Spiral": dãy 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144... với 11 phép cộng; các ô vuông có cạnh là số Fibonacci xếp cạnh nhau, đường xoắn ốc đi qua các ô. Thầy giải thích: dãy số là các số rời rạc, người ta dùng trí tưởng tượng chuyển sang hình học thành đường xoắn liên tục; từ đó khám phá cùng quy luật trong vỏ ốc, vỏ sò, hình dạng cơn bão, cách sắp cánh hoa. (B11 01:02)

Thầy cũng nhắc quy luật này liên quan tới tỷ lệ vàng (và nhắc thêm tương quan với các hằng số như e, nguồn chưa rõ). Dãy: 1, 1, 2, 3, 5, 8, 13, khoảng cách giữa các số nở dần ra. (B10 00:50)

### 9.3. Tỷ lệ vàng (phi)

Slide "The Golden Ratio": chia một đoạn thẳng thành hai phần a (dài) và b (ngắn) sao cho (a+b)/a = a/b. Giá trị phi = (1 + căn 5)/2 = 1,6180339887..., viết gọn Phi = 1,618. (B11 00:59)

Biên soạn tính lại: đặt x = a/b, từ (a+b)/a = a/b suy ra 1 + 1/x = x, tức x^2 - x - 1 = 0, nghiệm dương là (1 + căn 5)/2. Hệ quả: 1/phi xấp xỉ 0,618 và 1/phi^2 xấp xỉ 0,382 (hai mức Fibonacci quen thuộc; trong video chỉ có một slide Elliott ghi nhãn .618, thầy không dạy đầy đủ mọi mức). (B11 01:00)

Tỷ số hai số Fibonacci liên tiếp tiến dần về phi, dao động hai phía (biên soạn tính lại): (B11 01:00)

| Phép chia | Kết quả xấp xỉ |
|---|---|
| 2/1 | 2,000 |
| 3/2 | 1,500 |
| 5/3 | 1,6667 |
| 8/5 | 1,600 |
| 13/8 | 1,625 |
| 21/13 | 1,6154 |
| 34/21 | 1,6190 |
| 55/34 | 1,6176 |
| 89/55 | 1,6182 |
| 144/89 | 1,6180 |

Tức là tiến gần phi chứ không bằng ở mọi bước. (B11 03:49)

**Tính đệ quy** (thầy dùng đúng từ này): cái to có gì thì cái nhỏ cũng có vậy, cái nhỏ hơn nữa cũng vậy, "thằng to giống thằng nhỏ". Ví dụ trên slide "Golden Ratio in the Body": cánh chim và từng lớp lông cánh; tỷ lệ cẳng tay và bàn tay; các đốt xương ngón tay nối tiếp theo cùng tỷ lệ; khoảng cách các vùng trên khuôn mặt. Thầy ví như con trai giống bố, con gái giống mẹ. Đây là nền cho ý "sóng lớn chứa sóng nhỏ cùng cấu trúc" ở phần Elliott. Thầy chỉ vào ảnh sóng biển: sóng cũng theo tỷ lệ, từ chân sóng lên ngọn đều có quy luật; "dù sóng to hay sóng nhỏ gì cũng có quy luật của nó". (B11 00:59, 01:00)

### 9.4. Tỷ lệ vàng trong tự nhiên, nghệ thuật, thiết kế

- Slide "Golden Spiral in Nature" và "Golden Ratio in Nature": vỏ ốc, cơn bão nhìn từ trên cao, hoa, xương rồng, quả thông, hoa hướng dương, hoa cúc; "Golden Ratio in the Ancient World": ngôi đền cột cổ có lưới tỷ lệ chồng lên mặt đứng. Thầy kết luận người cổ đại đã hiểu và áp dụng các quy luật tỷ lệ này (theo thầy; slide chỉ là ảnh minh hoạ, không có số đo). (B11 01:03)
- Nghệ thuật: bức Tiệc ly có lưới tỷ lệ vàng chồng lên; chân dung Mona Lisa có đường xoắn vàng. Theo thầy, người vẽ dùng đúng tỷ lệ phi nên tranh có độ sâu, hài hoà, tinh tế, đó mới là tranh đáng tiền (slide không có tư liệu chứng minh ý định họa sĩ). Thiết kế số: ảnh hươu cao cổ, hoa, phong cảnh có lưới hoặc đường xoắn; đầu con vật, bông hoa, núi đều chứa tỷ lệ vàng (theo thầy). (B11 01:07-01:08)
- Logo: National Geographic có khung vàng với a/b xấp xỉ 1,61; Toyota a/b = a'/b' = 1,618; Apple; Pepsi có các đường tròn a/b = 1,618; biểu tượng chim Twitter dựng từ các cung tròn; nhân vật Sonic có đường xoắn phủ đầu và mặt. (B11 01:09)
- Niềm tin thầy nêu: cái gì theo tỷ lệ vàng thì cân bằng, cân bằng thì bền vững, tồn tại lâu; theo tỷ lệ vàng thì đẹp vì tạo hoá ẩn quy luật trong đó. Thầy cho rằng các công trình cổ theo tỷ lệ vàng trụ qua nhiều cuộc chiến tranh cũng vì thế (theo thầy). (B11 01:10)
- Hỏi đáp về nguồn gốc: học viên từng học nhiếp ảnh và kiến trúc hỏi tỷ lệ vàng có từ khi nào, vì kim tự tháp và đền Athens có trước Fibonacci mà chiều rộng, chiều dài đã theo tỷ lệ vàng (học viên nhớ Fibonacci ở thế kỷ 15-16, lệch với mốc 1170-1250 trên slide). Thầy trả lời: toán học Ai Cập với kim tự tháp có trước Fibonacci rất xa và người xưa đã hiểu tỷ lệ vàng; nhắc Fibonacci vì ông là người gần nhất hệ thống lại. (B11 01:11)
- Bố cục web "Divine Proportion: 1.618": khung rộng 960 px chia thành 593 px và 367 px (960 / 1,618 = 593; 960 - 593 = 367). Biên soạn tính lại: 593/367 xấp xỉ 1,6158, lệch nhẹ so với 1,618 do làm tròn. (B11 01:17)
- Phi Grid (hai đường dọc, hai đường ngang chia khung theo tỷ lệ phi) khác "Rule of Thirds" (chia ba phần bằng nhau). Biên soạn tính lại: với khung 900 đơn vị, vạch một phần ba ở 300 và 600, còn vạch phi ở khoảng 344 và 556. Thầy giải thích về nhiếp ảnh: chụp ảnh phải bố cục theo tỷ lệ mới ra ảnh nghệ thuật; đẩy đường chân trời lên tít phía trên thì ảnh bí, bức bối, mất độ sâu, giống vào căn nhà trần thấp đụng đầu. Thầy chốt loạt slide: "đây chính là quy luật của thị trường chứng khoán", dẫn sang sóng Elliott. (B11 01:17-01:18, 03:49)

### 9.5. Fibonacci theo trục giá

Công dụng thực tế thầy khuyên: dùng Fibonacci để ước lượng độ mở rộng lợi nhuận (vùng giá mục tiêu) hoặc điểm dừng, tức để ước đoán vùng, không phải bắt chính xác một điểm. Kết quả phụ thuộc hoàn toàn vào cách chọn điểm đầu và điểm cuối đoạn đo. (B10 00:53)

Lấy biên độ giữa đỉnh và đáy tham chiếu để ra các mức giá. Ở buổi 11, thầy nhắc lại: lấy mốc trên biểu đồ để xác định đoạn gom (vùng tích lũy, điểm bắt đầu của quá trình), kéo dãy Fibonacci ra sẽ được các điểm mục tiêu; các điểm này không chính xác tuyệt đối nhưng gần như ăn khớp với diễn biến giá. (B2 02:06; B11 00:52)

**Bài tập trục giá** (biên soạn tính lại): nhịp tăng từ A = 20 đến B = 30, độ dài nhịp 10. Mức hồi = 30 - tỷ lệ hồi x 10. (B10 02:09)

| Tỷ lệ hồi | Phép tính | Giá tương ứng |
|---|---|---|
| 23,6% | 30 - 0,236 x 10 | 27,64 |
| 38,2% | 30 - 0,382 x 10 | 26,18 |
| 50% | 30 - 0,5 x 10 | 25,00 |
| 61,8% | 30 - 0,618 x 10 | 23,82 |

Lưu ý: đổi A hoặc B thì mọi mức đổi theo. Mốc 50% có trong bộ công cụ nhưng không sinh trực tiếp từ tỷ số của dãy Fibonacci. Câu tự kiểm tra: dời đáy A lên mức giá khác thì các vùng hồi thay đổi thế nào. (B10 02:09, 02:47)

### 9.6. Sai lầm khi kéo Fibonacci theo hai điểm nhìn thấy

Theo thầy đây là lỗi "gần như 100% người học TA mắc": chọn một điểm mình thấy, chọn tiếp một điểm khác mình đang thấy, kéo công cụ Fibonacci và tin các vạch sinh ra. Công cụ luôn vẽ được các vạch từ bất kỳ hai điểm nào, kể cả khi hai điểm thuộc hai pha khác nhau. (B10 02:05)

Vì sao sai: tại thời điểm t đang đứng, người kéo không biết chu kỳ thực của mã, chỉ tin vào thứ mình đang thấy, mà thứ đang thấy là thứ "nhà cái đang cho mình thấy". Mọi vạch kéo ra là áp đặt bằng con mắt của mình lên chuỗi giá quá khứ, không gắn với ý đồ, chiến lược và tính chu kỳ của người tạo giá, nên không dự đoán được gì. Hình vẽ: trục ngang với vạch t, vùng bên phải t là các khả năng chưa xảy ra. (B10 02:06)

Lưu ý phương pháp (biên soạn): nếu chọn mốc bằng thông tin xuất hiện sau t rồi trình bày như dự báo tại t thì đó là lợi thế nhìn lại. Khi thử một phương pháp phải cố định dữ liệu có trước thời điểm lập giả thuyết. (B10 02:06)

**Cách làm đúng theo thầy:** trước hết đoán được người tạo giá đang muốn gì, tức xác định mã đang ở đâu trong quy trình đè, gom, đẩy, xả; sau đó mới chọn đầu mút để đo. Kéo công cụ mà không có bước này thì "không khác gì thầy bói xem voi". (B10 02:08)

Thầy chê lối lý luận trong sách: "Fibonacci thế này thì khả năng điều chỉnh 23%, nếu về 38% thì...". Theo thầy, mã đã điều chỉnh tới 0,382 (38,2% của nhịp đo) thì thường không còn cơ hội gì; sách bảo đó là ngưỡng hỗ trợ mạnh để bắt đáy ăn nhịp hồi, nhưng thực tế giá xuyên qua 38,2%, xuống 50% rồi đi tiếp. Các mức hồi chỉ là giả thuyết để kiểm, không phải kết luận. (B10 02:09)

Gốc tâm lý của lỗi: người dùng áp đặt ý chí và cái tôi lên đồ thị, tin vạch mình kẻ là đúng rồi "phán" tương lai. Thầy cũng cảnh báo "điểm đẹp nhìn lại": mức giá đẹp trên hình khi nhìn lại chưa chắc là mức người ta nhận ra hoặc mua được lúc đó; đừng nghĩ mình mua được đúng đáy, nhiều khi phải chấp nhận mua ở giữa vùng vì không đoán trước được ý đồ người lái. (B10 02:10, 00:53)

Về phía Elliott theo hai trục (xem chương 10): sai lầm phổ biến là mở biểu đồ giá, kéo công cụ rồi đếm sóng theo hình giá đã có, kiểu "thầy bói mù"; làm vậy là bị giá dẫn dắt, mỗi lần có đỉnh đáy mới lại đổi cách đếm. Fibonacci máy móc cũng không bắt được đoạn đè gom: sau khi đánh xong một sóng đẩy, tạo lập lại đè, vừa đè vừa gom; người chỉ kéo đường kiểm tra kiểu "đỉnh này không được vượt mức 1, 2, 3" gần như mất trọn đoạn đè gom ở dưới. (B2 02:07; B11 01:30)

Và khi đã vào giai đoạn xả: tay to không quan tâm tỷ lệ Fibonacci của thời gian xả, chỉ quan tâm bán được, khớp được, vừa bán vừa đỡ vừa kéo nhẹ để nhà đầu tư hấp thụ hết hàng. Thầy nói "nhiều bạn máy móc ghê, đoạn này không cần Phi-bô Phi-bê gì"; Fibonacci là để hiểu, chơi cho vui; cái thật sự là "bí mật tâm pháp" chỉ thế, còn vào chiến trường còn nhiều thứ nữa. (B11 02:21)

### 9.7. Fibonacci theo trục thời gian

Fibonacci theo trục thời gian là điều hầu như người Việt ít ai quan tâm, và chính vì không nắm được nên không đếm được chu kỳ. (B2 02:06)

Công cụ "Fibonacci vùng thời gian" (trong menu TradingView, cạnh các nhóm Fibonacci, cung Gann, quạt) dựng các vạch đứng theo quy luật Fibonacci trên trục thời gian, giống hình tán cây toả ra. Nó trả lời câu hỏi "khi nào" (nhịp đã chạy bao lâu, vùng thời gian nào dễ đổi nhịp), khác câu hỏi "giá lùi bao nhiêu" của Fibonacci theo giá. (B10 02:17)

Cách dùng theo thầy: chỉ kéo trên một đoạn đã hoàn thành (ví dụ từ đầu đến cuối đoạn nền); công cụ chiếu ra các mốc thời gian phía trước, trong đó có mốc "có khả năng đảo chiều". Đang đứng giữa đường thì chỉ ước được một vùng có thể xảy ra điều chỉnh, không biết mốc chính xác. Riêng đoạn giá chạy tiếp sau khi một chu trình hoàn tất là "vô định", không ai đoán được. (B10 02:18)

### 9.8. Hệ toạ độ hai chiều thời gian - giá

Cách thầy đề xuất: kẻ các vạch dọc là các mốc Fibonacci trên trục thời gian (các cửa sổ thời gian), kẻ các đường ngang là các mức Fibonacci theo giá, rồi đặt đường giá lên lưới đó để xem các nhịp có giao đúng các mốc không và có nằm trong phạm vi chu kỳ không. Chu kỳ bám theo các mốc Fibonacci trên trục thời gian; phạm vi giá đi theo khung do các mốc thời gian định ra. Thầy nói đây là "tâm pháp" mà dân giao dịch forex hay dùng. Buổi học chỉ nêu logic, chưa cho bộ tham số. (B2 02:08)

Thầy cũng nhấn: phải biết mẫu hình và các chu kỳ rồi mới lồng ghép được; giáo trình đại học hầu như không dạy Elliott, nhiều người chỉ lấy đường giá rồi vẽ theo ý chí của mình. (B2 02:11)

## 10. Sóng Elliott

### 10.1. Từ tỷ lệ vàng sang sóng giá

Hỏi đáp buổi 2: phần chu kỳ giống sóng Elliott, nhưng làm sao biết sóng nào lớn, sóng nào nhỏ? Thầy đáp: chu kỳ nền kinh tế có quy luật cỡ 10 năm; còn sóng Elliott về bản chất gắn với dãy Fibonacci, và dãy này luôn tạo các lớp lồng nhau. (B2 02:05)

Slide "Elliott Waves / Fibonacci Golden Ratio": cấp lớn nhất gồm pha tăng 5 sóng đánh số 1-2-3-4-5, sau đó pha điều chỉnh 3 sóng A-B-C. Phân rã xuống cấp nhỏ hơn có các số đếm 3, 5, 13, 21; chân hình ghi "89 Impulse Waves" và "55 Corrective Waves". Biên soạn tính lại: các số đếm đều thuộc dãy Fibonacci, 5 + 3 = 8, 21 + 13 = 34, 89 + 55 = 144; chỉ so số đếm trong cùng một cấp sóng. Số 89 và 55 là số đếm minh hoạ, không bắt buộc cho mọi mã. (B11 01:19, 03:49)

### 10.2. Cách thầy nhìn sóng

- Thầy phê bình cách dạy thông thường: "phang" hình Elliott vào rồi nói, người học không hiểu từ đâu ra. Theo thầy không cần bận tâm đánh số 1, 2, 3, 4, 5 rồi 6, 7, 8; thực chất chỉ chia hai bộ: sóng đẩy và sóng giảm (điều chỉnh). Có một quy luật tổng, và trong mỗi sóng tổng lại có các sóng nhỏ. (B11 01:19)
- Sóng lồng sóng như búp bê Nga: trong một sóng nhỏ lại ẩn một cấu trúc sóng nữa, mở ra con nào cũng giống y chang con lớn. Đây là tính đệ quy của tỷ lệ vàng áp vào giá. (B11 01:20)
- Thầy phản đối dùng Elliott hay Fibonacci một cách máy móc: người vẽ đang mặc định thị trường tuân theo chu kỳ dựa trên niềm tin vào số phi, tỷ lệ vàng, và mặc định như vậy nhiều lúc sai. Cách thầy đề xuất: dùng phân tích vĩ mô để xác định trạng thái và chu kỳ lớn trước, sau đó mới dùng Elliott, Fibonacci để hiện thực hoá thành các chu kỳ nhỏ và điểm quan sát cụ thể; phối hợp như vậy độ chính xác tăng (theo thầy, chưa có kiểm định xác suất). (B3 00:48)
- Thầy còn nói Elliott "chỉ làm mình quay cuồng": đếm sóng khi giá chưa đi hết thì có rất nhiều cách gán nhãn, "bó tay luôn", người cứ loay hoay theo sóng Elliott hay mắc bẫy. Nắm chu kỳ thì hay hơn đếm sóng. (B10 00:52)

### 10.3. Sai lầm lớn nhất: bám sóng nhỏ

Theo thầy, sai lầm "gần như 100% ai cũng dính" là bám theo các con sóng nhỏ nên thiếu tầm nhìn tổng thể, chỉ nhảy vào nhảy ra ăn chút ít trong sóng nhỏ. Người nhìn ra sóng to thì tỉnh hơn, chờ tới cuối đoạn tăng của sóng to mới ra; người giỏi hơn nhìn cấp cao hơn nữa và chờ cuối sóng cấp đó mới ra. (B11 01:20)

Nguyên nhân do cách học và cách dạy: không ai dạy về chu kỳ và quy luật tự nhiên, nên người học chỉ bám vào giá, ngồi học nến, nhìn đồ thị nến, MACD rồi nhảy sòn sòn theo từng tín hiệu ngắn và "trật hết". Thầy xếp đẳng cấp theo cấp sóng nhìn được: cấp thấp nhìn sóng nhỏ, cấp cao nhìn sóng lớn; ai luyện được nhìn ra cấp trên cùng thì "cực kỳ kinh khủng"; người chỉ nhìn sóng nhỏ luôn là người nhảy nhót và mất hàng. (B11 01:21-01:22)

Thầy tự thuật: khi mới áp dụng chỉ báo, ông bị "sóng nhỏ lừa": chỉ báo bảo nhảy ra thì ra, bảo nhảy vào thì vào rồi "chết", vì chỉ ăn rồi nhảy short trong sóng nhỏ mà không hiểu sóng lớn. Sau đó ông phá bỏ quy luật cũ, nhìn lại cấu trúc sóng lớn. (B11 03:20)

### 10.4. Ba lớp quy luật ứng với ba cấp sóng

Thầy vẽ thêm lên slide Elliott: cấp trên cùng là quy luật của tự nhiên, thể hiện thành niềm tin, ý tưởng tăng trưởng, nền kinh tế phục hồi; cấp giữa là quy luật của nền kinh tế; cấp dưới cùng là ý chí của đám đông, của đội lái, big boy, nhà tạo lập. Thầy ghi FA cạnh hình để nói phải ghép với phân tích cơ bản. (B11 01:29)

### 10.5. Sóng Elliott trong thực hành

- Slide "Figure 4-1" (Elliott Wave International, ghi January 2008): sóng 1-2-3-4-5, A-B-C, nhãn cấp lớn (1), (2), đường ngang tham chiếu .618 và đường nét đứt "Protective Stop". Thầy chỉ chiếu thoáng, không giảng cách đặt dừng lỗ hay tỷ lệ .618. (B11 01:58)
- Học viên đếm sóng 1 (lên), 2 (xuống), 3 (lên), 4 (xuống), 5 (đang đi đoạn cuối), thầy xác nhận; thầy yêu cầu kéo phạm vi về đoạn nền dài bên trái và vẽ vùng gom bằng một băng có hai biên cho cả đoạn nền, thêm một đường nữa ở dưới nếu cần (ba đường "đủ rồi"). Trong sóng lớn có sóng nhỏ (ví dụ trong đoạn từ 3 xuống 4) nhưng "đừng bao giờ nhìn nhỏ nữa", đừng quan tâm sóng nhỏ để khỏi mất sóng lớn. (B11 02:36)
- Học viên so chiều cao sóng 1 với sóng 5, nhận thấy hai nhịp gần tương đồng nên sóng 5 sắp xong; đây là phép so sánh trực quan, không phải quy tắc bắt buộc sóng 5 bằng sóng 1. (B11 02:41)
- Một nhịp giảm có thể thuộc cấp khác nhau: điều chỉnh nhỏ trong xu hướng lớn hay đổi cấu trúc cả chu kỳ. (B11 01:20)
- **Bài luyện 16** (biên soạn): che phần bên phải biểu đồ lịch sử tại một ngày, chỉ giữ thông tin trước đó; ghi cấp sóng, vùng nền, volume, kịch bản chính, kịch bản khác, dấu hiệu bác bỏ; lưu bản vẽ trước khi mở phần sau. (B11 02:42)

| Mục ghi | Câu hỏi |
|---|---|
| Mốc quan sát | Lúc đó thật sự đã biết những gì? |
| Kịch bản | Vì sao kỳ vọng đường đi này? |
| Dấu hiệu phản bác | Diễn biến nào cho thấy cách đếm hoặc luận điểm sai? |
| Ngày xem lại | Khi nào đối chiếu thay vì chờ vô hạn? |
| Kết quả | Đúng điều kiện nào, sai điều kiện nào, có bỏ qua ngoại lệ không? |

- Bài tập dự phóng: vẽ tay đường đi tiếp rồi lưu lại, so với diễn biến sau, để không chọn cách đếm sau khi đã nhìn thấy toàn bộ lịch sử. (B11 02:18)
- Thầy yêu cầu: lấy tất cả các mã mình cảm nhận được, phân tích y chang theo khung giai đoạn này (đè, gom, đẩy, xả); gần như mọi mã đều theo quy luật này, "không chạy đâu được". Các kỹ thuật cao hơn là "kỹ thuật của anh lái đò", ví như kỹ thuật phóng tàu lên vũ trụ nhưng đều bắt đầu từ nền tảng này. (B11 02:23)

## 11. Độ rộng thị trường, luân chuyển ngành và đối chiếu liên thị trường

Nguồn của nhóm này chỉ có các ý sau, chưa có bài giảng riêng về phân tích liên thị trường.

- **Độ rộng thị trường.** Chỉ số tính theo vốn hoá có thể được vài mã trụ nâng lên trong khi phần lớn cổ phiếu nhỏ đang yếu. Cần đối chiếu đường chỉ số với số mã tăng giảm, đường chỉ số ngành và thanh khoản để biết biến động tập trung hay lan rộng. (B2 01:29)
- **Đồ thị luân chuyển tương đối (Relative Rotation)** trên phần mềm Optuma: mỗi ngành là một điểm chạy thành quỹ đạo, chỉ so sức mạnh ngành với chỉ số chung. Thầy cho rằng công cụ này cũng chỉ dùng dữ liệu quá khứ, "có mua về cũng chỉ cho vui" nếu người dùng không hiểu chu kỳ; phải kết hợp thêm biến cơ bản (P/E, EPS). Theo thầy, đây là chỉ số có độ trễ chứ không dẫn dắt. (B2 01:15, 01:50) Xem thêm [Ngành và luân chuyển ngành](03-nganh-va-luan-chuyen-nganh.md).
- **Tự tính dòng tiền ngành từ dữ liệu giá:** lấy chỉ số ngành và chỉ số chung cùng ngày, chuẩn hoá về 100, lưu đường đi theo thời gian. Thầy nói sau này ra ứng dụng riêng sẽ chia sẻ. (B2 01:50)
- Thầy đã dùng Bloomberg và Thomson Reuters, hiểu các nhược điểm rồi cải tiến, đưa tư duy riêng vào công cụ của mình; chỉ giữ những gì cảm nhận là hữu ích cho đầu tư. (B2 01:52)
- **Ghép tầng (cách học viên làm):** một học viên làm theo thứ tự lọc kỹ thuật tìm nhóm, kiểm tra sector và vĩ mô có ủng hộ không, rồi check FA và câu chuyện (sơ đồ TA -> Sector -> Vĩ mô). Một học viên khác lọc "giá 5 đến giá 20" (đơn vị không rõ) trong ngành dẫn đầu, xem chất lượng nền giá và hướng đồ thị trước khi đọc báo cáo, loại mã có nền đi xuống. (B17 01:41, 02:00)
- **Báo cáo mẫu** ghép đồ thị TA, tín hiệu máy, dữ liệu sở hữu và so sánh theo ngành; trang VNINDEX có dải vàng ghi VNINDEX và BUY (trạng thái lịch sử), các trạng thái UP, DOWN, FLAT, Close VNINDEX, Sell Signal, Volatility GARCH(1,1) (trục biến động khác thang với điểm chỉ số, không lấy chênh lệch chiều cao giữa hai thang để suy số), CCI (đường cam), MACD, tỷ suất sinh lợi từng kỳ. Thầy nối với dự báo, phân tích rủi ro, quản lý tài khoản, tài sản và danh mục: phân tích doanh nghiệp để biết đang cân nhắc tài sản nào, phân tích chuỗi thời gian để theo dõi trạng thái; hai nhóm phục vụ quyết định khác nhau. (B7 03:43, 03:47)

## 12. Beta, hồi quy, kiểm thử và giới hạn của mô hình chuỗi thời gian

### 12.1. Slope và hồi quy trong TA

Ở buổi 1, thầy giới thiệu khái niệm slope (độ dốc) trong phương trình hồi quy dùng trong TA: khảo sát độ dốc của chỉ số để biết góc lên xuống dài hay ngắn, nhanh hay chậm; ông dặn ghi chú để nối với phần TA ở các buổi sau. (B1 01:26)

### 12.2. Beta là hệ số góc hồi quy, không phải "rủi ro"

Thầy hỏi beta là gì. Học viên Tống: beta đại diện rủi ro thị trường, ở Việt Nam lấy VN-Index làm chuẩn. Thầy sửa: hiểu beta là rủi ro là hiểu sai bản chất toán học; nói "mức tương quan, đồng biến của một cổ phiếu với thị trường" thì gần đúng hơn. (B10 01:44)

**Cách dựng.** Lấy chuỗi tỷ suất sinh lợi của cổ phiếu và chuỗi tỷ suất sinh lợi của thị trường cùng kỳ, xem chúng đồng pha hay nghịch pha bằng hồi quy tuyến tính y = ax + b, với x là lợi suất thị trường, y là lợi suất cổ phiếu. Hệ số góc a chính là beta. (Biên soạn bổ sung: trong hồi quy một biến, beta = hiệp phương sai của hai chuỗi lợi suất chia phương sai lợi suất thị trường; kết quả phụ thuộc chỉ số tham chiếu, tần suất và giai đoạn lấy mẫu. Tương quan và beta là hai đại lượng khác thang đo.) Hình bảng: công thức y = ax + b viết xanh, a được khoanh; hai đường dốc lên cạnh chữ "VN"; beta ở trái, alpha khoanh ở giữa. (B10 01:45-01:46)

**Quy trình tính.** Lấy giá P(t) từng phiên, đổi thành chuỗi phần trăm thay đổi r(t) = P(t) / P(t-1) - 1, rồi mới hồi quy để ra đường thẳng và beta. Chuỗi phải đủ dài, thường dùng 252 quan sát (số phiên của một năm). (B10 01:50)

**Cách đọc beta theo thầy.** Beta lớn hơn 1 là mã "ngóc đầu lên rất mạnh", chạy mạnh hơn thị trường; beta gần 0 là thị trường lên mà mã vẫn "phẳng lặng như mặt nước", không lên theo; beta âm là đi ngược chiều thị trường. Vì thế beta là công cụ lọc mã theo xu thế, không phải để né. Thầy kể những người học ở Mỹ về hay nói "mã beta cao không chơi vì rủi ro", còn ông thì "muốn ăn đậm phải là mã beta lớn hơn 1". (B10 01:46-01:47)

**Phần dư và alpha.** Phần lợi nhuận cổ phiếu mà biến động thị trường không giải thích được là phần dư của hồi quy. Từ đây sinh ý tưởng "săn alpha": người làm định lượng (quant) tìm cách bắt phần lợi nhuận riêng đó. Theo thầy cả ngành quant đi lên từ những mô hình gốc đơn giản như vậy. (B10 01:47)

Không thể suy beta chỉ bằng nhìn đường giá dốc của một mã; phải có chuỗi lợi suất của mã và của chỉ số cùng kỳ. Thầy thử vẽ kênh hồi quy lên đồ thị giá và lưu ý mỗi phần mềm cài thuật toán tính khác nhau nên kết quả giữa các phần mềm lệch nhau; khi lệch phải kiểm khung thời gian, chuỗi đầu vào, thang đo. Sau khi có đường hồi quy, người ta tính phương sai để gọi là "độ rủi ro": đó là mô tả độ biến động của các điểm quan sát quanh đường hồi quy, tức tổng khoảng cách từ điểm tới đường. Lý thuyết coi các điểm này phân phối ngẫu nhiên, nhưng theo thầy thực tế chúng không ngẫu nhiên mà có quy luật. (B10 01:48, 01:51)

**Bài tập beta** (biên soạn tính lại): giả sử mô hình ước lượng là lợi suất cổ phiếu = 0,5% + 1,5 x lợi suất thị trường + phần dư, tức beta 1,5 và hệ số chặn 0,5%. (B10 01:49)

| Lợi suất thị trường trong kỳ | Phần theo thị trường | Lợi suất cổ phiếu dự đoán khi phần dư bằng 0 |
|---|---|---|
| -1% | 1,5 x (-1%) = -1,5% | -1,0% |
| 0% | 0% | 0,5% |
| 1% | 1,5% | 2,0% |
| 2% | 3,0% | 3,5% |

Ở kỳ thị trường tăng 2%, nếu cổ phiếu thực tăng 5% thì phần dư kỳ đó là 5% - 3,5% = 1,5 điểm phần trăm. Hệ số chặn (0,5%), beta (1,5) và phần dư (1,5 điểm phần trăm) là ba đại lượng khác nhau. (B10 01:49)

Câu tự kiểm tra: hai mã tăng giống nhau trên đồ thị giá có nhất thiết cùng beta không, cần chuỗi nào để tính. (B10 02:47)

### 12.3. Hồi quy độ dốc của giá và khối lượng để lọc mã đang tăng

Chạy hồi quy xu hướng cho chuỗi khối lượng, cần độ dốc dương và càng lớn càng tốt; đồng thời kiểm độ dốc chuỗi giá cũng dương. Cả hai cùng dương thì cổ phiếu đang uptrend. Chữ "beta" thầy dùng ở đây (độ dốc của vol) là độ dốc của từng phép hồi quy theo thời gian, khác beta thị trường. Hình bảng ghi các chữ "Vol", "Trend", "slope", "Algo". (B10 01:53)

### 12.4. Phê bình mô hình chuỗi thời gian và ngưỡng quá mua

Thầy nhắc các mô hình dự báo chuỗi thời gian trong học thuật: ARIMA, GARCH, VAR, cùng các bài báo kể cả của người đoạt Nobel. Nhận xét: "tính cho vui, ý nghĩa thấp lắm". (B10 01:57) Ở buổi 2, thầy cũng nhắc mô hình ARIMA để dự báo chuỗi thời gian và nói ông tự sáng tạo cách lồng phương thức TA vào mô hình chuỗi thời gian để phát hiện điểm đảo chiều. (B2 00:37)

Lý do theo thầy: các mô hình này đặt trên nền xác suất, coi phần giá chưa giải thích được là nhiễu ngẫu nhiên và tìm cách khử nhiễu. Nhưng trên thị trường, người tạo giá không hành xử theo xác suất mà theo "ý chí" và quy trình có chủ đích: đè, gom, đẩy, phân phối, xả. Khi giá bắt đầu chuyển từ tích luỹ sang tăng, mô hình vẫn coi các bước tăng đầu là dao động ngẫu nhiên quanh mức cũ. Hệ quả: mọi hệ thống thiết kế theo lý thuyết đó đều bán ra rất sớm, vừa tăng là bán, thậm chí bán đúng lúc giá chuẩn bị chạy. (B10 01:58-01:59; xem thêm 6.5 về ngưỡng quá mua)

### 12.5. Kiểm thử và tối ưu

- Ở giai đoạn đã có phương pháp thì việc còn lại không phải tìm phương pháp mới mà là cải tiến dần: kiểm thử lại (backtest) tốt hơn, lọc nhanh hơn, tức quá trình tối ưu (optimize). (B10 01:36)
- Một mô hình có thể phản ứng khác nhau giữa các pha thị trường vì người tham gia và mức chú ý của đám đông thay đổi; nên tách giai đoạn chọn quy tắc khỏi giai đoạn kiểm thử, xem cả trường hợp bỏ sót lẫn báo sai. (B10 01:38)
- Giả định giao dịch phải thực hiện được: tín hiệu đẹp nhưng lệnh không khớp thì không tạo được kết quả mô hình dự kiến; ghi lại giả định thực thi (giá có thể khớp, khối lượng, mức chịu biến động, thời gian chờ) để kiểm thử. (B10 02:47)
- **Hiệu ứng theo tháng và ngày trong tuần:** thầy lấy ví dụ nhận xét kiểu "thứ Hai hoặc thứ Tư mua, thứ Sáu bán" như điều có thể xuất hiện trong thống kê quá khứ (đồ thị cột 12 vị trí tháng, vài cột nổi trội). Buổi giảng không nêu tập mẫu, thời gian và chi phí giao dịch. Khi đọc dạng biểu đồ này cần biết số quan sát mỗi nhóm, cách tính lợi nhuận, và kết quả có lặp lại ngoài mẫu không. (B7 03:52)
- Thầy khuyên "đừng bao giờ chơi" nhóm 3 (phương pháp momentum, động lượng: giao dịch rất ngắn, tần suất cao, mỗi lần ăn rất nhỏ): đó là phương pháp tệ nhất ông từng thử nghiệm, kể cả ở thị trường thế giới, vì tỷ lệ lợi nhuận trên rủi ro quá nhỏ (theo thầy, không nêu số liệu). Ở bảng thầy đánh số: nhóm 2 là mô hình, thuật toán ("AI + TA"), nhóm 3 là momentum. (B10 02:12)

### 12.6. Hai lớp tín hiệu: bắt xu hướng và xác nhận hoàn tất đảo chiều

Phương pháp riêng thầy mô tả sơ lược (bí mật cá nhân, không có trong sách): lớp một dùng một mô hình toán để bắt xu hướng và dự báo điểm; lớp hai dùng một phương trình dạng parabol (đường cong hình cung, tên thuật toán nghe không rõ, nguồn chưa rõ) để bắt tín hiệu "hoàn tất đảo chiều của cả một chu kỳ". (B10 02:01)

Quy tắc phối hợp: lớp parabol có quyền cao hơn. Khi mô hình dự báo ngắn phát tín hiệu bán mà trên chu trình tổng thể đường cong chưa hoàn thành đảo chiều thì vẫn giữ hàng. Theo thầy, ghép hai lớp như vậy khắc phục bệnh bán sớm và hiệu quả chiến lược cao lên rõ. Nguồn không có công thức hay bảng kiểm định. (B10 02:02)

Thuật toán quan trọng nhưng muốn thiết kế phải có ba thứ: ý tưởng nghiệp vụ (cần máy tìm mẫu gì, trong bối cảnh nào), kinh nghiệm "chiến trường", và kiểm thử bằng máy tính. (B10 02:03)

## 13. Thuật toán lọc, bảng tín hiệu scan và phần mềm

### 13.1. Máy chỉ hỗ trợ để tìm

Mọi logic và suy luận đã đọc được thị trường thì có thể thiết kế thành thuật toán bất kỳ; công cụ máy móc và trí tuệ nhân tạo chỉ "hỗ trợ để tìm", khi đã lọc ra rồi thì "máy cơm" (con người) phải hoạt động và kiểm tra lại ở đoạn cuối. Thầy nói sách vở khác không dạy những điều này (theo thầy). Nếu đi sâu vào thuật toán thì "cả là một môn học", rất nhiều toán; thầy chỉ giới thiệu qua logic. (B10 02:30, 02:39)

Thầy nói cuộc chơi sau này là từ máy tính, "không thể dùng con người ngồi cơ hết"; hỗ trợ của máy tính "vô cùng quan trọng", nhưng các phần mềm, app nhà đầu tư đang dùng chỉ ở mức sơ cấp. Tổng thể thầy muốn máy theo dõi trạng thái thị trường và sự "xoay trục" của thị trường, đưa ra cho nhà đầu tư coi. (B12 03:05)

### 13.2. Khó nhất là định nghĩa hình

Thầy tự lập trình bộ lọc từ khoảng năm 2020, dùng nhiều ngôn ngữ lập trình để mô tả suy nghĩ thành điều kiện; các chỉ tiêu như đường trung bình, tỷ lệ tăng, khối lượng, các đường cắt nhau "ai làm cũng được", "chơi vui thôi", nhưng lọc mẫu hình thì khó. Thầy ví dụ các mã lọc được bằng bộ lọc cao cấp là nhóm đang điều chỉnh và nằm trong quá trình gom như DPM, CTG, CNG. (B12 02:53, 02:56)

Biên soạn tính lại: giao cắt chỉ báo dễ viết thành biểu thức nếu dữ liệu sạch; lọc nền tích lũy hay mẫu đảo chiều còn phải thống nhất đoạn quan sát, cách chọn điểm và điều kiện đi trước. Cách cụ thể hoá "đi ngang": chọn cửa sổ 20 phiên (giả định), đo biên bằng (cao nhất trừ thấp nhất) chia giá trung vị, thêm một cách đo độ dốc, chọn ngưỡng thử, lấy cả ví dụ bộ lọc nhận sai, đổi độ dài cửa sổ để xem độ nhạy, giữ phần sau mốc tách khỏi dữ liệu chọn ngưỡng. (B12 02:53, 02:57)

Thầy làm các báo cáo scan "cách đây mấy năm", cập nhật trong đêm: thay vì nhà đầu tư tự sàng, hệ thống trích lọc các mảng, xếp hàng các mẫu hình (đảo chiều...) và sẽ tích hợp thẳng vào app, tự động quét không cần thiết lập; sắp tới có đồ thị trực quan. (B12 03:00)

### 13.3. Bảng tín hiệu scan (báo cáo mẫu)

Báo cáo scan tín hiệu mẫu dạng PDF (dòng ngày thuộc tài liệu, không phải ngày ghi hình). Tên theo ảnh, dấu "-" là không có mã đọc chắc; mã trong cột là kết quả hiển thị ở báo cáo mẫu. (B12 03:01)

| STT | Tên tín hiệu | Mã nhìn được trong khung |
|---|---|---|
| 1 | TKAI Signal Buy | - |
| 2 | TKAI Signal Sell | - |
| 3 | Forecast BUY+ | ACL, AGF, VNINDEX |
| 4 | CCI và RSI OverSold Sideway UP | - |
| 5 | CCI và RSI OverBought Sideway DOWN | - |
| 6 | MACD Cross(9,12) | ABT, ACL, AGF, VNINDEX |
| 7 | SmartTrend UP | - |
| 8 | SmartTrend DOWN | - |
| 9 | TrendScore DOWN | - |
| 10 | TrendScore UP | ABT, ACL, AGF, VNINDEX |
| 11 | PSAR reverse Up | - |
| 12 | PSAR reverse Trend Down | AGF |
| 13 | Return/Risk > | ACL, AGF, VNINDEX |
| 14 | Return/Risk < | ABT |
| 15 | ARIMA Forecast UP (T+3) | ABT, ACL, VNINDEX |
| 16 | ARIMA Forecast Down (T+3) | AGF |
| 17 | TrendMACD Up | - |
| 18 | TrendMACD Down | ABT, ACL, AGF, VNINDEX |
| 19 | MACD Cross Signal UP | - |
| 20 | MACD Cross Signal DOWN | - |
| 21 | BB Upper Crossover | - |
| 22 | BB Lower Crossover | - |
| 23 | RSI OverSold và Trend Up | - |
| 24 | RSI OverBought và Trend Down | - |
| 25 | RSI OverSold Sideway Accum | - |
| 26 | RSI OverBought Sideway | - |
| 27 | CCI TREND UP | ACL, VNINDEX |
| 28 | CCI TREND DOWN | ABT, AGF |
| 29 | Chaikin money flow UP | - |
| 30 | Chaikin money flow DOWN | ABT, ACL, AGF, VNINDEX |
| 31 | ADX Up | ABT, AGF |
| 32 | ADX Down | ACL, VNINDEX |
| 33 | N/W (chưa rõ nghĩa) | - |
| 34 | N/W (chưa rõ nghĩa) | - |

Các cột của bảng scan gồm số thứ tự, hình minh hoạ tín hiệu, tên tín hiệu, mã xuất hiện, ghi chú. Video không cho công thức, ngưỡng hay quy tắc gán nhãn của từng tín hiệu; không thể tái tạo thuật toán chỉ từ bảng này. (B12 03:01)

Trang tổng hợp AIQUANT (đầu đề "THẦN KINH AI SYSTEM"), lướt nhanh: (B12 03:01)

| Khối | Nhãn đọc được | Cách đọc |
|---|---|---|
| Xu thế theo kỳ | Ngắn hạn, trung hạn, dài hạn | Ba thước màu riêng, một số chữ số nhỏ không rõ |
| Trạng thái | Strong Up Trend + Up Trend, No Trend, Strong Down Trend + Down Trend | Ba thước bên dưới, kết quả mẫu |
| Phạm vi | Thế giới, Chỉ số Index, Chỉ số hàng hoá, HOSE, HNX, UPCOM | Nhãn phân phạm vi, chưa thấy cách lấy dữ liệu |
| Cảm nhận thị trường | VN's Sentiment Market, Thế giới | Thanh ngang hiển thị dải mức |

### 13.4. Phần mềm

- **Bài khảo sát đầu buổi 4:** thầy hỏi học viên dùng phần mềm gì; các câu trả lời nghe được có TradingView và một số tên khác (nghe như FireAnt, nguồn chưa rõ). Thầy nhận xét học viên chủ yếu dùng phần mềm miễn phí và thông báo phần thực hành sẽ dùng **AmiBroker** cài trên Windows. (B4 04:09)
- **Môi trường:** thầy không dùng Mac nên không hướng dẫn cài trên Mac; học viên dùng Mac tự tìm cách hoặc mượn, mua một máy Windows cũ. Theo thầy AmiBroker rất nhẹ, laptop Windows cũ rẻ tiền cũng chạy được. (B4 04:10)
- **Nguồn gốc AmiBroker theo lời thầy:** do một nhà đầu tư cá nhân rất giỏi (lời thoại nghe như người Ba Lan, nguồn chưa rõ) tự viết bằng C++ để dùng cho chính mình rồi mới bán cho các nhà đầu tư khác; giá bản quyền thầy đánh giá là rẻ và được cập nhật lâu dài (con số giá và thời hạn giấy phép trong lời thoại không nhất quán, nguồn chưa rõ). Học viên dùng bản nào là quyền của họ, thầy chỉ hướng dẫn cách sử dụng. (B4 04:11)
- **Lý do chọn AmiBroker:** khả năng tuỳ biến rất nhiều, tự viết công thức và bộ lọc thay vì chỉ dùng những gì hiển thị sẵn. Thầy nhận xét phần lớn nền tảng xem chart khác thực chất nhúng biểu đồ của TradingView; mỗi công cụ có ưu nhược điểm. (B4 04:12)
- **Bộ lọc AmiBroker (B17):** AmiBroker dễ cài (có file cài trên mạng) nhưng tự viết bộ lọc phải học AFL (ngôn ngữ công thức của AmiBroker), rất mất thời gian và dễ "sa đà vào kỹ thuật quá, mất cảm nhận". Thầy muốn lớp ưu tiên khả năng đọc và cảm nhận bảng giá; ai muốn thì thầy gửi file cài. (B17 01:30)
- **Replay:** TradingView có chế độ Replay, AmiBroker cũng có (xem chương 15). (B17 01:29)
- **FireAnt:** biểu đồ ngày trên FireAnt được học viên dùng để vận dụng kế Đả thảo kinh xà (xem chương 14). (B13 03:12)
- **Optuma:** đồ thị luân chuyển tương đối (xem chương 11). **Bloomberg, Thomson Reuters:** thầy từng dùng. (B2 01:15, 01:52)

## 14. Thực hành đọc biểu đồ qua các ví dụ trong lớp

Phần này gom các ví dụ mã cụ thể thầy và lớp phân tích, tách ba lớp thông tin: dữ liệu thấy trên hình, kỳ vọng được nói trong lớp, suy luận về người tham gia. (B15 02:14)

| Lớp thông tin | Ví dụ | Cách ghi nhận |
|---|---|---|
| Dữ liệu thấy trên hình | Giá, volume, các nền và vùng dao động của QNC, HHV, BCG | Mô tả vị trí tương đối; chỉ chép số đọc chắc |
| Kỳ vọng được nói trong lớp | Vùng ba mươi mấy, 35-36 hoặc 42 của HHV; ví dụ lời 15% sau vài phiên | Giữ người nói, thời điểm và điều kiện; chưa phải mục tiêu đã kiểm chứng |
| Suy luận về người tham gia | Nhả hàng, đảo hàng, test, phản ứng khi có người bám theo | Là nhận định hoặc câu chuyện của thầy |

### 14.1. Nền tích lũy, thử cung và volume (ví dụ FireAnt, B13)

Biểu đồ ngày trên FireAnt (tên mã mờ, nguồn chưa rõ, không gán mã): vùng đi ngang kéo dài nhiều tháng, các nhịp hạ xuống rồi hồi, những lần "thử kéo". Thầy gọi các nhịp đó là kiểm tra: kéo lên gặp hàng bán xuống thì còn khó khăn, sau đó lại hấp thụ (gom) rồi thử lại (theo thầy, cách diễn giải hình giá, biểu đồ cuối ngày không xác nhận được danh tính người đặt lệnh). Thứ tự đọc: nền dài, các nhịp thử, rồi giai đoạn tăng. (B13 03:12)

Khi thử nhiều lần mà thấy hàng bên ngoài không xuất hiện nhiều, bên tổ chức nhịp giá có thể tự tin hơn để đưa giá đi (theo thầy). Phải đánh giá toàn bộ quá trình chuẩn bị và phản ứng của nguồn cung, không chỉ một cây nến cuối. (B13 03:15)

Kéo biểu đồ lùi xa hơn để tìm điểm bắt đầu ý tưởng gom: nhìn những lần đạp xuống rồi bị hấp thụ, những lần đánh thử và các vùng quay về tích lũy. Nếu đếm quá muộn thì bỏ sót một phần chuẩn bị; điểm bắt đầu quan sát ảnh hưởng cách hiểu lượng tích lũy. Giả thuyết của lớp: đã có lần bên kéo muốn đưa giá đi nhưng gặp điều kiện chưa thuận (thị trường chung hoặc một nguồn hàng khác bán ra); bên đó lại dìm xuống, hấp thụ rồi thử tiếp, kế hoạch không phải lúc nào cũng đi một đường thẳng. (B13 03:17-03:18)

Một học viên: sau hai cột đỏ volume lớn, các cây tiếp theo volume không còn lớn, nên hiểu hàng ngoài không nhiều và bên kéo tiếp tục đẩy. Thầy đồng ý trong ví dụ này: một nhịp hạ quyết liệt mà không lôi được nhiều cung có thể là phép thử, sau đó giá bị kéo ngược. Đây là giả thuyết của lớp, không phải mọi cây đỏ volume nhỏ đều là rũ hay bảo đảm bật lên ngay. (B13 03:20)

Hỏi đáp quan trọng: học viên hỏi từ vùng giá khoảng 5 lên 8 rồi rung là chưa dài; nếu lên khoảng 12-13 mà rung mạnh thì có nên thoát, và có cộng volume để phân biệt rũ với ra hàng được không. Thầy: khi giá đã vào giai đoạn chạy thì không thể cộng volume theo cách của nền gom (xem 4.4). (B13 03:21)

Khi biểu đồ có nhiều nhịp cao, hình dáng giống vai đầu hoặc cụm núi: thầy nói trong tình huống ấy bản thân có thể đã ra để an toàn vì thấy dấu hiệu phân phối, dù nhịp và volume còn được giữ khá khéo (theo thầy). Học viên nhắc nguyên tắc phần trước: tập trung hai nhịp mạnh ban đầu, những nhịp sau khó thì bỏ để tìm cơ hội khác. Đây là kế hoạch quản lý vị thế của thầy, không phải quy tắc phải bán mọi đồ thị tương tự. (B13 03:23)

Từ ví dụ DIG thầy nói về chữ "tích" và "phân" (tích lũy và phân phối): nhà phân tích kỹ thuật phải học đọc để phân biệt hai pha này; nền gom lâu và chuẩn bị trận địa lâu (lời thoại nhiễu). (B13 03:32)

### 14.2. Các biểu đồ khác ở buổi 13

- **CTG:** lớp khoanh các vùng đỉnh, các lần hạ thấp, khu vực hồi gần nhất và một số cột volume; có nét phác của lớp ở vùng chưa có giá bên phải. Cột volume lớn trong phiên hồi chưa chắc là gom (xem 4.4). (B13 03:41-03:42)
- **GAB:** đường giá dựng mạnh rồi đi gần ngang ở vùng cao, các cột volume sau nhịp đầu thưa và thấp hơn; thầy đánh giá thanh khoản kém. (B13 03:45)
- **LHG:** hai biên xanh khoanh nền dài, các bậc tăng, vùng cao đóng khung nghiêng và khoanh nhiều dấu đỏ, một cột khối lượng được khoanh. Tín hiệu thầy đọc là sự thay đổi của cách đi giá và lượng ở vùng cao, không phải một mức bán duy nhất áp dụng cho mọi người. (B13 03:50)
- **CMX:** nền nhiều tháng được kẻ biên ngang đỏ, đường giá vượt lên rồi có các đỉnh và nhịp hạ trong vùng mới; chữ "Game tăng vốn" do lớp ghi. (B13 03:52)
- **L14:** thầy nhắc trong so sánh về lối kéo giá thốc; L14 cũng xuất hiện ở hình trước với nền rất thấp rồi nhịp tăng dốc (mã chưa rõ, nguồn chưa rõ). (B13 03:40)

### 14.3. Buổi 9 - 12

- **PDR:** đọc vùng đi ngang sau nhịp tăng bằng cách đặt khối lượng, số lần thử cản, độ sâu nhịp lùi và phản ứng khi quay về nền vào cùng một trình tự; giá có thể giữ trong biên một thời gian trước khi đổi hướng. (B9 03:00)
- **C4G (B12):** một học viên đọc nhịp đầu là gom, một lần lùi rồi gom tiếp, nhịp tăng cuối năm, vùng hiện tại còn gom; học viên khác đọc là nhả hàng ở nhịp trước, đang ra nốt hàng, có thể giật lên rồi hạ dần, tích lũy rồi mới đánh lại quý II-III. Thầy lưu ý cùng một đồ thị dẫn tới hai kịch bản vì cách đặt điểm bắt đầu và nhận định thị trường khác nhau. Tiêu chí kiểm tra (biên soạn): độ dài nền, vị trí cột volume lớn, phản ứng giá sau nhịp giảm, còn giữ biên cũ hay không. Khi so mã cần thống nhất khung ngày hoặc tuần, tách cấu trúc giá khỏi kết quả kinh doanh ngành. (B12 02:11-02:13, 02:35)
- **VN-Index dự phóng (B14):** trên một biểu đồ dự báo phải tách ba lớp: (1) nến và cột khối lượng là dữ liệu nền; (2) các nhãn "Phase A", "Phase B", "Phase C" là chú thích đặt lên biểu đồ; (3) đường cong, hộp, mũi tên, kênh đỏ và xanh là nét vẽ thêm. Đường ở vùng thời gian chưa có nến là dự phóng, không phải diễn biến đã xảy ra. Video không giảng tiêu chí hoàn thành từng pha A/B/C, và tên mẫu hình chính thức không nghe đủ rõ. Khi phóng hoặc dịch biểu đồ, các đường kéo dọc và chéo trông khác đi; phải đọc con số cùng lời giới hạn của người trình bày, không chọn một điểm chạm của nét vẽ làm mức dừng chắc chắn. Thầy cho phóng ra lịch sử nhiều năm để so tỷ lệ và hình dung sức ép của một nhịp giảm; không gán mọi điểm của nét đỏ vào dữ liệu lịch sử, không lấy chiều dài nét vẽ làm phép tính phần trăm. Các nét đỏ lùi xuống và hồi lên chỉ là trao đổi giữa người học và giảng viên, không do phần mềm hay công thức tự sinh ra, không có kiểm định. (B14 01:40-01:45)

### 14.4. Buổi 15 - 17

- **MVC (B15):** đọc biểu đồ ngày theo cấu trúc: đoạn nền bên trái, nhịp đi lên ở giữa, cụm dao động sau đỉnh bên phải; cột khối lượng đọc theo đúng vị trí thời gian của giá. Một cấu trúc giống nhau không bảo đảm kế hoạch phía sau bất biến: hành vi của những người cùng tham gia (ví dụ người ngoài ôm quá nhiều hàng) có thể làm bối cảnh đổi. (B15 02:02-02:03)
- **VNM:** biểu đồ đi ngang hoặc giảm nhiều năm (từ 2018) không hợp với đầu cơ theo nhịp (xem 5.7). (B15 02:30)
- **GIC:** dải giá đi ngang rất hẹp nhiều phiên kèm volume "kỳ cục", thầy đọc là cổ phiếu "tự đánh với nhau", giao dịch chủ yếu qua lại giữa các tài khoản cùng nhóm; nhìn báo cáo doanh nghiệp là kiểm tra được ngay (theo thầy). Một vòng khoanh quanh vùng đi ngang chỉ xác định vùng cần chú ý, chưa giải thích nguồn lực tạo ra giá; không thể mua chỉ vì nhận ra một vùng đi ngang. (B15 02:31)
- **CPH:** phần khối lượng gần như không có cột đáng kể; phải hỏi lượng đối ứng trước khi nói tỷ lệ tăng kỳ vọng. (B15 02:32)
- **FLC (B17):** bài tập Replay (xem chương 15). (B17 01:30)

## 15. Cách luyện tập

### 15.1. Vẽ tay và vẽ ít

- Thầy không thích công cụ vẽ có sẵn vì phải chấm từng điểm một cách máy móc; khi không tự vẽ thì người học không tăng được trí nhớ, logic, bị phụ thuộc công nghệ, khả năng cảm nhận kém đi. Khi nhìn bất kỳ đồ thị nào phải nhìn tổng thể các "đường mạch" của nó trước. (B10 00:40)
- Kéo công cụ qua hai mốc A, B là ra ngay hình và tỷ lệ, "cực kỳ máy móc", rồi giá chạy khác lại phải kéo chỉnh. Vẽ tay buộc mình tự chọn đoạn đang so sánh, mốc đổi nhịp, và mới so được đoạn này với đoạn kia. (B10 01:00)
- Thầy khuyên đặt một bảng nhỏ cạnh màn hình, tự vẽ đường giá của thị trường hoặc một mã với các vùng cần quan tâm và ghi nguyên tắc tự rút ra (có thể vẽ trên máy). Vẽ tay buộc nói được đâu là diễn biến chính và vì sao chọn các điểm đánh dấu; thầy nói vẽ tay thì "cảm nhận rất rõ". (B17 01:28)
- **Vẽ càng ít càng tốt.** Thầy kể thời mới ra trường thử hết mọi loại đường, vẽ kín đồ thị đến mức không biết mình đang vẽ gì. Kết luận: người vẽ càng ít càng là đỉnh cao, không cần vẽ mà đọc được là cao nhất; nên chọn số ít yếu tố, tập vẽ tay và chỉ đánh dấu các điểm trọng tâm. (B10 02:20-02:21; B15 02:14-02:15)
- Cách vẽ của thầy: "tôi phân tích kỹ thuật chỉ vẽ đường cản (đường đen) ra ngoài, rồi vẽ đường tương lai, chấm hết"; càng hiểu thị trường càng hạn chế vẽ, nhiều đường chỉ làm rối mắt. Mỗi đường cần gắn một câu hỏi (giá có giữ nền không, có vượt cản không, có quay lại kiểm không). Khi thời gian trôi, đem diễn biến thật so với điều kiện đã ghi. (B9 02:53)
- Nét đánh dấu chỉ để xác định vùng, nhịp và câu hỏi đang phân tích; không để tên mô hình hay nhiều chỉ báo che mất sự tương tác mua bán. (B15 02:14)

### 15.2. Đường kịch bản và điều kiện xác nhận

Cách dùng đường kịch bản vẽ sang vùng trắng: lưu đường dự kiến và ghi điều kiện xác nhận (giá vượt mức nào, quay lại vùng nào, lượng tăng hay giảm); nếu diễn biến khác giả thuyết thì cập nhật ngay các phần dựa trên đường đó. (B9 03:06)

Bài tập ngầm của thầy: chọn mốc A, mốc B và khoảng giá cần giải thích; thử bỏ một nhịp nhỏ xem câu chuyện ở khung lớn có đổi không; với mỗi cách vẽ, ghi diễn biến nào củng cố giả thuyết và diễn biến nào buộc phải sửa. Ngoài ra nên ghi lại các mốc đã dùng để vẽ đường xu thế, để sau kiểm xem mình có dời đường cho khớp kết quả hay không. (B10 01:01, 00:37)

### 15.3. Replay và không nhìn trước đáp án

- **Replay** (TradingView có chế độ Replay, AmiBroker cũng có): mở một mã tại mốc quá khứ, cho dữ liệu hiện dần từng thanh, bấm dừng ở các điểm chuyển nhịp để tự phân tích với dữ liệu chưa đầy đủ. Tập phản xạ đúng thời điểm. (B17 01:29)
- **Bài tập Replay với FLC:** lùi về khoảng ba tháng trước, cho hiện thêm đúng một phiên mỗi lần; tại mỗi mốc ghi dự đoán trước khi bấm tiếp, đối chiếu tin đã xuất hiện đến ngày đó, xem dữ liệu mới củng cố hay bác cách hiểu cũ. Đừng nhìn toàn bộ đồ thị trước (nhìn hết rồi thì kết quả sau khiến ta đánh giá quá cao khả năng dự đoán). Thầy nói chính cách "mô phỏng lại" này giúp thầy nghĩ ra nhiều điều. (B17 01:30)
- **Vẽ trên trang trắng:** không mở biểu đồ có sẵn mà tự tưởng tượng và vẽ tiếp để tăng độ cảm nhận (xem 4.3). (B11 01:23)
- **Che phần bên phải biểu đồ** tại một ngày, ghi cấp sóng, vùng nền, volume, kịch bản chính, kịch bản khác, dấu hiệu bác bỏ (bảng ở 10.5). (B11 02:42)
- **Bài luyện đọc vòng vận động:** giữ nguyên hình biểu đồ và nói có mấy vòng; rèn luyện này "dễ, không khó". (B9 02:46)

### 15.4. Đọc nhanh và nhật ký

- Có thể đọc thử cấu trúc một mã chưa từng theo dõi ngay khi mở biểu đồ, bằng bộ câu hỏi cố định: đoạn nào giá đang được giữ, nhịp nào có dấu hiệu giằng co giữa các bên, thay đổi nào cho thấy lượng hàng đang chuyển tay. Thầy nói đọc nhiều thì dần hiểu "tâm pháp", đọc rất nhanh; nhưng tốc độ nhận xét không biến thành độ chắc chắn về danh tính hay ý định người khác. (B15 02:07)
- Phải kéo rộng biểu đồ để thấy cả nền dài phía trước lẫn nhịp mới: câu hỏi không phải phiên hiện tại xanh hay đỏ mà là nhịp hiện tại đứng ở đâu trong toàn bộ lịch sử vận động của mã (nền gốc, nhịp tăng, vùng dao động sau tăng). (B15 02:11)
- Cách luyện của thầy: lúc rảnh ngồi bấm hết mã này qua mã khác để xem biểu đồ. Với mỗi mã nên ghi lại chuỗi: nền ban đầu, nhịp tăng, các lần hồi, volume thay đổi thế nào và kịch bản đã dự kiến; so nhiều trường hợp để không lấy một hình duy nhất làm chân lý. (B15 02:20)
- Nên đọc giá như biểu hiện của cách người ta chơi và của tâm lý, rồi hỏi: ai đang có lợi ích, điều gì khiến người ngoài bán hoặc mua, vì sao giá được đỡ ở đoạn này mà không được đỡ ở đoạn khác; không trả lời bằng một tín hiệu giao cắt hay tên mẫu hình. (B15 02:26)
- Thông lệ của học viên Mỹ: vẽ đường giá để phác xu hướng hoặc vùng sau một nhịp tăng, đánh dấu ngưỡng phá lên và phá xuống kèm ghi chú nguyên nhân từng mốc, đặt cảnh báo giá về điện thoại; khi cảnh báo đến thì mở lại bối cảnh thị trường chung, tin doanh nghiệp, lịch công bố kết quả rồi mới quyết định. (B17 01:55)
- Phép luyện nhóm: lấy tất cả các mã mình cảm nhận được và phân tích y chang theo khung giai đoạn đè, gom, đẩy, xả (B11 02:23).

### 15.5. Bảng ôn tập "Đọc lại một biểu đồ theo trình tự"

Bảng do người biên soạn học liệu lập cho buổi 10. (B10 02:47)

| Câu hỏi | Dữ kiện cần ghi | Mốc học lại |
|---|---|---|
| Đang đọc công cụ và thời kỳ nào? | Mã, sàn, khung nến, phạm vi thời gian, đơn vị giá và khối lượng | B10 00:30:00 |
| Cấu trúc trước đoạn đang xét là gì? | Đỉnh, đáy, vùng đi ngang, đường xu hướng và phản ứng trước đó | B10 00:35:00 |
| Có kịch bản nào khác? | Điều kiện tiếp diễn, điều chỉnh hoặc đổi xu thế, dữ liệu làm mỗi kịch bản yếu đi | B10 00:40:00 |
| Vì sao mã vào danh sách theo dõi? | Tiêu chí lọc theo xu thế, ngành, FA và thanh khoản | B10 01:10:00, 01:30:00 |
| Chỉ báo đang đo gì? | Cửa sổ MA, cơ sở hồi quy beta hoặc mốc đầu cuối của phép đo | B10 00:25:00, 01:45:00 |
| Giả định giao dịch có thực hiện được? | Giá có thể khớp, khối lượng, mức chịu biến động và thời gian chờ | B10 00:55:00, 02:10:00 |

Năm câu tự kiểm tra kèm bài: (1) nến có thân tăng nhưng bóng trên dài cho biết điều gì trong phiên, và thiếu dữ liệu gì để biết thứ tự giá chạm đỉnh và đáy (bài OHLC); (2) nếu giá hiện tại giữ nguyên mà giá cũ bị loại khỏi cửa sổ thì MA có thể đổi hướng không (bài SMA); (3) hai mã tăng giống nhau trên đồ thị giá có nhất thiết cùng beta không, cần chuỗi nào để tính (bài hồi quy); (4) dời đáy A trong phép đo Fibonacci lên mức giá khác thì các vùng hồi thay đổi thế nào; (5) tín hiệu đẹp nhưng lệnh không khớp có tạo được kết quả mô hình dự kiến không (ghi lại giả định thực thi để kiểm thử). (B10 02:47)

## 16. Thứ tự kết hợp phân tích cơ bản với phân tích kỹ thuật

Thứ tự theo thầy, từ lớn đến nhỏ:

1. **Xác định trạng thái và chu kỳ lớn bằng vĩ mô trước**, sau đó mới dùng Elliott, Fibonacci để hiện thực hoá thành các chu kỳ nhỏ và điểm quan sát cụ thể. Phối hợp như vậy độ chính xác tăng (theo thầy, chưa có kiểm định xác suất). (B3 00:48)
2. **Nền tảng doanh nghiệp (FA) trước, kỹ thuật chọn thời điểm sau.** FA là nền tảng; TA bổ trợ quy trình, chọn thời điểm hành động. Thầy hẹn dạy cách kết hợp ở phần sau. Trên hình có chữ "FA = nền tảng" và TA được khoanh. (B4 02:00, 02:30)
3. **Xu thế là tiêu chí lọc số một**, rồi mới đến MA, khối lượng. (B10 01:17)
4. **Đọc thế, tâm lý, vị thế, rồi mới đến điểm vào và ra.** (B10 00:23)
5. **Ghép với phân tích cơ bản ở mỗi cấp sóng:** thầy ghi "FA" cạnh slide Elliott để nói ba cấp quy luật (tự nhiên, kinh tế, ý chí đám đông) phải ghép với FA. (B11 01:29)
6. **Công cụ rời không thay được đọc hành vi:** theo thầy chỉ có cách đọc hành vi kết hợp hiểu doanh nghiệp mới nhận ra vùng đang bị đè để gom. Mã đã đẩy tới mức người ngoài ôm quá nhiều hàng thì bối cảnh đổi. (B4 02:52; B15 02:03)
7. **Kiểm tra chéo bằng báo cáo doanh nghiệp.** Ví dụ dải giá hẹp kèm volume kỳ cục (GIC) là cổ phiếu "tự đánh với nhau", nhìn báo cáo là kiểm tra được. (B15 02:31)
8. **Thứ tự lọc của học viên** (thầy không phán xét riêng): TA tìm nhóm -> sector và vĩ mô ủng hộ không -> check FA và câu chuyện; hoặc lọc theo ngành dẫn đầu, xem chất lượng nền giá trước khi đọc báo cáo. (B17 01:41, 02:00)
9. Phân vai: phân tích doanh nghiệp để biết đang cân nhắc tài sản nào; phân tích chuỗi thời gian để theo dõi trạng thái; hai nhóm phục vụ quyết định khác nhau. (B7 03:47)

## 17. Quy trình áp dụng

Bộ bước dưới đây gom từ những gì thầy dạy và các bài luyện đi kèm; nó là cách đọc, không phải hệ thống ra lệnh.

1. **Ghi nhận bối cảnh dữ liệu:** mã, sàn, khung nến, phạm vi thời gian, đơn vị giá và khối lượng. Kéo biểu đồ đủ dài để thấy đỉnh cũ và nền gốc. (B10 02:47; B9 02:26)
2. **Xác định xu thế và khung thời gian:** đối chiếu ngày với tuần, tháng; nhịp ngắn đặt trong nhịp lớn. (B2 02:14; B10 01:17)
3. **Mô tả bằng ngôn ngữ tâm lý:** "lưỡng lự", "hấp thụ", "thử cung", thay vì chỉ gọi "sideway". (B10 00:33)
4. **Đặt giá và khối lượng cạnh nhau:** nền dài, khối lượng thất thường nhưng giá giữ biên là gom; khối lượng co khi giá tăng là hàng cạn; khối lượng lớn lặp lại mà giá tiến ít ở vùng cao là cảnh báo. (B11 02:01, 01:25-01:26; B11 01:38)
5. **Gán giai đoạn đè, gom, đẩy, xả** như một giả thuyết, kèm ba cột: điều thấy, giả thuyết, dấu hiệu phân biệt về sau. (B11 02:04; B10 02:08)
6. **Chỉ khi đó mới chọn đầu mút để đo** bằng Fibonacci (giá và thời gian) hoặc kéo đường chu kỳ trên đoạn đã hoàn tất. (B10 02:08, 01:07)
7. **Dựng kịch bản và kịch bản khác:** ghi điều kiện xác nhận, dấu hiệu phản bác và ngày xem lại. (B9 03:06; B11 02:42)
8. **Tự hỏi mình đang bị dắt về hướng nào** khi tín hiệu quá đẹp, và vị trí đó nguy hiểm ra sao; kiểm tra động cơ bên kia. (B9 01:49; B15 00:03)
9. **Ghép với nền tảng doanh nghiệp, ngành và vĩ mô** trước khi quyết định. (B4 02:00; B17 01:41)
10. **Đối chiếu diễn biến thật với điều kiện đã ghi;** nếu khác giả thuyết thì cập nhật ngay. (B9 02:53, 03:06)

## 18. Sai lầm thường gặp

1. Học thuộc tên mẫu hình, tin hình "đúng sách" mà không hỏi điều kiện và hành động nào tạo nên hình; cố ép đồ thị cho giống một mẫu. (B15 00:01-00:02; B10 00:47)
2. Mua đuổi chỉ báo, hoặc coi tên chỉ báo, một ngưỡng đơn lẻ (RSI 70, MACD dương, MA 50 và 200) là quyết định cuối. Đặt cùng một chỉ báo lên mọi đoạn giá như nhau. (B4 02:47; B10 02:29)
3. Bật quá nhiều chỉ báo và vẽ kín đồ thị. (B10 01:04, 02:20)
4. Mua theo điểm bùng nổ (giá và khối lượng đột biến kèm MACD cắt lên) khi lái đã kích lên, "có hàng đâu mà mua". (B9 02:20)
5. Kéo Fibonacci qua hai điểm đang nhìn thấy mà không biết mã đang ở đâu trong quy trình đè gom đẩy xả; tin ngưỡng 38,2% là hỗ trợ chắc. (B10 02:05-02:09)
6. Đếm sóng khi giá chưa đi hết, theo hình giá đã có ("thầy bói mù"), đổi cách đếm mỗi lần có đỉnh đáy mới; bám sóng nhỏ, nhảy vào nhảy ra. (B2 02:07; B10 00:52; B11 01:20)
7. Dùng mô hình chuỗi thời gian và ngưỡng quá mua đo khoảng cách so với mức gần đây: bán rất sớm, đúng lúc giá sắp chạy. (B10 01:58-02:00)
8. Chọn mốc bằng thông tin xuất hiện sau thời điểm lập giả thuyết rồi trình bày như dự báo (lợi thế nhìn lại); nhìn toàn bộ đồ thị trước khi đoán. (B10 02:06; B17 01:30)
9. Không mua mã đang bị đè gom, tích lũy mà lao vào mã đang tăng và đu theo. (B11 01:32)
10. Tin vùng hỗ trợ vì quá khứ "chưa thủng"; chơi mã "giữ không cho xuống nhưng không bao giờ tăng". (B11 01:55-01:56)
11. Dùng một phép đọc cho mọi giai đoạn: cộng volume theo cách của nền gom khi giá đã vào pha chạy; coi tổng volume một phiên là số hàng một bên đã thu; coi mọi cột volume lớn khi hồi là gom hoặc là phân phối đã xong. (B13 03:21; B15 02:03; B13 03:42)
12. Bê nguyên cách đọc chart nước ngoài vào thị trường có cơ chế giá trần và thanh khoản khác. (B4 02:45)
13. Đọc một cây nến riêng lẻ hoặc dùng mô hình nến (Hammer, Hanging Man) để ra quyết định. (B10 02:35)
14. Hiểu beta là "rủi ro", hay suy beta chỉ từ độ dốc đường giá của một mã. (B10 01:44, 01:48)
15. Chỉ dùng TA, thiếu cơ sở giá trị doanh nghiệp: bán sớm rồi không dám mua lại. (B4 01:59)
16. Áp đặt cái tôi lên đồ thị, tin vạch mình kẻ là đúng rồi "phán" tương lai. (B10 02:10)
17. Cho rằng đường đều và nến lên đều là rủi ro thấp; nhầm một nhịp hồi giúp bớt kẹt với việc cấu trúc đã đổi. (B15 02:21-02:23)
18. Nhầm lượng nhỏ giao dịch được với độ sâu cung cầu: lượng lớn có thể thiếu người đối ứng khi cần thoát. (B15 02:22)

## 19. Bối cảnh lúc ghi hình

> Các nhận định dưới đây là góc nhìn tại thời điểm giảng, cuối 2021 - đầu 2022, thị trường Việt Nam.

- Ở Việt Nam, theo thầy, chỉ cần chất lệnh mua lớn ở giá trần là khoá phiên; ở nước ngoài khó làm vậy vì có bán khống đối ứng. (B4 02:45)
- Học viên chủ yếu dùng phần mềm miễn phí (TradingView, FireAnt...). Thầy chọn AmiBroker cho phần thực hành vì tuỳ biến, và kể các báo cáo scan thầy làm sẽ tích hợp vào app tự động quét. Thầy nói sau này ra ứng dụng riêng sẽ chia sẻ công cụ xoay vòng tương đối tự tính. (B4 04:09; B12 03:00; B2 01:50)
- Bitcoin vừa tạo kiểu bơm xả mới mà sách kỹ thuật chưa có; vài năm sau sách mới cập nhật. (B9 02:11)
- Một học viên cho rằng năm đó tài chính phát triển vì logistics và các ngành khác chưa bắt kịp, tiền "chạy ngoài đường" phải chảy vào thị trường tài chính (bối cảnh 2021-2022). (B11 00:30)
- Một học viên nói chu kỳ bão Mặt Trời trùng năm 2020 với nhiều hiện tượng lạ; thầy giải thích theo cách riêng (theo thầy). (B11 00:40)
- Mã và nhận định trong lớp: HQC (ba chu kỳ), PDR (đi ngang sau nhịp tăng), C4G (hai cách đọc, kịch bản quý II-III), DPM, CTG, CNG (nhóm đang điều chỉnh và nằm trong quá trình gom theo bộ lọc thầy), HHV (vùng ba mươi mấy, 35-36, 42 được nói trong lớp), FLC (bài Replay), GIC, CPH, VNM, DIG, GAB, LHG, CMX, MVC, QNC, BCG: đều là giả thuyết đọc hình giá tại thời điểm đó, không phải khuyến nghị. (B9 02:47, 03:00; B12 02:11, 02:53; B15 02:14, 02:30-02:32; B13 03:32-03:52)
- Báo cáo scan mẫu và trang VNINDEX có tín hiệu và giá là dữ liệu tại thời điểm lập mẫu, không phải thời điểm ghi hình; bảng mã trong báo cáo (ABT, ACL, AGF, VNINDEX) là kết quả hiển thị của mẫu. (B7 03:43; B12 03:01)
- Biểu đồ VN-Index dự phóng với Phase A, B, C là nét vẽ thêm, đường ở vùng chưa có nến là dự phóng, không phải diễn biến đã xảy ra. (B14 01:40)
- Các lời thầy về độ chính xác bản thân ("gần 99,99%"), việc đã kiểm định mẫu nến "thất bại hết", phương pháp momentum "tệ nhất" và hai lớp tín hiệu đều là tự thuật, không kèm số liệu kiểm chứng. (B14 01:11; B10 01:37, 02:12, 02:02)

## 20. Câu hỏi tự kiểm tra

1. Theo thầy, TA phản ánh cái gì, và vì sao các đáp án như "điểm mua bán", "cung cầu" chưa bao quát? (chương 2)
2. Vì sao thầy nói "chả có dự báo nào được cả", và điều gì thì thầy cho là đọc được? (2.2)
3. Cho nến Open 40, High 43, Low 39, Close 42, hãy tính biên độ, thân, bóng trên, bóng dưới và lợi suất đóng so với mở. (chương 3)
4. Thầy phân biệt cách hiển thị nến với việc đọc mô hình nến như thế nào? (3.3)
5. Nếu sau khi đẩy hai phiên, phiên thứ ba khối lượng vẫn tăng, thầy giải thích ra sao; nếu khối lượng co lại thì sao? (4.3)
6. Vùng đi ngang thuần khác vùng gom ở điểm nào về khối lượng và biên giá? (5.5)
7. Tăng 50% rồi giảm 50% giá về đâu, và cần tăng bao nhiêu để hồi từ 70 lên 100? (5.7)
8. Vì sao thầy cho rằng MA(50) và MA(200) tự thân không có ý nghĩa; ý nghĩa nằm ở đâu? (6.2)
9. Vì sao thầy gọi điểm mua theo mẫu hình là "điểm chết", và thầy đọc lại cờ, tam giác, vai đầu vai thế nào? (7.2, 7.3)
10. Kể ba dấu hiệu hoặc cách thầy dùng để chia chu kỳ trên đồ thị và cách đánh số chu kỳ (0, âm 1, 1, 2, 3). (8.4)
11. Dãy Fibonacci được sinh ra thế nào, tỷ số hai số liền kề tiến về giá trị nào, và 1/phi bằng khoảng bao nhiêu? (9.2, 9.3)
12. Với nhịp tăng từ 20 lên 30, các mức hồi 23,6%, 38,2%, 50%, 61,8% nằm ở giá nào; vì sao đổi đầu mút thì mọi mức đổi? (9.5)
13. Vì sao thầy nói kéo Fibonacci qua hai điểm nhìn thấy là lỗi "gần như 100% người học mắc", và cách làm đúng là gì? (9.6)
14. Sóng lồng sóng nghĩa là gì; vì sao bám sóng nhỏ là sai lầm lớn nhất? (10.2, 10.3)
15. Beta tính thế nào từ giá, đọc beta lớn hơn 1, gần 0 và âm ra sao; với beta 1,5, hệ số chặn 0,5% khi thị trường tăng 2% thì cổ phiếu dự đoán tăng bao nhiêu? (12.2)

## 21. Liên quan

- [Dòng tiền, bảng điện và hành vi tay to](07-dong-tien-bang-dien-va-hanh-vi-tay-to.md): đè, gom, đẩy, xả nhìn từ hành vi tay to và sổ lệnh.
- [Binh pháp và 36 kế trong chứng khoán](08-binh-phap-36-ke.md): các kế như Đả thảo kinh xà gắn với ví dụ FireAnt.
- [Tâm lý đầu tư](09-tam-ly-dau-tu.md): gốc tâm lý của việc áp đặt ý chí lên đồ thị và bị "dắt mũi".
- [Quản trị vốn, rủi ro và danh mục](10-quan-tri-von-rui-ro-danh-muc.md): hiểu chu kỳ rủi ro khi đánh nhiều chu kỳ.
- [Quy trình đầu tư và chọn cổ phiếu](11-quy-trinh-dau-tu-va-chon-co-phieu.md): vị trí của TA trong quy trình.
- [Chu kỳ kinh tế và chỉ báo](01a-chu-ky-kinh-te-va-chi-bao.md) và [Ngành và luân chuyển ngành](03-nganh-va-luan-chuyen-nganh.md): lớp vĩ mô và ngành đi trước kỹ thuật.
- [Sách, tài liệu, công cụ](21-sach-tai-lieu-cong-cu.md): phần mềm và công cụ được nhắc.
- [Tình huống các mã khác](12c-tinh-huong-cac-ma-khac.md): các mã được đọc biểu đồ trong lớp.
- Khái niệm nên tra trong phụ lục: Bollinger Bands, Ichimoku, RSI, MACD, CCI, PSAR, ADX, Chaikin money flow, ARIMA, GARCH, VAR, Market Profile, Volume Profile, gần với phần bổ sung trong thư mục phụ lục.

