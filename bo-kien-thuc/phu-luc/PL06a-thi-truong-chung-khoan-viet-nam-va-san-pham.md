# Phụ lục PL06a - Cơ chế thị trường chứng khoán Việt Nam và sản phẩm tài chính (phần 1)

> Phụ lục của Bộ kiến thức NKT. Giải thích những khái niệm thầy nhắc tới trong bài giảng mà chưa giảng đầy đủ. Nội dung được tra cứu từ các nguồn bên ngoài (thời điểm tra cứu: tháng 11/2026), không phải lời thầy.

Lưu ý chung khi đọc: khoá học được ghi hình từ cuối 2021 đến đầu 2022. Từ đó đến nay (tháng 11/2026) thị trường Việt Nam đổi khá nhiều về chu kỳ thanh toán, hệ thống giao dịch, lô lẻ, bán khống, giao dịch trong ngày và xếp hạng thị trường. Ở các mục quy định, phụ lục tách rõ "tại thời điểm khoá học" và "hiện hành". Những chỗ ghi "kiến thức chung, chưa đối chiếu văn bản gốc" là chỗ tôi không mở được văn bản gốc trong lần tra cứu này, nên người đọc cần kiểm lại trước khi dùng. Phụ lục chỉ giải thích khái niệm, không phải lời khuyên đầu tư.

## Danh sách mục
Cụm 1. Chỉ số, vốn hoá và free float
1. Cách tính VN-Index, VN30, VNMidcap, VNSmallcap; bluechip, bigcap, midcap, smallcap; quỹ chỉ số và ETF
2. Cổ phiếu trụ, trọng số trong chỉ số, độ rộng thị trường và hiện tượng "xanh vỏ đỏ lòng"
3. Free float, cổ phiếu trôi nổi thấp, "một mình một chợ" và tỷ lệ sở hữu nhà nước 51%

Cụm 2. Cơ chế giao dịch và hạ tầng thị trường
4. Giá trần, giá sàn, biên độ dao động, thu hẹp biên độ 2008 và cơ chế ngắt mạch (circuit breaker)
5. Chu kỳ thanh toán T+3, T+2, T+2,5, T+0 và hệ thống giao dịch KRX
6. Diện cổ phiếu hạn chế giao dịch
7. Độ sâu thị trường và sổ lệnh (market depth, order book)
8. Chia lệnh và lệnh thuật toán (iceberg, TWAP, VWAP), bot chia lệnh
9. Giao dịch thoả thuận, thị phần môi giới, bán cho quỹ ngoại, tài khoản kho và repo cổ phiếu

Cụm 3. Bán khống, phái sinh và chứng quyền
10. Bán khống (short selling), hợp đồng tương lai VN30 và đội short
11. Chứng quyền có bảo đảm (covered warrant)

Cụm 4. Vay, thâu tóm và giao dịch của người nội bộ
12. Cầm cố cổ phiếu, trần giá cho vay, vay kho (3:7, 2:8) và tài sản bảo đảm bằng cổ phiếu
13. Chào mua công khai, premium khi mua nguyên lô (control premium), ngưỡng sở hữu 25% và 50%
14. Giao dịch nội gián và công bố giao dịch của người nội bộ, cổ đông lớn

Cụm 5. Dòng vốn, dòng tiền thông minh và tài sản số
15. ETF, dòng vốn quỹ ngoại vào Việt Nam và dòng vốn toàn cầu
16. Dòng vốn ngoại đầu 2022: quỹ Đài Loan 5.000 tỷ, ETF Fubon, các quỹ mua ròng tháng 1/2022
17. Dòng tiền thông minh (smart money, "big boy")
18. Bitcoin và tài chính phi tập trung (DeFi) (đã chuyển sang folder ngoai-dau-tu)

Cụm 6. Forex (giao dịch ngoại hối bán lẻ)
19. Forex cơ chế: lot, pip, đòn bẩy 1:100 và 1:200, ký quỹ, stop out, mức nạp tối thiểu (đã chuyển sang folder ngoai-dau-tu)
20. Forex chi phí: phí qua đêm (swap, rollover), hoa hồng (commission), spread (đã chuyển sang folder ngoai-dau-tu)
21. Forex sàn giao dịch: dealing desk, market maker so với ECN, STP; giấy phép FSA, FCA; tình trạng pháp lý ở Việt Nam (đã chuyển sang folder ngoai-dau-tu)

Cụm 7. Lịch sử thị trường, hành vi và các chuyện lẻ
22. Đấu giá cổ phần doanh nghiệp nhà nước 2005-2007, đặt cọc 10% và thị trường Việt Nam 2004-2008
23. Hiệu ứng nghỉ Tết trên thị trường chứng khoán Việt Nam
24. Đường cong tâm lý và FOMO trong giao dịch
25. Gian lận thẻ để bán lại bản quyền phần mềm giá rẻ

## Cụm 1. Chỉ số, vốn hoá và free float

### Cách tính VN-Index, VN30, VNMidcap, VNSmallcap; bluechip, bigcap, midcap, smallcap; quỹ chỉ số và ETF

**Thầy nhắc ở:** B2 01:27, B2 01:31, B4 03:14, B9 00:41, B9 02:01, B12 00:33 - thầy nói quỹ dùng khoảng 10% vốn để "kích" chỉ số, dòng tiền luân chuyển giữa các nhóm vốn hoá, FLC đáng lẽ chờ vào rổ VN30 rồi bán cho quỹ; phần chỉ số chuyển thành tài liệu tự đọc.

**Là gì:** VN-Index là chỉ số giá của toàn bộ cổ phiếu niêm yết trên sàn HOSE, được tính theo vốn hoá thị trường (giá nhân khối lượng). VN30, VNMidcap, VNSmallcap là các chỉ số con cũng của HOSE: VN30 gồm 30 cổ phiếu lớn nhất xét theo vốn hoá và thanh khoản trong rổ VNAllshare, VNMidcap gồm 70 cổ phiếu vốn hoá trung bình, VNSmallcap gồm các cổ phiếu vốn hoá nhỏ.

**Giải thích:**
- Công thức: VN-Index = 100 x (tổng giá hiện hành x khối lượng niêm yết) / (tổng giá kỳ gốc x khối lượng kỳ gốc). Khi có niêm yết mới, tăng vốn, huỷ niêm yết hoặc giảm vốn, mẫu số được điều chỉnh bằng một hệ số chia để chỉ số không bị nhảy giả. Phiên giao dịch đầu tiên của HOSE là 28/7/2000, chỉ số lấy mốc gốc 100 điểm.
- Hệ quả của việc tính theo vốn hoá: mã nào vốn hoá lớn thì "nặng" trong chỉ số. Một mã vốn hoá lớn tăng 3% có thể kéo chỉ số nhiều hơn hàng trăm mã nhỏ cùng tăng 3%. Vì vậy người ta dùng vài mã lớn để "kích" chỉ số trong khi phần đông cổ phiếu đứng yên.
- Các chỉ số nhóm như VN30 thường được xây theo vốn hoá điều chỉnh free float (phần cổ phiếu thực sự tự do giao dịch) và có trần tỷ trọng mỗi mã, danh mục được rà soát định kỳ (hiểu biết chung, chưa đối chiếu phương pháp luận chính thức của HOSE; nên tra tài liệu "phương pháp tính chỉ số" trên website HOSE).
- Cách gọi bluechip, bigcap, midcap, smallcap là cách gọi của thị trường, không phải khái niệm pháp lý. Thực hành thường dùng: VN30 là nhóm bluechip/bigcap, VNMidcap là nhóm trung bình, VNSmallcap là nhóm nhỏ. Ngưỡng vốn hoá cụ thể thay đổi theo thời kỳ.
- ETF (quỹ hoán đổi danh mục) là quỹ niêm yết mô phỏng một chỉ số. Cơ chế: các tổ chức tham gia lập quỹ nộp rổ cổ phiếu để nhận chứng chỉ quỹ (tạo lập) hoặc làm ngược lại (hoàn trả), nhờ vậy giá ETF bám sát giá trị tài sản ròng. Khi dòng tiền vào ETF tăng thì quỹ phải mua các cổ phiếu trong rổ theo tỷ trọng, nên việc một mã được thêm vào rổ chỉ số có thể tạo ra cầu mua mang tính cơ học. Đây là ý của thầy khi nói về chuyện FLC chờ vào VN30 rồi bán cho quỹ.
- Ở Việt Nam có các ETF nội mô phỏng VN30 và các chỉ số khác của HOSE (hiểu biết chung, nên tra danh sách ETF trên HOSE), và các ETF nước ngoài mô phỏng chỉ số về Việt Nam (xem mục dòng vốn ngoại bên dưới).

**Liên hệ với bài học:** Hiểu cách tính này giúp đọc đúng câu "kích index": index tăng không có nghĩa phần lớn cổ phiếu tăng. Điểm khác với hiểu biết phổ thông: nhiều người nghĩ VN-Index là "trung bình các cổ phiếu", thực ra là trung bình có trọng số vốn hoá nên bị chi phối bởi nhóm lớn.

**Đọc thêm:** [Wikipedia tiếng Việt - VN-Index](https://vi.wikipedia.org/wiki/VN-Index); [Wikipedia tiếng Anh - VN-Index](https://en.wikipedia.org/wiki/VN-Index); [Wikipedia tiếng Anh - Ho Chi Minh City Stock Exchange](https://en.wikipedia.org/wiki/Ho_Chi_Minh_City_Stock_Exchange); [Wikipedia tiếng Anh - Exchange-traded fund](https://en.wikipedia.org/wiki/Exchange-traded_fund)

### Cổ phiếu trụ, trọng số trong chỉ số, độ rộng thị trường và hiện tượng "xanh vỏ đỏ lòng"

**Thầy nhắc ở:** B13 03:02, B14 01:00 - thầy coi hiện tượng chỉ số xanh nhưng đa số cổ phiếu đỏ là dấu hiệu "Điệu hổ ly sơn".

**Là gì:** Cổ phiếu trụ là cổ phiếu có tỷ trọng vốn hoá lớn trong chỉ số, nên giá của nó quyết định phần lớn biến động chỉ số. Độ rộng thị trường (market breadth) là mức độ lan toả của xu hướng: bao nhiêu mã tăng, bao nhiêu mã giảm. "Xanh vỏ đỏ lòng" là cách gọi khi chỉ số xanh (tăng) nhưng số mã giảm lại nhiều hơn số mã tăng.

**Giải thích:**
- Ví dụ số minh hoạ (giả định): giả sử một mã chiếm 10% trọng số và tăng 4%, riêng mã đó đã đóng góp khoảng 0,4 điểm phần trăm vào mức tăng của chỉ số. Nếu 300 mã còn lại cùng giảm trung bình 0,3% với tổng trọng số 90%, chúng kéo chỉ số xuống khoảng 0,27 điểm phần trăm. Kết quả chỉ số vẫn xanh, trong khi bảng điện có nhiều mã đỏ.
- Chỉ báo độ rộng thường dùng: tỷ lệ số mã tăng so với số mã giảm (advance/decline), phần trăm số mã đang nằm trên đường trung bình động 50 hoặc 200 phiên, số mã mới lập đỉnh so với số mã mới lập đáy.
- Điệu hổ ly sơn là kế thứ 15 trong Tam thập lục kế, nghĩa là dụ hổ rời núi. Trong cách thầy dùng, việc đẩy vài mã trụ để giữ chỉ số xanh khiến nhà đầu tư yên tâm trong khi các mã khác bị xả là một dạng "điệu hổ ly sơn" (xem thêm Phụ lục PL08 về Tam thập lục kế).
- Lưu ý: độ rộng yếu chưa chứng minh có ai cố ý thao túng. Nó có thể chỉ phản ánh dòng tiền tập trung vào nhóm lớn.

**Liên hệ với bài học:** Mục này giúp đọc bảng điện đúng cách: không chỉ nhìn điểm chỉ số mà nhìn thêm số mã tăng giảm và nhóm mã nào đóng góp điểm. Khác với cách nhìn phổ thông là "chỉ số xanh nghĩa là thị trường tốt".

**Đọc thêm:** [Wikipedia tiếng Anh - Ho Chi Minh City Stock Exchange](https://en.wikipedia.org/wiki/Ho_Chi_Minh_City_Stock_Exchange); [Wikipedia tiếng Anh - Investor sentiment](https://en.wikipedia.org/wiki/Investor_sentiment)

### Free float, cổ phiếu trôi nổi thấp, "một mình một chợ" và tỷ lệ sở hữu nhà nước 51%

**Thầy nhắc ở:** B13 03:46, B14 00:59, B5 02:38 - thầy dùng cho cổ phiếu THD, học viên nói lái gom hết hàng trôi nổi; thầy nhắc khi tra ngược cấu trúc cổ đông.

**Là gì:** Free float (cổ phiếu tự do chuyển nhượng, "trôi nổi") là phần cổ phiếu do nhà đầu tư thông thường nắm giữ, không tính phần của sáng lập viên, ban lãnh đạo, cổ đông chi phối hoặc nhà nước. Công thức: free float = cổ phiếu đang lưu hành trừ cổ phiếu bị hạn chế chuyển nhượng hoặc nắm giữ chiến lược.

**Giải thích:**
- Ví dụ: công ty có 10 triệu cổ phiếu lưu hành, 3 triệu cổ phiếu bị khoá hoặc do cổ đông chi phối giữ, thì free float là 7 triệu cổ phiếu (70%).
- Free float thấp thì lượng hàng thực sự mua bán được ít. Khi dòng tiền đổ vào, giá dễ bị đẩy mạnh và dao động mạnh, còn khi cần bán thì khó thoát. Cách gọi "một mình một chợ" ám chỉ cổ phiếu có ít hàng tự do và ít nguồn cung đối ứng, nên một nhóm nhỏ có thể chi phối giá.
- Cổ đông nhà nước nắm từ 51% trở lên tức là giữ quyền chi phối. Phần này thường không giao dịch, nên free float thực tế chỉ còn nhiều nhất 49% trừ thêm các cổ đông lớn khác và phần nhà đầu tư nước ngoài bị giới hạn theo room ngoại.
- Cách tra: báo cáo thường niên, báo cáo quản trị và danh sách cổ đông lớn do doanh nghiệp công bố, hoặc các trang dữ liệu chứng khoán (cách tra này là hiểu biết chung).
- Free float còn được dùng để tính trọng số trong nhiều chỉ số, nên mã có free float thấp thường có tỷ trọng hiệu chỉnh nhỏ hơn vốn hoá thô.

**Liên hệ với bài học:** Hiểu free float giúp hiểu vì sao thầy và học viên coi các mã "ít hàng" là dễ bị thao túng giá, và vì sao khi tra ngược cấu trúc cổ đông cần cộng trừ để ra phần hàng thật sự lưu thông.

**Đọc thêm:** [Wikipedia tiếng Anh - Free float](https://en.wikipedia.org/wiki/Free_float); [Wikipedia tiếng Anh - Short squeeze](https://en.wikipedia.org/wiki/Short_squeeze) (cổ phiếu float nhỏ dễ bị "bóp" mạnh khi có đầu cơ)

## Cụm 2. Cơ chế giao dịch và hạ tầng thị trường

### Giá trần, giá sàn, biên độ dao động, thu hẹp biên độ 2008 và cơ chế ngắt mạch (circuit breaker)

**Thầy nhắc ở:** B2 01:55, B4 02:45, B9 02:39, B11 02:47 - thầy chê chính sách thu hẹp biên độ năm 2008 là "thô bạo", nói chất lệnh mua giá trần làm khoá phiên, và so sánh Việt Nam với Mỹ.

**Là gì:** Biên độ dao động giá là mức tăng giảm tối đa so với giá tham chiếu trong một phiên. Giá trần là mức giá cao nhất được đặt, giá sàn là mức thấp nhất. Cơ chế ngắt mạch (circuit breaker) là việc tạm dừng giao dịch khi thị trường giảm quá mạnh trong thời gian ngắn.

**Giải thích:**
- Quy định khi khoá học ghi hình và hiện nay trùng nhau về mức: cổ phiếu và chứng chỉ quỹ trên HOSE có biên độ +/-7% so với giá tham chiếu, ngày đầu niêm yết trên HOSE là +/-20% (theo mô tả HOSE trên Wikipedia, tra tháng 11/2026). Hiểu biết chung (chưa đối chiếu văn bản gốc): HNX là +/-10%, UPCoM là +/-15%.
- Khi giá khớp ở trần với dư mua lớn, lệnh mua chồng lên nhau không khớp được vì không còn lệnh bán. Khi đó theo nguyên tắc ưu tiên về giá rồi về thời gian (lệnh đặt trước khớp trước), lệnh vào sau xếp hàng chờ. Thầy dùng điều này để nói về "chất lệnh mua trần khoá phiên" tạo cảm giác cầu rất mạnh.
- Thu hẹp biên độ 2008: theo hiểu biết chung, trong năm 2008 HOSE thu hẹp biên độ từ mức khoảng +/-5% xuống còn +/-1% trong thời kỳ thị trường lao dốc, sau đó nới dần. Tôi chưa tìm được văn bản hoặc nguồn tin cậy để xác nhận từng mốc ngày và từng mức, nên chỉ nên hiểu đây là ý chung: cơ quan quản lý dùng công cụ biên độ để làm chậm đà giảm, và thầy cho rằng cách làm đó thô bạo vì nó nhốt thanh khoản.
- Ngắt mạch ở Mỹ: ngưỡng được tính theo mức giảm của chỉ số S&P 500 so với giá đóng cửa hôm trước: cấp 1 giảm 7%, cấp 2 giảm 13%, cấp 3 giảm 20%. Cấp 1 và 2 dừng giao dịch ít nhất 15 phút (không áp dụng nếu xảy ra sau 15h25 giờ New York), cấp 3 dừng giao dịch đến hết ngày. Cơ chế bắt đầu từ tháng 1/1988 sau ngày Thứ Hai Đen 1987 và được dùng nhiều lần trong tháng 3/2020. Với từng cổ phiếu, Mỹ dùng cơ chế riêng (Limit Up-Limit Down) theo biên độ trong khung 5 phút.
- Việt Nam hiện dùng biên độ giá từng mã làm công cụ chính, không có ngắt mạch theo phần trăm chỉ số như Mỹ (hiểu biết chung; chưa tìm được văn bản xác nhận quy định ngắt mạch toàn thị trường). Hệ thống KRX vận hành từ 5/5/2025 chưa thay mức biên độ (các nguồn tra được không nêu thay đổi biên độ).

**Liên hệ với bài học:** So sánh Việt Nam với Mỹ trong bài là so hai cách chặn biến động: Việt Nam chặn từng mã theo mức tuyệt đối cố định hằng ngày, Mỹ chặn cả thị trường theo ngưỡng chỉ số và có thời gian "nghỉ" để tin tức lan toả.

**Đọc thêm:** [Wikipedia tiếng Anh - Trading curb](https://en.wikipedia.org/wiki/Trading_curb); [Wikipedia tiếng Anh - Ho Chi Minh City Stock Exchange](https://en.wikipedia.org/wiki/Ho_Chi_Minh_City_Stock_Exchange); [Dân Trí - KRX chính thức vận hành từ ngày 5/5](https://dantri.com.vn/kinh-doanh/he-thong-krx-chinh-thuc-van-hanh-tu-ngay-55-20250424144532178.htm)

### Chu kỳ thanh toán T+3, T+2, T+2,5, T+0 và hệ thống giao dịch KRX

**Thầy nhắc ở:** B13 01:26, B14 00:26, B15 00:29, B16 00:32, B17 00:25, B2 01:38, B4 02:18, B9 02:39, B11 02:47 - thầy và học viên nhắc "hàng về", bị chốt lời, không kịp bán vào thứ Ba; thầy bàn T+0 và so sánh Mỹ với Việt Nam.

**Là gì:** Chu kỳ thanh toán T+n là số ngày làm việc từ ngày khớp lệnh (T) đến ngày tiền và chứng khoán được chuyển giao thật. "Hàng về" là lúc cổ phiếu mua được hiện trong tài khoản và có thể bán. T+0 là mua và bán lại ngay trong cùng ngày. KRX là hệ thống công nghệ giao dịch mới của thị trường, do Sở Giao dịch Chứng khoán Hàn Quốc cung cấp.

**Giải thích:**
- Tại thời điểm khoá học (cuối 2021 đầu 2022): chu kỳ T+3. Theo Thời báo Tài chính Việt Nam, trước 29/8/2022 chứng khoán mua ở ngày T+0 phải chờ đến T+3 mới bán được. Việc bù trừ do Tổng công ty Lưu ký và Bù trừ chứng khoán Việt Nam (VSD, nay là VSDC) thực hiện, và khi đó hoàn tất thanh toán vào khoảng 15h30 đến 16h00. Giao dịch trong ngày (T+0) với cổ phiếu cơ sở chưa có, nên chuyện "mua hôm nay bán ngay hôm nay" chỉ làm được với phái sinh.
- Thay đổi 29/8/2022: VSD ban hành Quyết định 109/QĐ-VSD (ngày 19/8/2022) về quy chế bù trừ và thanh toán, và Quyết định 110/QĐ-VSD về quy chế thành viên lưu ký, hiệu lực từ 29/8/2022. Chu kỳ rút xuống T+2, thanh toán giữa ngân hàng thanh toán và VSD hoàn tất khoảng 11h00 đến 11h30, thành viên lưu ký phân bổ tiền và chứng khoán cho khách chậm nhất 13h. Nhà đầu tư vì vậy có thể bán chứng khoán mua ở T+0 ngay trong phiên chiều T+2. Báo chí hay gọi cách này là "T+2,5" vì hàng về giữa ngày T+2 chứ không phải đầu ngày.
- Mốc quan trọng khác: lô lẻ trên HOSE được đề xuất áp dụng từ 12/9/2022 (bài báo ngày 29/8/2022); KRX chính thức vận hành tại HOSE và HNX từ 5/5/2025 (sau khi dự kiến ban đầu từ năm 2021 bị trì hoãn).
- Hiện hành (tháng 11/2026): cổ phiếu, chứng chỉ quỹ, chứng quyền thanh toán T+2; trái phiếu T+1 (theo bài báo Tuổi Trẻ ngày 27/2/2026 về sự cố thanh toán, và tổng hợp tin tức). T+0 cho cổ phiếu cơ sở và bán chứng khoán "chờ về" vẫn chưa triển khai. Bộ Tài chính đặt trong Đề án nâng hạng (Quyết định 2014/QĐ-TTg) việc nghiên cứu cơ chế vay, cho vay chứng khoán, bán khống có kiểm soát qua giao dịch chờ về và giao dịch trong ngày trong giai đoạn 2026-2028. Bài báo ngày 28/10/2026 nêu Bộ trưởng Tài chính nói thị trường đang hướng tới CCP và T+0 nhưng chưa có lộ trình cụ thể.
- Hạ tầng đi kèm: cơ chế đối tác bù trừ trung tâm (CCP) được lên kế hoạch vận hành chậm nhất quý 1/2027 (lộ trình UBCKNN công bố tháng 7/2025; Tổng giám đốc VSDC nói đầu năm 2027 ngày 6/1/2026). Thông tư 145/2026/TT-BTC (ban hành 30/9/2026, hiệu lực 16/11/2026) quy định đăng ký, lưu ký, bù trừ và thanh toán chứng khoán; một nguồn ghi nó thay Thông tư 119/2020/TT-BTC, cần đối chiếu văn bản gốc.
- Nâng hạng: FTSE Russell công bố ngày 8/10/2025 nâng Việt Nam từ thị trường cận biên lên mới nổi thứ cấp; các nguồn tin ghi hiệu lực vào đầu tháng 9/2026 (một số nguồn ghi 21/9/2026). Trước đó Việt Nam chưa đạt tiêu chí về chu kỳ thanh toán và chi phí giao dịch lỗi thanh toán; các cải cách như Thông tư 68/2024/TT-BTC (bỏ yêu cầu ký quỹ trước giao dịch với tổ chức đầu tư nước ngoài, hiệu lực 2/11/2024) và KRX là phần đáp ứng. Theo bài ngày 10/7/2026 trên Vietstock, ở kỳ rà soát tháng 6/2026 MSCI vẫn chưa đưa Việt Nam vào danh sách theo dõi nâng hạng.

**Liên hệ với bài học:** Các câu "hàng về", "không kịp thứ Ba" trong bài phải hiểu theo T+3 của thời điểm đó: mua ngày thứ Hai thì T+3 là thứ Năm, nghĩa là tiền và hàng chưa thể xoay vòng trong 2 ngày giữa. Ngày nay T+2 giảm độ trễ khoảng một ngày nhưng vẫn khác Mỹ (Mỹ đã chuyển sang T+1 từ 28/5/2024, hiểu biết chung) và khác kiểu T+0 mà thầy hay đem ra so sánh.

**Đọc thêm:** [Thị trường Tài chính Tiền tệ - Từ 29/8 rút ngắn thanh toán xuống T+2](https://thitruongtaichinhtiente.vn/tu-ngay-29-8-chinh-thuc-rut-ngan-thoi-gian-thanh-toan-giao-dich-chung-khoan-xuong-con-t-2-41949.html); [Thời báo Tài chính - HOSE áp dụng giao dịch lô lẻ từ ngày 12/9](https://thoibaotaichinhvietnam.vn/hose-se-ap-dung-giao-dich-lo-le-tu-ngay-129-111606.html); [Tuổi Trẻ - Thanh toán T+2 trục trặc chiều 27/2/2026](https://tuoitre.vn/thanh-toan-t-2-truc-trac-nhieu-giao-dich-chua-ve-tai-khoan-chieu-27-2-20260227145126394.htm); [VnEconomy - Lộ trình CCP của UBCKNN](https://vneconomy.vn/uy-ban-chung-khoan-nha-nuoc-cong-bo-lo-trinh-trien-khai-ccp-cho-thi-truong-chung-khoan-co-so.htm); [VnEconomy - Tổng giám đốc VSDC nói về năm 2026](https://vneconomy.vn/tong-giam-doc-vsdc-nam-2026-tiep-tuc-nang-cap-he-thong-de-cho-phep-ban-chung-khoan-cho-ve.htm); [Diễn đàn Doanh nghiệp - Bán khống và T0 dự kiến 2026](https://diendandoanhnghiep.vn/trien-khai-nghiep-vu-ban-khong-va-thuc-hien-giao-dich-t0-du-kien-vao-2026-10165058.html); [Mekong ASEAN - Hướng tới T+0 (28/10/2026)](https://mekongasean.vn/chung-khoan-viet-nam-huong-toi-giao-dich-t0-nang-hang-theo-tieu-chi-msci-61177.html); [Luật Việt Nam - Thông tư 145/2026/TT-BTC](https://luatvietnam.vn/chung-khoan/thong-tu-145-2026-tt-btc-quy-dinh-dang-ky-luu-ky-bu-tru-va-thanh-toan-chung-khoan-449607-d1.html)

### Diện cổ phiếu hạn chế giao dịch

**Thầy nhắc ở:** B13 03:26 - thầy nhắc ví dụ cổ phiếu chỉ giao dịch vào ngày thứ Sáu.

**Là gì:** Sở giao dịch xếp cổ phiếu vào các diện cảnh báo, kiểm soát, hạn chế giao dịch, tạm ngừng hoặc đình chỉ khi doanh nghiệp vi phạm công bố thông tin, lỗ kéo dài, chậm nộp báo cáo, kiểm toán không chấp nhận toàn phần và các lý do khác. Diện hạn chế giao dịch là diện bị siết về cách khớp lệnh và về margin.

**Giải thích:**
- Tại thời điểm khoá học: thầy nói có cổ phiếu chỉ giao dịch một số ngày trong tuần, ví dụ thứ Sáu. Tôi chưa tìm được văn bản hoặc nguồn tin cậy xác nhận quy định cụ thể và danh sách mã bị áp dụng ở cuối 2021 đầu 2022. Từ khoá gợi ý để tra: "chứng khoán hạn chế giao dịch" Quy chế niêm yết HOSE HNX 2021, "khớp lệnh định kỳ một lần mỗi tuần".
- Sau KRX (5/5/2025): theo bài tổng hợp của VFS, trước KRX cổ phiếu hạn chế giao dịch chủ yếu khớp lệnh liên tục và thoả thuận; sau KRX áp dụng cơ chế khớp lệnh định kỳ nhiều lần (PCA). Dân Trí liệt kê "giao dịch chứng khoán thuộc diện bị hạn chế" là một nội dung quy định mới của KRX.
- Hiện hành: danh sách mã không được margin quý IV/2026 do HOSE công bố ngày 6/10/2026 có 65 mã, trong đó 24 mã diện cảnh báo, 5 mã diện kiểm soát (ABS, DQC, HAS, SBV, TTF) và 3 mã diện hạn chế giao dịch (DGC, DRH, VMD). Danh sách thay đổi theo từng kỳ, nên chỉ có giá trị tại ngày công bố.

**Liên hệ với bài học:** Đây là lưu ý rủi ro thanh khoản: cổ phiếu diện hạn chế khó bán, không dùng margin được, và giá không phản ánh nhu cầu liên tục. Cần tra thông báo của sở giao dịch trước khi mua một mã nghi vấn.

**Đọc thêm:** [Báo Pháp luật - HOSE đưa 65 mã vào diện không được margin quý IV/2026](https://doanhnhan.baophapluat.vn/hose-dua-65-ma-chung-khoan-vao-dien-khong-duoc-giao-dich-margin-quy-iv-2026.html); [VFS - Hệ thống KRX là gì](https://www.vfs.com.vn/he-thong-krx-la-gi); [Dân Trí - KRX vận hành từ 5/5](https://dantri.com.vn/kinh-doanh/he-thong-krx-chinh-thuc-van-hanh-tu-ngay-55-20250424144532178.htm)

### Độ sâu thị trường và sổ lệnh (market depth, order book)

**Thầy nhắc ở:** B4 03:01 - bảng giá chỉ hiện 3 mức giá, công ty chứng khoán thấy hết.

**Là gì:** Sổ lệnh là danh sách tất cả lệnh mua và lệnh bán đang chờ khớp, xếp theo giá. Độ sâu thị trường là khối lượng chờ ở từng mức giá, đo khả năng hấp thụ một lệnh lớn mà giá không bị đẩy nhiều. Định nghĩa trên Wikipedia: độ sâu là kích thước lệnh cần có để làm giá thị trường dịch chuyển một mức nhất định; thị trường sâu cần lệnh rất lớn mới làm giá đổi.

**Giải thích:**
- Bảng giá thường chỉ hiển thị 3 mức giá mua và 3 mức giá bán tốt nhất. KRX tiếp tục hiển thị 3 mức giá chào mua và chào bán tốt nhất (cả trong các đợt khớp lệnh định kỳ). Dữ liệu sổ lệnh sâu hơn (cấp 2) có ở một số công ty chứng khoán hoặc nhà cung cấp dữ liệu, và các lệnh có thể bị ẩn hoặc huỷ nhanh nên không phải lúc nào cũng phản ánh ý định thật.
- Yếu tố ảnh hưởng độ sâu: bước giá nhỏ giúp thị trường sâu hơn, giới hạn biên độ và yêu cầu ký quỹ cao làm giảm số người tham gia, và độ minh bạch kém làm người ta ngại đặt lệnh.
- Ở Việt Nam bước giá của HOSE là 10 đồng (giá dưới 10.000 đồng), 50 đồng (từ 10.000 đến dưới 50.000 đồng), 100 đồng (từ 50.000 đồng trở lên); một lô chẵn là 100 cổ phiếu (hiểu biết chung, chưa đối chiếu văn bản gốc). Vì bước giá lớn so với giá cổ phiếu rẻ, số mức giá trong cùng biên độ ít hơn nên sổ lệnh Việt Nam nhìn "mỏng" hơn so với thị trường bước giá nhỏ.

**Liên hệ với bài học:** Thầy nói công ty chứng khoán thấy nhiều hơn nhà đầu tư thường, tức là có chênh lệch thông tin về sổ lệnh. Hiểu độ sâu giúp thấy rằng vài lệnh lớn có thể gây trượt giá nhiều ở cổ phiếu mỏng.

**Đọc thêm:** [Wikipedia tiếng Anh - Market depth](https://en.wikipedia.org/wiki/Market_depth); [Dân Trí - KRX vận hành từ 5/5](https://dantri.com.vn/kinh-doanh/he-thong-krx-chinh-thuc-van-hanh-tu-ngay-55-20250424144532178.htm)

### Chia lệnh và lệnh thuật toán (iceberg, TWAP, VWAP), bot chia lệnh

**Thầy nhắc ở:** B13 02:56, B17 02:18 - thầy mô tả gom 10.000 cổ trong một giây bằng các lệnh nhỏ.

**Là gì:** Chia lệnh là chia một lệnh lớn thành nhiều lệnh nhỏ đặt rải theo thời gian để giá không bị đẩy và để người khác không đoán được ý định. Các thuật toán thực thi phổ biến gồm TWAP (chia đều theo thời gian), VWAP (chia theo tỷ lệ khối lượng giao dịch của thị trường) và iceberg (chỉ hiện một phần nhỏ của lệnh).

**Giải thích:**
- Iceberg: lệnh giới hạn có "lượng hiển thị" nhỏ hơn tổng lượng. Khi lượng hiển thị khớp hết, lệnh bị đẩy xuống cuối hàng chờ và phần tiếp theo mới hiện ra. Nhược điểm: khớp chậm hơn và ở nhiều sàn tốn phí cao hơn; giao dịch vẫn hiện trong dữ liệu khớp sau khi xảy ra.
- Cách nhận diện trên dữ liệu khớp (suy luận từ cơ chế): thấy liên tục các lệnh khớp cùng kích cỡ ở một mức giá, và lượng chào mới lại hiện ra sau mỗi lần khớp. Cũng có những thuật toán "dò" gửi các lệnh nhỏ để phát hiện lệnh ẩn.
- VWAP còn là thước đo: so giá khớp trung bình của một lệnh với VWAP cùng khung giờ để đánh giá chất lượng thực thi.
- Việc ở Việt Nam có hỗ trợ iceberg gốc hay không, và bot chia lệnh qua API của công ty chứng khoán vận hành thế nào, tôi chưa tìm được nguồn đáng tin; từ khoá gợi ý: "lệnh thuật toán công ty chứng khoán API TWAP VWAP Việt Nam".

**Liên hệ với bài học:** Nó giúp hiểu cách một tổ chức gom hàng mà bảng điện nhìn như có nhiều người nhỏ lẻ mua. Với người đọc dữ liệu khớp, dấu hiệu đáng chú ý là nhịp đặt lệnh đều đặn bất thường.

**Đọc thêm:** [Wikipedia tiếng Anh - Iceberg order](https://en.wikipedia.org/wiki/Iceberg_order); [Wikipedia tiếng Anh - Algorithmic trading](https://en.wikipedia.org/wiki/Algorithmic_trading)

### Giao dịch thoả thuận, thị phần môi giới, bán cho quỹ ngoại, tài khoản kho và repo cổ phiếu

**Thầy nhắc ở:** B9 01:23, B9 01:26, B9 01:28, B12 00:48 - thầy nói ông chủ lớn xả qua kênh thoả thuận; học viên nhắc tài khoản kho.

**Là gì:** Giao dịch thoả thuận (put-through) là giao dịch mà hai bên tự thoả thuận giá và khối lượng rồi nhập vào hệ thống của sở, thường dùng cho lô lớn. Tài khoản kho là cách gọi tài khoản đứng tên người khác dùng để cất cổ phiếu hoặc cầm cố. Repo cổ phiếu là hợp đồng bán cổ phiếu kèm cam kết mua lại sau một thời gian ở mức giá thoả thuận.

**Giải thích:**
- Thoả thuận không tham gia khớp lệnh liên tục nên không trực tiếp đổi giá thị trường theo sổ lệnh, nhưng vẫn được công bố khối lượng và giá. Người nắm lô lớn có thể bán cho quỹ ngoại hoặc tổ chức qua kênh này để tránh làm sụt giá. Đây là hiểu biết chung; quy định về giá trị, khối lượng tối thiểu và khung giờ thoả thuận do quy chế của sở quy định và thay đổi theo KRX (KRX mở rộng khung giờ và chuẩn hoá giao dịch thoả thuận).
- Thị phần môi giới: các công ty chứng khoán xếp hạng theo giá trị giao dịch khách hàng; giao dịch thoả thuận lớn của một khách có thể làm thị phần một công ty biến động mạnh trong quý (hiểu biết chung; cách tra: báo cáo thị phần môi giới hằng quý do HOSE, HNX công bố).
- Repo cổ phiếu và vay bằng cổ phiếu là cách các cổ đông lớn huy động tiền, và khi giá giảm thì có thể bị gọi bổ sung tài sản hoặc bị xử lý. Cổ đông cũng có thể bán thoả thuận để trả nợ vay; đây là một lý do vì sao các đợt "thoả thuận" lớn không phải lúc nào cũng là tin xấu về triển vọng doanh nghiệp.
- Tôi chưa mở được văn bản gốc để dẫn điều khoản chính xác; nên đối chiếu quy chế giao dịch của HOSE hiện hành.

**Liên hệ với bài học:** Mục này giải thích vì sao khối lượng lớn bất thường trên bảng điện có thể không phải do nhà đầu tư nhỏ, và vì sao cần phân biệt giá trị khớp lệnh với giá trị thoả thuận khi đọc dữ liệu.

**Đọc thêm:** [Dân Trí - KRX vận hành từ 5/5 (giao dịch thoả thuận thuộc nhóm thay đổi)](https://dantri.com.vn/kinh-doanh/he-thong-krx-chinh-thuc-van-hanh-tu-ngay-55-20250424144532178.htm); [VFS - Hệ thống KRX là gì](https://www.vfs.com.vn/he-thong-krx-la-gi)

## Cụm 3. Bán khống, phái sinh và chứng quyền

### Bán khống (short selling), hợp đồng tương lai VN30 và đội short

**Thầy nhắc ở:** B1 00:54, B2 01:38, B4 02:59, B9 00:55, B9 02:39, B11 02:11, B13 02:35 - thầy thích bán khống, nói Việt Nam chưa cho, cách short chỉ số là dùng phái sinh VN30; "nếu ở nước ngoài thì short".

**Là gì:** Bán khống là bán một chứng khoán mà mình không sở hữu (đi mượn) với kỳ vọng giá giảm, rồi mua lại sau để trả. Lãi khi giá giảm, lỗ khi giá tăng. "Cover" là mua lại để đóng vị thế. Hợp đồng tương lai chỉ số VN30 là hợp đồng phái sinh bán lẻ chuẩn hoá trên chỉ số VN30, cho phép vào lệnh bán (short) mà không cần mượn cổ phiếu.

**Giải thích:**
- Cơ chế bán khống cổ phiếu cơ sở: (1) vay cổ phiếu từ một bên cho vay thông qua công ty môi giới, (2) bán ngay ở thị trường, (3) khi giá giảm mua lại và trả cổ phiếu. Lợi nhuận bằng chênh lệch giá trừ phí vay và cổ tức mà người bán khống phải trả bù. Ví dụ: cổ phiếu 10 USD, bán khống 100 cổ phiếu thu 1.000 USD; giá về 8 USD thì mua lại hết 800 USD, lãi 200 USD; nếu giá lên 25 USD thì mua lại 2.500 USD, lỗ 1.500 USD.
- Rủi ro: lỗ về lý thuyết không giới hạn (giá có thể tăng vô hạn, trong khi lãi tối đa bị chặn khi giá về 0); bị gọi bổ sung ký quỹ; bị buộc đóng vị thế khi khó vay (buy-in); và short squeeze: khi giá tăng nhanh, người bán khống phải mua lại làm giá tăng thêm. Ví dụ lịch sử: cổ phiếu Volkswagen tháng 10/2008 tăng từ khoảng 211 euro lên trên 1.000 euro trong chưa đầy hai ngày; GameStop tháng 1/2021 chạm 483 USD trong phiên 28/1/2021.
- Quy định nước ngoài: Mỹ yêu cầu xác nhận khả năng vay (locate), có quy tắc thay thế uptick từ 2010 hạn chế lệnh bán khống khi cổ phiếu giảm 10% trở lên; EU cấm bán khống trần, báo cáo cơ quan quản lý khi vị thế đạt 0,1% vốn và công bố công khai khi đạt 0,5%; Hàn Quốc ban đầu chỉ cho khoảng 350 mã, đến 31/3/2025 mở ra khoảng 2.700 mã (nguồn: Vietstock 10/7/2026).
- Hợp đồng tương lai VN30 (hiểu biết chung, chưa đối chiếu văn bản gốc): giá trị hợp đồng bằng điểm chỉ số nhân 100.000 đồng, ký quỹ ban đầu cỡ hai chữ số phần trăm giá trị hợp đồng và được điều chỉnh theo biến động (công ty chứng khoán thường đặt cao hơn), thanh toán bằng tiền theo giá thanh toán cuối cùng, đáo hạn vào thứ Năm thứ ba của tháng. Ví dụ: chỉ số 1.500 điểm thì giá trị hợp đồng 150 triệu đồng, ký quỹ 15% là 22,5 triệu đồng, mỗi 10 điểm thay đổi là 1 triệu đồng lãi hoặc lỗ. Vì ký quỹ chỉ là một phần, đòn bẩy cao nên cả lãi và lỗ lớn nhanh. Chi phí gồm phí giao dịch và phí duy trì ký quỹ. "Đội short" là cách gọi trong bài giảng cho nhóm cùng vào vị thế bán; "cover" là đóng vị thế khi giá về vùng mục tiêu.
- Tình trạng pháp lý tại thời điểm khoá học (cuối 2021): Luật Chứng khoán 2019 có hiệu lực 1/1/2021; Nghị định 155/2020/NĐ-CP và Thông tư 120/2020/TT-BTC (ban hành 31/12/2020) đã có khung ban đầu cho bán khống có tài sản bảo đảm, qua hệ thống vay và cho vay chứng khoán của VSD, chỉ áp dụng cho cổ phiếu và chứng chỉ quỹ niêm yết, không được bán khống trong 5 ngày làm việc trước ngày đăng ký cuối cùng. Nhưng thiếu tiêu chí chọn chứng khoán được phép bán khống nên theo Báo Đầu Tư (11/5/2023) hoạt động này "bị ngưng trệ". Vì vậy với nhà đầu tư thường, cách short duy nhất là phái sinh VN30, đúng như thầy nói.
- Hiện hành (tháng 11/2026): bán khống ở thị trường cơ sở vẫn chưa vận hành. Vietstock (10/7/2026) viết rằng bán khống có kiểm soát đã đưa vào Đề án nâng hạng và đang được nghiên cứu; Diễn đàn Doanh nghiệp (19/11/2025) dẫn lộ trình nghiên cứu 2026-2028 theo Quyết định 2014/QĐ-TTg. Hạ tầng CCP dự kiến chạy muộn nhất quý 1/2027.
- Tấn công đầu cơ bán khống nội tệ (hiểu biết chung): một số quỹ đầu cơ bán khống đồng tiền của quốc gia giữ tỷ giá cố định hoặc yếu, như đồng bảng Anh ngày 16/9/1992 và đồng baht Thái năm 1997, buộc ngân hàng trung ương phá giá hoặc thả nổi. Chưa mở nguồn trong lần tra này; từ khoá: "Black Wednesday 1992 George Soros", "khủng hoảng tài chính châu Á 1997 baht".

**Liên hệ với bài học:** Thầy thích short vì thị trường có chu kỳ giảm, và Việt Nam chỉ cho short qua phái sinh. Cần nhớ phái sinh có đáo hạn, ký quỹ biến động và đòn bẩy, nên khác bán khống cổ phiếu kiểu nước ngoài (không đáo hạn, trả cổ phiếu khi muốn).

**Đọc thêm:** [Wikipedia tiếng Anh - Short (finance)](https://en.wikipedia.org/wiki/Short_(finance)); [Wikipedia tiếng Anh - Short squeeze](https://en.wikipedia.org/wiki/Short_squeeze); [Báo Đầu Tư - Hoàn thiện cơ chế bán khống tại Việt Nam](https://baodautu.vn/phap-luat-ve-ban-khong-va-kinh-nghiem-cho-viet-nam---bai-3-hoan-thien-co-che-ban-khong-tai-viet-nam-d189327.html); [Vietstock - Quản lý giao dịch bán khống (10/7/2026)](https://vietstock.vn/2026/07/quan-ly-giao-dich-ban-khong-kinh-nghiem-quoc-te-va-ham-y-chinh-sach-cho-lo-trinh-nang-hang-thi-truong-viet-nam-143-1464256.htm); [Diễn đàn Doanh nghiệp - Bán khống và T0 dự kiến 2026](https://diendandoanhnghiep.vn/trien-khai-nghiep-vu-ban-khong-va-thuc-hien-giao-dich-t0-du-kien-vao-2026-10165058.html)

### Chứng quyền có bảo đảm (covered warrant)

**Thầy nhắc ở:** B17 02:52 - học viên kể ví dụ chứng quyền Hoà Phát của SSI.

**Là gì:** Chứng quyền có bảo đảm (CW) là chứng khoán do công ty chứng khoán phát hành, cho người nắm giữ quyền (không phải nghĩa vụ) mua hoặc bán một chứng khoán cơ sở với tổ chức phát hành theo giá định trước, hoặc nhận phần chênh lệch giữa giá thực hiện và giá cơ sở vào ngày thực hiện. Giao dịch trên sàn như cổ phiếu.

**Giải thích:**
- Thị trường Việt Nam bắt đầu giao dịch CW từ ngày 28/6/2019 trên HOSE, với các tổ chức phát hành đầu tiên như SSI, HSC và VCSC, chứng khoán cơ sở là cổ phiếu trong rổ VN30.
- Các yếu tố chính: giá thực hiện (giá chốt trước), tỷ lệ chuyển đổi (bao nhiêu CW ứng với một cổ phiếu cơ sở), ngày đáo hạn (CW thường có vòng đời vài tháng đến vài năm; Wikipedia ghi trung bình khoảng 6 đến 12 tháng, một số dài hơn). Người mua trả phí quyền chọn, và với CW mua, lỗ tối đa bằng số tiền đã bỏ ra.
- Tổ chức phát hành phòng ngừa rủi ro bằng cách mua cổ phiếu cơ sở trong thị trường theo mức delta, rồi điều chỉnh khi giá thay đổi. Vì vậy khi nhiều người mua CW, cũng có thể tạo thêm cầu cho cổ phiếu cơ sở (hiểu biết chung).
- Ví dụ tính nhanh (giả định): CW mua có giá thực hiện 30.000 đồng, tỷ lệ chuyển đổi 5:1, giá phát hành 1.000 đồng. Nếu lúc đáo hạn cổ phiếu cơ sở là 36.000 đồng, giá trị nội tại là (36.000 - 30.000) / 5 = 1.200 đồng, lãi 200 đồng trên mỗi CW. Nếu cổ phiếu ở dưới 30.000 đồng thì CW về 0 và mất 1.000 đồng đã mua.
- Chi tiết điều khoản của từng mã nằm trong bản công bố thông tin của tổ chức phát hành; tôi chưa mở được các bản đó trong lần tra này.

**Liên hệ với bài học:** Ví dụ chứng quyền Hoà Phát minh hoạ đòn bẩy: số tiền nhỏ, biên lãi lỗ rất lớn nhưng có thời hạn, khác hẳn việc giữ cổ phiếu vô thời hạn.

**Đọc thêm:** [Wikipedia tiếng Việt - Chứng quyền có bảo đảm](https://vi.wikipedia.org/wiki/Chứng_quyền_có_bảo_đảm); [Wikipedia tiếng Anh - Covered warrant](https://en.wikipedia.org/wiki/Covered_warrant)

## Cụm 4. Vay, thâu tóm và giao dịch của người nội bộ

### Cầm cố cổ phiếu, trần giá cho vay, vay kho (3:7, 2:8) và tài sản bảo đảm bằng cổ phiếu

**Thầy nhắc ở:** B13 03:46, B16 01:53, B17 01:11 - thầy nêu định giá tài sản bảo đảm; học viên coi vay kho là nguy hiểm nhất; bàn trường hợp Novaland.

**Là gì:** Cầm cố cổ phiếu là việc dùng cổ phiếu làm tài sản bảo đảm cho một khoản vay. Có hai kênh chính: margin (vay ký quỹ ngay tại công ty chứng khoán, cổ phiếu mua vào là tài sản bảo đảm) và vay ngoài, thường qua ngân hàng, tổ chức tín dụng, công ty tài chính hoặc cá nhân nhận cầm cố cổ phiếu trong "kho". "Vay kho" là cách gọi của giới đầu tư khi gửi cổ phiếu vào kho của bên cho vay để lấy tiền, kèm tỷ lệ vay như 3:7 hoặc 2:8.

**Giải thích:**
- Margin tại công ty chứng khoán: chỉ được dùng cho các mã nằm trong danh sách đủ điều kiện do sở công bố định kỳ (ví dụ HOSE công bố danh sách 65 mã không đủ điều kiện margin quý IV/2026 ngày 6/10/2026, loại các mã diện cảnh báo, kiểm soát, hạn chế giao dịch, lỗ, kiểm toán ngoại trừ). Tỷ lệ ký quỹ ban đầu và tỷ lệ gọi ký quỹ do công ty đặt trong khung pháp luật (hiểu biết chung: tỷ lệ ký quỹ ban đầu tối thiểu 50% giá trị lệnh, chưa đối chiếu văn bản gốc).
- Vay kho và cầm cố ngoài: giá trị cho vay thường là một tỷ lệ của giá thị trường, và bên cho vay định giá lại hằng ngày. Cách hiểu "3:7" hay "2:8" phụ thuộc quy ước từng bên (tỷ lệ vay trên giá trị tài sản hay phần tự có trên phần vay), nên cần hỏi rõ hợp đồng. Rủi ro chính: giá giảm sâu thì bên cho vay có quyền gọi thêm tài sản hoặc xử lý (bán) cổ phiếu bảo đảm, có thể bán dồn ép trên thị trường làm giá giảm tiếp (bán giải chấp).
- Rủi ro thêm: tài sản bảo đảm là cổ phiếu có tính thanh khoản thấp, bị khoá giao dịch hoặc rơi vào diện hạn chế thì khó bán; một cổ đông lớn cầm cố nhiều cổ phiếu thì khi giá giảm lực bán giải chấp có thể rất lớn.
- Về trường hợp Novaland: tôi chưa tìm được nguồn đáng tin trong lần tra này để nêu diễn biến cụ thể; từ khoá gợi ý: "Novaland cầm cố cổ phiếu cổ đông lớn", "NVL bán giải chấp 2022". Phần quy định định giá tài sản bảo đảm và quyền của trái chủ trong cầm cố ngoài công ty chứng khoán cũng chưa được đối chiếu với văn bản gốc.

**Liên hệ với bài học:** Cầm cố và vay kho là cách đòn bẩy ngoài tầm nhìn của sàn nên học viên coi là nguy hiểm: không có cơ chế cảnh báo công khai, chỉ khi giá rơi mới lộ ra qua đợt bán giải chấp.

**Đọc thêm:** [Báo Pháp luật - HOSE đưa 65 mã vào diện không được margin quý IV/2026](https://doanhnhan.baophapluat.vn/hose-dua-65-ma-chung-khoan-vao-dien-khong-duoc-giao-dich-margin-quy-iv-2026.html)

### Chào mua công khai, premium khi mua nguyên lô (control premium), ngưỡng sở hữu 25% và 50%

**Thầy nhắc ở:** B15 01:05, B15 01:08 - thầy nói trả cao hơn khoảng 30-35% là kinh nghiệm.

**Là gì:** Chào mua công khai (tender offer, mandatory offer) là việc một bên công bố mua cổ phiếu của công ty đại chúng với giá và thời hạn xác định, gửi tới tất cả cổ đông. Control premium là phần giá cao hơn giá thị trường mà người mua chịu trả để giành quyền kiểm soát công ty.

**Giải thích:**
- Ngưỡng sở hữu: ở Việt Nam, luật quy định người mua đạt tới 25% cổ phiếu có quyền biểu quyết của công ty đại chúng mà không phải qua giao dịch bình thường thì phải thực hiện chào mua công khai (Luật Chứng khoán 2019, hiệu lực 1/1/2021; hiểu biết chung, chưa mở văn bản gốc nên cần đối chiếu điều khoản). Ngưỡng 50% là ngưỡng đa số, quyết định các nghị quyết thông thường của đại hội cổ đông, và 65% cho các nội dung quan trọng theo Luật Doanh nghiệp 2020 (hiểu biết chung, cần kiểm lại).
- Mục đích của quy định chào mua bắt buộc, theo Wikipedia: bảo vệ cổ đông thiểu số khi quyền kiểm soát đổi chủ và buộc người mua trả phần bù giá cho quyền kiểm soát. Ngưỡng ở các nước khác nhau: Anh khoảng 30%, Úc và Canada 20%, Brazil và Ấn Độ 25%, Nhật và Thuỵ Sĩ một phần ba; Mỹ không có yêu cầu chào mua bắt buộc.
- Premium: khi nắm đủ tỷ lệ kiểm soát, người mua có quyền bổ nhiệm hội đồng quản trị, chia cổ tức, sáp nhập. Phần bù này vì thế thường lớn hơn giá thị trường của cổ phiếu lẻ. Con số 30 đến 35% thầy nói là kinh nghiệm; mức thường được nhắc trong các thương vụ M&A thường nằm trong khoảng vài chục phần trăm, nhưng tôi chưa tìm được số liệu thống kê có nguồn cho Việt Nam.
- Ví dụ giả định: giá thị trường 20.000 đồng, premium 30% thì giá chào mua là 26.000 đồng; mua 25% của 100 triệu cổ phiếu tức 25 triệu cổ phiếu sẽ cần 650 tỷ đồng.

**Liên hệ với bài học:** Mục này giải thích vì sao khi thương vụ thâu tóm sắp diễn ra, giá thường nhảy lên: thị trường định giá phần bù kiểm soát, và vì sao cổ phiếu có free float thấp, nắm nhiều cổ đông lớn, khó thành mục tiêu thâu tóm.

**Đọc thêm:** [Wikipedia tiếng Anh - Mandatory offer](https://en.wikipedia.org/wiki/Mandatory_offer)

### Giao dịch nội gián và công bố giao dịch của người nội bộ, cổ đông lớn

**Thầy nhắc ở:** B6 03:12, B9 02:41, B11 01:46, B11 03:15 - thầy nói nhiều người trong cuộc đánh chứng khoán, ví dụ chủ tịch đăng ký bán 5 triệu cổ phiếu và ông Quyết đăng ký bán 175 triệu cổ phiếu.

**Là gì:** Giao dịch nội gián là mua bán chứng khoán dựa trên thông tin quan trọng chưa công bố của doanh nghiệp, hoặc tiết lộ thông tin đó cho người khác giao dịch. Còn giao dịch của người nội bộ (lãnh đạo, thành viên hội đồng quản trị, cổ đông lớn, người có liên quan) bằng thông tin đã công khai là hợp pháp nhưng phải báo cáo và công bố.

**Giải thích:**
- Khái niệm chung: nhiều nước cấm giao dịch dựa trên thông tin quan trọng chưa công bố; người nội bộ vẫn được giao dịch cổ phiếu công ty mình nếu không dùng thông tin ấy và phải báo cáo (Mỹ dùng Form 4 trong vài ngày làm việc). Tranh luận học thuật: Milton Friedman cho rằng áp lực mua bán của người nội bộ chính là một dạng thông tin cho thị trường; nghiên cứu khác cho rằng giao dịch nội gián trái phép làm tăng chi phí vốn của doanh nghiệp.
- Khung pháp lý Việt Nam: Luật Chứng khoán 2019 (hiệu lực 1/1/2021); Nghị định 155/2020/NĐ-CP (sửa đổi bởi Nghị định 245/2025/NĐ-CP); Thông tư 96/2020/TT-BTC về công bố thông tin (ban hành 16/11/2020, hiệu lực 1/1/2021), được sửa đổi bởi Thông tư 68/2024/TT-BTC (hiệu lực 2/11/2024), Thông tư 18/2025/TT-BTC (hiệu lực 5/5/2025) và Thông tư 08/2026/TT-BTC (hiệu lực 3/2/2026), hợp nhất tại Văn bản hợp nhất 10/VBHN-BTC ký ngày 20/4/2026.
- Thời hạn đăng ký và công bố: theo hiểu biết chung, người nội bộ và người liên quan phải báo cáo sở giao dịch và UBCKNN trước ngày giao dịch ít nhất 3 ngày làm việc và công bố sau khi hoàn tất trong vòng 3 ngày làm việc; cổ đông lớn (từ 5% vốn) có nghĩa vụ báo cáo khi tỷ lệ thay đổi. Tôi chưa đọc được Điều 31 và 33 của văn bản hợp nhất nên số ngày và ngưỡng cần đối chiếu. Hình sự: Bộ luật Hình sự có tội danh sử dụng thông tin nội bộ để mua bán chứng khoán và tội thao túng thị trường (hiểu biết chung, cần đối chiếu điều khoản). Mức xử phạt hành chính nằm trong Nghị định 156/2020/NĐ-CP và các sửa đổi (cần đối chiếu).
- Tác động thường thấy lên giá: thông tin đăng ký bán lớn của người nội bộ hay làm giá điều chỉnh vì thị trường coi đó là tín hiệu thiếu niềm tin; ngược lại đăng ký mua thường được coi là tín hiệu tích cực. Đây là xu hướng, không phải quy luật.
- Các ví dụ cụ thể thầy nêu (chủ tịch đăng ký bán 5 triệu cổ phiếu, ông Quyết đăng ký bán 175 triệu cổ phiếu): chưa tìm được nguồn đáng tin để xác nhận con số và công văn gốc; từ khoá: "FLC Trịnh Văn Quyết đăng ký bán cổ phiếu 2022". Phụ lục không suy diễn về các vụ việc cá nhân ngoài thông tin đã được cơ quan chức năng hoặc báo chí chính thống công bố.

**Liên hệ với bài học:** Thầy dùng thông tin đăng ký giao dịch của người nội bộ như tín hiệu cần đọc cùng với diễn biến giá. Cần phân biệt "công bố giao dịch người nội bộ" (hợp pháp, minh bạch) với "giao dịch nội gián" (bất hợp pháp).

**Đọc thêm:** [Wikipedia tiếng Anh - Insider trading](https://en.wikipedia.org/wiki/Insider_trading); [Luật Việt Nam - Văn bản hợp nhất 10/VBHN-BTC năm 2026](https://luatvietnam.vn/chung-khoan/van-ban-hop-nhat-10-vbhn-btc-2026-huong-dan-cong-bo-thong-tin-thi-truong-chung-khoan-432898-d5.html); [Vietstock - Quản lý giao dịch bán khống (nêu Nghị định 155/2020)](https://vietstock.vn/2026/07/quan-ly-giao-dich-ban-khong-kinh-nghiem-quoc-te-va-ham-y-chinh-sach-cho-lo-trinh-nang-hang-thi-truong-viet-nam-143-1464256.htm)

## Cụm 5. Dòng vốn, dòng tiền thông minh và tài sản số

### ETF, dòng vốn quỹ ngoại vào Việt Nam và dòng vốn toàn cầu (Mỹ, Đài Loan, Nhật, Thái Lan, Singapore)

**Thầy nhắc ở:** B1 02:54, B1 02:51 - thầy khoanh ETF trên slide, nói tiền Mỹ vào châu Á và rút về khi Mỹ giảm.

**Là gì:** ETF ngoại là quỹ niêm yết ở nước ngoài mô phỏng chỉ số hoặc rổ cổ phiếu Việt Nam. Dòng vốn ngoại là phần tiền của nhà đầu tư nước ngoài mua ròng hoặc bán ròng trên thị trường. Với thị trường mới nổi và cận biên như Việt Nam, dòng vốn này nhạy với tâm lý toàn cầu và với lãi suất, đồng đô la Mỹ.

**Giải thích:**
- Cơ chế ETF: tổ chức tham gia lập quỹ nộp rổ chứng khoán để nhận chứng chỉ quỹ và ngược lại, nên khi tiền vào quỹ nhiều ("inflow") quỹ phải mua cổ phiếu trong rổ, khi tiền ra ("outflow") quỹ phải bán. Wikipedia lưu ý các giao dịch mua bán của ETF có thể ảnh hưởng đáng kể giá tài sản cơ sở.
- ETF nào mua Việt Nam (hiểu biết chung, chưa đối chiếu danh sách mới nhất): ví dụ quỹ VanEck Vietnam ETF niêm yết ở Mỹ, Xtrackers FTSE Vietnam UCITS ETF ở châu Âu, Fubon FTSE Vietnam ETF ở Đài Loan. Danh mục và quy mô thay đổi theo từng kỳ, cần tra trang của quỹ.
- Đồng pha, ngược pha, lệch pha: nói về mối quan hệ giữa chuỗi dòng vốn hoặc chu kỳ của hai thị trường. Đồng pha là cùng hướng cùng lúc, ngược pha là ngược hướng, lệch pha là cùng hướng nhưng có độ trễ. Thầy dùng khi nói dòng vốn Mỹ vào châu Á rồi rút về khi Mỹ giảm: hai thị trường đồng pha ở chiều rút.
- Nâng hạng và dòng vốn thụ động (diễn biến sau khoá học): FTSE Russell công bố ngày 8/10/2025 xác nhận nâng Việt Nam từ thị trường cận biên lên mới nổi thứ cấp. Theo Báo Đấu Thầu (đăng lại VGP), HSBC ước tính vốn thụ động có thể tăng thêm khoảng 1,5 đến 2 tỷ USD trong 6 tháng đầu sau nâng hạng; Ngân hàng Thế giới dự báo dòng vốn ngắn hạn khoảng 5 tỷ USD trước và sau nâng hạng; tỷ trọng Việt Nam trong chỉ số FTSE Emerging Market khoảng 0,5% (theo ước tính HSBC dẫn Reuters), tài sản đi theo bộ chỉ số FTSE Russell khoảng 18.100 tỷ USD cuối năm 2024. Thời điểm hiệu lực: các nguồn ghi đầu tháng 9/2026, trong đó một số ghi 21/9/2026. Thông tư 08/2026/TT-BTC (hiệu lực 3/2/2026) cho phép nhà đầu tư nước ngoài đặt lệnh qua tổ chức môi giới toàn cầu mà không cần mở tài khoản giao dịch riêng, một điều kiện để mở đường dòng vốn này.
- Cần phân biệt dự báo với kết quả thực tế: số liệu trên là ước tính tại thời điểm công bố, không phải dòng vốn đã giải ngân. Tôi chưa tìm được số liệu dòng vốn thực hiện sau thời điểm nâng hạng.

**Liên hệ với bài học:** Thầy dùng dòng vốn ngoại như một chất xúc tác cho kịch bản tiền đổ về nhóm bluechip. Bài học là khi ETF mua, tiền chảy vào các mã có trong rổ chỉ số theo tỷ trọng, nên nhóm vốn hoá lớn, free float cao hưởng lợi trước.

**Đọc thêm:** [Báo Đấu Thầu - Thị trường chứng khoán Việt Nam được nâng hạng](https://baodauthau.vn/thi-truong-chung-khoan-viet-nam-duoc-nang-hang-post186368.html); [VnEconomy - Thị trường chứng khoán Việt Nam bước vào nhóm mới nổi thứ cấp](https://vneconomy.vn/thi-truong-chung-khoan-viet-nam-chinh-thuc-buoc-vao-nhom-moi-noi-thu-cap.htm); [Người Đưa Tin - Bộ Tài chính nới cơ chế cho nhà đầu tư nước ngoài từ 3/2/2026](https://www.nguoiduatin.vn/bo-tai-chinh-noi-co-che-giao-dich-chung-khoan-cho-nha-dau-tu-nuoc-ngoai-tu-3-2-2026-204260203210031525.htm); [Wikipedia tiếng Anh - Exchange-traded fund](https://en.wikipedia.org/wiki/Exchange-traded_fund)

### Dòng vốn ngoại đầu 2022: quỹ Đài Loan 5.000 tỷ, ETF Fubon, các quỹ mua ròng tháng 1/2022

**Thầy nhắc ở:** B13 02:37, B16 00:52, B16 00:53 - thầy dẫn làm chất xúc tác cho kịch bản tiền về bluechip.

**Là gì:** Thầy nhắc đến các thông tin về dòng tiền từ quỹ Đài Loan (khoảng 5.000 tỷ đồng) và ETF Fubon, cùng việc các quỹ ngoại mua ròng trong tháng 1/2022.

**Giải thích:** Chưa tìm được nguồn đáng tin trong lần tra này để xác nhận tên quỹ, quy mô 5.000 tỷ đồng và thời điểm giải ngân thực tế. Từ khoá gợi ý: "Fubon FTSE Vietnam ETF 2022", "quỹ Đài Loan mua cổ phiếu Việt Nam 5.000 tỷ", "khối ngoại mua ròng tháng 1/2022 HOSE". Khi tra cần phân biệt: số tiền huy động (IPO) của quỹ, số tiền thực giải ngân vào cổ phiếu Việt Nam, và số mua ròng của khối ngoại hằng ngày do sở công bố. Ba con số này thường lệch nhau về thời điểm và quy mô.

**Liên hệ với bài học:** Đây là ví dụ thầy dùng để nói về kỳ vọng dòng tiền về bluechip; nên coi là thông tin thầy dẫn trong bối cảnh lúc đó, chưa được kiểm chứng ở đây.

**Đọc thêm:** [Wikipedia tiếng Anh - Exchange-traded fund](https://en.wikipedia.org/wiki/Exchange-traded_fund) (kiến thức nền về dòng tiền vào ra của ETF)

### Dòng tiền thông minh (smart money, "big boy")

**Thầy nhắc ở:** B7 01:22, B7 01:43 - thầy dùng trong ẩn dụ rót nước.

**Là gì:** "Dòng tiền thông minh" là cách gọi dòng tiền của các nhà đầu tư lớn, có thông tin tốt và có nghiệp vụ như quỹ, tự doanh, nhà đầu tư tổ chức. Ở Việt Nam người ta hay gọi các tay chơi lớn là "big boy".

**Giải thích:**
- Cách nhận diện thường dùng: khối lượng khớp lớn bất thường ở vùng giá đi ngang, mua ròng của khối ngoại hoặc tự doanh, lệnh chia nhỏ đặt đều (xem mục chia lệnh), giá đóng cửa gần mức cao nhất của phiên. Đây là cách suy luận từ dữ liệu, không có thước đo chính thức.
- Hạn chế: nhãn "thông minh" thường được dán sau khi giá đã chạy; khối ngoại hoặc tự doanh mua ròng không bảo đảm đúng, vì họ cũng có thể sai hoặc mua theo cơ chế (ví dụ ETF mua theo rổ). Tôi chưa tìm được nguồn học thuật chuẩn cho thuật ngữ này; Wikipedia chỉ có trang định hướng và dẫn tới "smart money index" dùng trong phân tích tài chính.
- Ẩn dụ rót nước trong bài: tổ chức rót "nước" (tiền) từ từ để mực nước (giá) lên mà không gây xáo trộn, khác với dòng tiền nhỏ lẻ vào ồ ạt.

**Liên hệ với bài học:** Mục này giúp hiểu vì sao thầy đòi hỏi quan sát dấu vết dòng tiền, nhưng cần nhớ đây là giả định về hành vi, không phải sự thật có thể đo trực tiếp.

**Đọc thêm:** [Wikipedia tiếng Anh - Iceberg order](https://en.wikipedia.org/wiki/Iceberg_order); [Wikipedia tiếng Anh - Algorithmic trading](https://en.wikipedia.org/wiki/Algorithmic_trading)

### Bitcoin và tài chính phi tập trung (DeFi)

> Mục này không liên quan đến đầu tư nên đã chuyển sang [PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md](../../ngoai-dau-tu/phu-luc/PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md).

## Cụm 6. Forex (giao dịch ngoại hối bán lẻ)

### Forex cơ chế: lot, pip, đòn bẩy 1:100 và 1:200, ký quỹ, stop out, mức nạp tối thiểu

> Mục này không liên quan đến đầu tư nên đã chuyển sang [PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md](../../ngoai-dau-tu/phu-luc/PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md).

### Forex chi phí: phí qua đêm (swap, rollover), hoa hồng (commission), spread

> Mục này không liên quan đến đầu tư nên đã chuyển sang [PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md](../../ngoai-dau-tu/phu-luc/PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md).

### Forex sàn giao dịch: dealing desk, market maker so với ECN, STP; giấy phép FSA, FCA; tình trạng pháp lý ở Việt Nam

> Mục này không liên quan đến đầu tư nên đã chuyển sang [PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md](../../ngoai-dau-tu/phu-luc/PL06a-thi-truong-chung-khoan-viet-nam-va-san-pham.md).

## Cụm 7. Lịch sử thị trường, hành vi và các chuyện lẻ

### Đấu giá cổ phần doanh nghiệp nhà nước 2005-2007, đặt cọc 10% và thị trường Việt Nam 2004-2008

**Thầy nhắc ở:** B15 01:36, B15 01:38 - thầy hồi tưởng bùng nổ 2006-2007, đỉnh và sụp đổ 2007-2008, ví dụ PVD.

**Là gì:** Đấu giá cổ phần lần đầu (IPO qua đấu giá) là cách bán cổ phần của doanh nghiệp nhà nước khi cổ phần hoá: nhà đầu tư đăng ký mua theo giá mình đặt, giá khớp theo nguyên tắc từ cao xuống thấp cho đến khi bán hết. Đặt cọc là khoản tiền nhà đầu tư nộp trước để bảo đảm thanh toán nếu trúng.

**Giải thích:**
- Bối cảnh pháp lý: theo trang Wikipedia về cổ phần hoá, Nghị định 187/2004/NĐ-CP yêu cầu đấu giá cổ phần lần đầu, giúp nhà nước thu thêm nhiều tiền so với bán theo giá định sẵn; Nghị định 64/2002/NĐ-CP giới hạn nhà đầu tư nước ngoài ở mức 30%. Đến năm 2008 có khoảng 3.000 doanh nghiệp vừa và nhỏ được cổ phần hoá.
- Tiền đặt cọc 10% giá trị cổ phần đăng ký mua theo giá khởi điểm là mức tôi biết từ hiểu biết chung, chưa đối chiếu văn bản gốc.
- Diễn biến thị trường 2006-2008 (hiểu biết chung, chưa đối chiếu nguồn trong lần tra này): VN-Index tăng rất mạnh trong 2006 và đầu 2007, lập đỉnh khoảng 1.170 điểm vào ngày 12/3/2007, rồi giảm sâu trong 2008 và chạm đáy ở khoảng 235 điểm vào đầu năm 2009. Vụ việc đặt giá đấu cao rồi giá thị trường xuống thấp hơn giá đấu cũng xảy ra ở nhiều thương vụ giai đoạn này.
- PVD (cổ phiếu khoan dầu khí): giá đấu và giá đỉnh chưa tra được nguồn đáng tin; từ khoá: "PVD đấu giá cổ phần 2006", "PVD đỉnh 2007".
- Cho vay cầm cố thời đó: ngân hàng và công ty chứng khoán cho vay có tài sản bảo đảm là cổ phiếu khi thị trường tăng nóng, và các vụ bán giải chấp khuếch đại đà giảm 2008 (hiểu biết chung).

**Liên hệ với bài học:** Thầy dùng giai đoạn 2006-2008 như bài học về chu kỳ bong bóng: tín dụng bằng cổ phiếu, giá đấu cao, kỳ vọng tăng vô hạn và cuối cùng là sụp đổ. Các cơ chế "kích giá" rồi "giải chấp" thầy mô tả cũng lặp lại ở các chu kỳ sau.

**Đọc thêm:** [Wikipedia tiếng Việt - Cổ phần hoá](https://vi.wikipedia.org/wiki/Cổ_phần_hóa); [Wikipedia tiếng Anh - Ho Chi Minh City Stock Exchange](https://en.wikipedia.org/wiki/Ho_Chi_Minh_City_Stock_Exchange)

### Hiệu ứng nghỉ Tết trên thị trường chứng khoán Việt Nam

**Thầy nhắc ở:** B14 00:45 - thầy dự báo giữ qua Tết có thưởng.

**Là gì:** Là hiện tượng thống kê cho rằng chỉ số thường có xu hướng tăng quanh kỳ nghỉ Tết Nguyên Đán: trước Tết có tâm lý thận trọng hoặc chốt lời, sau Tết dòng tiền và tâm lý được kỳ vọng tốt hơn.

**Giải thích:** Chưa tìm được nguồn đáng tin trong lần tra này để dẫn thống kê VN-Index trước và sau Tết qua nhiều năm, hoặc diễn biến cụ thể của Tết 2022. Từ khoá gợi ý: "thống kê VN-Index trước và sau Tết Nguyên Đán", "hiệu ứng Tết chứng khoán Việt Nam". Cần nhớ khi đọc: các hiệu ứng theo lịch kiểu này thường được nhắc ở nhiều thị trường, nhưng độ lặp lại không ổn định qua các năm, và số năm quan sát thường quá ít để kết luận chắc chắn. Hiệu ứng nghỉ lễ còn bị che bởi chu kỳ vĩ mô, lãi suất và tin doanh nghiệp.

**Liên hệ với bài học:** Dự báo "giữ qua Tết có thưởng" của thầy nên được hiểu như một kịch bản xác suất. Không nên coi là quy luật.

**Đọc thêm:** Chưa có đường dẫn đã mở để giới thiệu.

### Đường cong tâm lý và FOMO trong giao dịch

**Thầy nhắc ở:** B4 02:35 - chu kỳ cảm xúc nghi ngờ, hy vọng, lạc quan, sợ hãi.

**Là gì:** Đường cong tâm lý mô tả chu kỳ cảm xúc của đám đông nhà đầu tư theo diễn biến giá: từ nghi ngờ ở đáy, hy vọng, lạc quan, hưng phấn ở đỉnh rồi hoảng loạn khi giảm. FOMO (fear of missing out, sợ bỏ lỡ) là thôi thúc mua theo vì thấy người khác đang lời.

**Giải thích:** Theo Wikipedia về tâm lý nhà đầu tư, tâm lý đám đông thường dao động giữa lạc quan và bi quan; chú ý và khối lượng giao dịch cao có thể tự kéo thêm sự chú ý; nhà đầu tư nhỏ lẻ hay mua và bán đồng loạt; và bi quan cực độ thường theo sau bởi nhịp phục hồi lớn hơn bình thường (tín hiệu ngược chiều). Phần đầy đủ về đường cong tâm lý nằm trong Phụ lục PL09 (tâm lý, giáo dục, quản trị, kỹ năng).

**Liên hệ với bài học:** Mục này chỉ nhắc nhanh: khi thấy mình muốn mua vì sợ lỡ cơ hội, đó thường là lúc nên tạm dừng và xem lại kế hoạch.

**Đọc thêm:** [Wikipedia tiếng Anh - Investor sentiment](https://en.wikipedia.org/wiki/Investor_sentiment)

### Gian lận thẻ để bán lại bản quyền phần mềm giá rẻ

**Thầy nhắc ở:** B6 01:10 - thầy nhắc ngắn.

**Là gì:** Một số nơi bán khoá bản quyền phần mềm giá rất rẻ có thể mua khoá bằng thẻ thanh toán bị đánh cắp (carding) hoặc dùng các phương thức gian lận khác rồi bán lại cho người khác.

**Giải thích:** Chưa tìm được nguồn đáng tin trong lần tra này về cơ chế cụ thể. Điều có thể nói ở mức chung: khi chủ thẻ phát hiện giao dịch lạ, họ khiếu nại hoàn tiền (chargeback), nhà phát hành phần mềm có thể thu hồi khoá, nên người mua cuối cùng mất bản quyền. Việc mua bán khoá nguồn gốc không rõ còn có thể vi phạm điều khoản sử dụng và pháp luật. Từ khoá gợi ý để tự tra: "carding chargeback license key bị thu hồi", "bản quyền phần mềm giá rẻ rủi ro".

**Liên hệ với bài học:** Thầy nhắc làm ví dụ về hàng giá rẻ bất thường thường có nguồn gốc không sạch; nguyên tắc chung là hỏi vì sao rẻ.

**Đọc thêm:** Chưa có đường dẫn đã mở để giới thiệu.

