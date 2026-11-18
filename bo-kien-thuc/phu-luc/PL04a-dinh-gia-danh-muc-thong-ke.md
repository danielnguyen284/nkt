# Phụ lục PL04a - Định giá, lý thuyết danh mục và thống kê tài chính (phần 1)

> Phụ lục của Bộ kiến thức NKT. Giải thích những khái niệm thầy nhắc tới trong bài giảng mà chưa giảng đầy đủ. Nội dung được tra cứu từ các nguồn bên ngoài (thời điểm tra cứu: tháng 11/2026), không phải lời thầy.

Lưu ý chung: phụ lục chỉ giải thích khái niệm, không phải lời khuyên đầu tư. Các ví dụ số là số giả định để người đọc tự tính lại bằng tay hoặc Excel. Một số đường dẫn Wikipedia được viết với ký hiệu %5F thay cho dấu gạch dưới; trình duyệt vẫn mở đúng trang.

## Danh sách mục

Cụm 1. Nền tảng: giá trị, giá cả và ba cách tiếp cận định giá
1. Giá trị nội tại, fair value, biên an toàn và câu "Price is what you pay, value is what you get"
2. Giá trị nội tại theo ba lớp giá, kỳ vọng đồng thuận (consensus), "ngài Thị trường" của Graham, trí tuệ đám đông
3. Ẩn dụ người dắt chó của André Kostolany (giá cả và giá trị)
4. Ba cách tiếp cận định giá (thu nhập, tài sản hoặc chi phí, thị trường) và các phương pháp con

Cụm 2. Định giá bằng dòng tiền
5. DCF, FCF, giá trị cuối kỳ (Gordon, exit multiple), chiết khấu dòng tiền về hiện tại
6. Dòng tiền tự do và giá trị doanh nghiệp (FCFF, FCFE, EV, DCF)
7. Chuẩn hoá lợi nhuận qua chu kỳ (hệ số chu kỳ, P/E chu kỳ hoá)
8. Định giá quyền chọn thực và mô hình Black-Scholes (real options)

Cụm 3. Định giá tương đối, lợi thế cạnh tranh và loại cổ phiếu
9. Các bội số định giá (P/E, P/S, P/B, EV/EBITDA, tỷ suất cổ tức, earnings yield, PEG, CAGR, P/E tương đối)
10. Con hào kinh tế và quyền định giá (economic moat, pricing power)
11. Cổ phiếu phòng thủ, cổ phiếu tăng trưởng và chu kỳ ngành

Cụm 4. Định giá đặc thù, theo phần và theo kịch bản
12. Định giá theo tổng các phần (SOTP), theo tài sản, phân tích độ nhạy và kịch bản; nguyên tắc "chia để trị"
13. Định giá tập đoàn đa ngành nợ cao (ví dụ Masan) và NAV (net asset value)
14. Định giá trong M&A, quỹ tương hỗ, quỹ hưu trí, ngân hàng, bảo hiểm
15. Kịch bản A/B/C, mô hình định giá trên Excel và dashboard theo dõi đầu tư

Cụm 5. Thị trường hiệu quả, danh mục và bài học thất bại
16. Giả thuyết thị trường hiệu quả và bước đi ngẫu nhiên (EMH, random walk)
17. Beta, alpha, CAPM và mô hình thị trường (market model)
18. Đầu tư theo chỉ số (index investing)
19. LTCM và sách "Khi các thiên tài thất bại" (Roger Lowenstein)

Cụm 6. Chiến lược đầu tư và quản trị vị thế
20. Đầu tư theo xu thế, "xu thế là bạn" và tranh luận với đầu tư giá trị
21. CAN SLIM của William O'Neil
22. Chỉ báo tâm lý ngược chiều (contrarian sentiment) và chỉ số VIX
23. Đánh gấp thếp (Martingale), anti-Martingale và nhồi lệnh thuận xu hướng (pyramiding)
24. Lệnh cắt lỗ, chốt lời (stop-loss, take-profit) và trượt giá (slippage)
25. Giá vốn bình quân và trung bình giá

Cụm 7. Thống kê, mô hình định lượng và kiểm thử
26. Hồi quy tuyến tính, R và R bình phương, thống kê t, mức ý nghĩa, hồi quy giả
27. Các mô hình chuỗi thời gian ARIMA, GARCH, VAR
28. ARIMA, Machine Learning, Deep Learning, phân tích cụm (clustering), AIQuant
29. Backtest, tối ưu tham số, quá khớp và look-ahead bias

Cụm 8. Ngành quản lý quỹ và nghề phân tích
30. Lợi nhuận bình quân của quỹ đầu tư Mỹ, quỹ quant và quỹ ngoại tại Việt Nam
31. Chứng chỉ CFA (Chartered Financial Analyst)

## Cụm 1. Nền tảng: giá trị, giá cả và ba cách tiếp cận định giá

### Giá trị nội tại, fair value, biên an toàn và câu "Price is what you pay, value is what you get"

**Thầy nhắc ở:** B7 00:55, B7 01:42, B11 02:56 - slide mở đầu phần định giá, thầy nhắc Benjamin Graham cùng nhóm sách "bán đắt".

**Là gì:** Giá trị nội tại (intrinsic value) là giá trị "thật" của doanh nghiệp suy ra từ khả năng sinh lời và tài sản, độc lập với giá giao dịch từng ngày. Fair value (giá trị hợp lý) là ước tính của người định giá về mức giá công bằng. Biên an toàn (margin of safety) là khoảng chênh giữa giá trị nội tại ước tính và giá mua.

**Giải thích:** Graham và Dodd đưa thuật ngữ biên an toàn vào cuốn Security Analysis (1934), Graham nhắc lại trong The Intelligent Investor. Graham viết rằng biên an toàn luôn phụ thuộc vào giá phải trả: lớn ở mức giá này, nhỏ ở mức giá cao hơn, và không còn ở mức giá cao hơn nữa. Công thức đơn giản: biên an toàn = (giá trị nội tại - giá mua) / giá trị nội tại. Ví dụ số: ước tính giá trị nội tại 100.000 đồng, giá thị trường 70.000 đồng thì biên an toàn là (100 - 70) / 100 = 30%. Biên này che cho sai số của chính ước tính (giả định tăng trưởng, lãi suất chiết khấu), không phải bảo đảm không lỗ. Về câu nói: Buffett viết trong thư cổ đông Berkshire Hathaway năm 2008 rằng "Long ago, Ben Graham taught me that Price is what you pay; value is what you get", nghĩa là ông dẫn lại lời thầy mình, đặt ngay trong đoạn nói về việc giá cổ phiếu giảm theo thị trường chung là dịp mua hàng chất lượng khi được giảm giá. Một số trang trên mạng ghi câu này là của Graham hoặc của Buffett, nhưng văn bản thư năm 2008 cho thấy Buffett nêu rõ là học từ Graham. Giá trị nội tại không phải một con số chính xác mà là một khoảng; hai người định giá có thể ra hai con số khác nhau.

**Liên hệ với bài học:** Phần mở đầu định giá của thầy dựa vào tách bạch giữa "giá" (thị trường trả) và "giá trị" (ước tính của mình). Hiểu hai khái niệm này giúp đọc các phần sau về DCF, bội số, kịch bản: tất cả đều là cách ước tính giá trị nội tại. Khác với cách dùng phổ thông: nhiều người nói "định giá thấp" chỉ vì P/E thấp, trong khi theo Graham đó chỉ là điểm xuất phát.

**Đọc thêm:** [Thư cổ đông Berkshire Hathaway 2008](https://www.berkshirehathaway.com/letters/2008ltr.pdf); [Margin of safety (Wikipedia)](https://en.wikipedia.org/wiki/Margin%5Fof%5Fsafety%5F(financial)); [Building in a margin of safety (Morningstar)](https://morningstar.co.uk/uk/news/107923/building-in-a-margin-of-safety-when-buying-shares.aspx)

### Giá trị nội tại theo ba lớp giá, kỳ vọng đồng thuận (consensus), "ngài Thị trường" của Graham, trí tuệ đám đông

**Thầy nhắc ở:** B13 02:01, B13 02:02, B13 03:51 - thầy tách ba lớp giá: ước tính của mình, đánh giá của đám đông, giá thị trường.

**Là gì:** Ba lớp giá là cách nhìn của thầy: (1) giá trị nội tại theo ước tính cá nhân, (2) giá trị mà đám đông (kỳ vọng đồng thuận của giới phân tích, nhà đầu tư) cho là đúng, (3) giá đang giao dịch. "Ngài Thị trường" (Mr. Market) là câu chuyện ngụ ngôn của Graham. Trí tuệ đám đông (wisdom of crowds) là hiện tượng trung bình ước tính của nhiều người độc lập có thể rất sát sự thật.

**Giải thích:** Mr. Market xuất hiện trong chương 8 của The Intelligent Investor (1949): bạn có một người đối tác tên Mr. Market, mỗi ngày anh ta ra giá mua phần của bạn hoặc bán phần của anh ta, lúc bi quan lúc phấn khích. Bạn không bắt buộc phải nhận giá nào. Graham còn nói thị trường ngắn hạn là cỗ máy bỏ phiếu, dài hạn là cái cân. Wisdom of crowds bắt nguồn từ Francis Galton: tại hội chợ Plymouth, 800 người đoán trọng lượng một con bò, trung vị ước tính 1.207 pound, sai lệch dưới 1% so với trọng lượng thật 1.198 pound. Điều kiện để đám đông đúng: các ước tính phải độc lập và đa dạng; trung bình triệt tiêu sai số ngẫu nhiên nhưng không triệt tiêu sai số có hệ thống hoặc thiên kiến chung. Khi ảnh hưởng xã hội, tâm lý bầy đàn xuất hiện thì đám đông có thể sai chung, đó là lúc xuất hiện bong bóng và hoảng loạn. Quan hệ với thị trường hiệu quả: nếu đám đông luôn đúng thì giá phản ánh hết thông tin và không còn gì để "tìm giá trị"; Graham và các nhà đầu tư giá trị cho rằng đám đông đôi khi sai, đó là cơ hội.

**Liên hệ với bài học:** Thầy dùng ba lớp giá để nhắc nhà đầu tư phân biệt "mình nghĩ gì", "thiên hạ nghĩ gì" và "giá đang là gì"; lợi thế đến từ khoảng chênh giữa lớp 1 và lớp 3, còn lớp 2 là thứ cần đối chiếu (đồng thuận quá cao có thể là tín hiệu ngược). Chú ý: phần lớn tài liệu nói trí tuệ đám đông đúng khi độc lập, trong khi giá thị trường chứng khoán Việt Nam có nhiều nhà đầu tư cá nhân cùng đọc một nguồn tin, nên giả định độc lập khó thỏa.

**Đọc thêm:** [Mr. Market (Wikipedia)](https://en.wikipedia.org/wiki/Mr.%5FMarket); [The wisdom of Graham's Mr Market (Morningstar)](https://www.morningstar.com.au/investing/the-wisdom-of-grahams-mr-market); [Wisdom of the crowd (Wikipedia)](https://en.wikipedia.org/wiki/Wisdom%5Fof%5Fthe%5Fcrowd)

### Ẩn dụ người dắt chó của André Kostolany (giá cả và giá trị)

**Thầy nhắc ở:** B7 00:58 - thầy dùng clip chó đuổi con vật nhỏ.

**Là gì:** Ẩn dụ được gán cho nhà đầu cơ André Kostolany: nền kinh tế như người đi dạo, thị trường chứng khoán như con chó chạy tới chạy lui; chó có thể chạy xa phía trước hoặc tụt lại phía sau nhưng cuối cùng phải theo chủ.

**Giải thích:** Các nguồn mô tả phổ biến: "mối quan hệ giữa sàn chứng khoán và nền kinh tế giống như người dắt chó đi dạo; người đi chậm, con chó chạy tới lui". Chủ là kinh tế thực hoặc giá trị nội tại, chó là giá thị trường dao động ngắn hạn. Bài của Josh Brown (The Reformed Broker) kể một biến thể với chó Jack Russell. Tôi không tìm được văn bản gốc tiếng Đức của Kostolany nên câu chữ chính xác và nguồn trích của ẩn dụ chưa kiểm chứng; nên coi đây là cách diễn đạt lưu truyền chứ không phải trích dẫn nguyên văn. Ý nghĩa: dây dắt bằng thun, chó chạy xa hay gần đều có giới hạn, tương tự giá lệch giá trị trong phạm vi nào đó rồi bị kéo lại.

**Liên hệ với bài học:** Thầy dùng clip để minh hoạ giá dao động quanh giá trị. Lưu ý khác biệt: trong ẩn dụ gốc, "chủ" thường là kinh tế vĩ mô; thầy gắn nó với giá trị doanh nghiệp. Ẩn dụ giống ý "Ngài Thị trường" của Graham (mục trên).

**Đọc thêm:** [My favorite analogy for stocks vs the economy (The Reformed Broker)](https://thereformedbroker.com/2018/11/26/my-favorite-analogy-for-stocks-vs-the-economy/comment-page-1); [10 André Kostolany quotes (justETF)](https://justetf.com/en/academy/10-quotes-kostolany.html); [André Kostolany (Wikipedia)](https://en.wikipedia.com/wiki/Andr%C3%A9%5FKostolany)

### Ba cách tiếp cận định giá (thu nhập, tài sản hoặc chi phí, thị trường) và các phương pháp con

**Thầy nhắc ở:** B7 01:55, B7 03:00 - slide "Valuation Approaches, globally".

**Là gì:** Tiêu chuẩn thẩm định giá quốc tế (IVS) chia mọi phương pháp thành ba cách tiếp cận: thị trường (so sánh với tài sản giống hoặc tương tự có giá giao dịch), thu nhập (quy dòng tiền tương lai về một giá trị hiện tại), và chi phí (giá trị bằng chi phí tạo ra tài sản tương đương, trừ hao mòn).

**Giải thích:**
- Thu nhập: chiết khấu dòng tiền (DCF), vốn hoá thu nhập, và phương pháp thu nhập vượt trội (excess earnings) dùng cho tài sản vô hình, tách phần lợi nhuận vượt mức hợp lý do tài sản vô hình tạo ra.
- Thị trường: so sánh bội số (P/E, EV/EBITDA, P/B) với doanh nghiệp tương tự hoặc với giao dịch mua bán trước đó.
- Chi phí: chi phí thay thế (replacement cost, xây tài sản có công năng tương đương theo giá và công nghệ hiện nay) và chi phí tái tạo (reproduction cost, dựng bản sao y hệt); phương pháp cộng gộp (summation) cộng giá trị từng tài sản trừ nợ. Với doanh nghiệp, các biến thể là giá trị sổ sách (BV), giá trị tài sản ròng (NAV, giá trị tài sản trừ nợ phải trả), và RNAV (revalued NAV, đánh giá lại tài sản theo giá thị trường, hay dùng cho bất động sản và công ty địa ốc).
Ví dụ số: tài sản sổ sách 1.000 tỷ, nợ 400 tỷ, nhưng đất đánh giá lại tăng thêm 300 tỷ thì BV = 600 tỷ, RNAV = 900 tỷ. Một lưu ý: IVSC đã đổi số hiệu chương trong các bản sau (có nguồn ghi là IVS 103 trong bản dự thảo 2023); cần kiểm tra bản hiện hành trước khi trích.
Ở Việt Nam, Bộ Tài chính ban hành các Tiêu chuẩn thẩm định giá Việt Nam (TĐGVN), ví dụ TĐGVN 05 về quy trình thẩm định giá (Thông tư 28/2015/TT-BTC) và các tiêu chuẩn 08, 09, 10 (Thông tư 126/2015/TT-BTC) hướng dẫn các cách tiếp cận; năm 2024 có Thông tư 42/2024/TT-BTC về chuẩn mực thẩm định giá bất động sản. Tôi không kiểm được tình trạng hiệu lực mới nhất của từng văn bản.

**Liên hệ với bài học:** Thầy dùng slide này làm bản đồ: mọi kỹ thuật ở các phần sau thuộc một trong ba nhóm. Chọn cách tiếp cận phụ thuộc loại tài sản: công ty tăng trưởng nghiêng thu nhập, công ty địa ốc hay tài sản nặng nghiêng tài sản, và thị trường dùng để đối chiếu chéo.

**Đọc thêm:** [IVS 105 Valuation Approaches (IVSC)](https://www.ivsc.org/wp-content/uploads/2021/10/IVS105ValuationApproaches.pdf); [Valuation approaches and methods (RICS)](https://ww3.rics.org/uk/en/journals/property-journal/valuation-approaches-methods-models.html); [Thông tư 28/2015/TT-BTC (TĐGVN 05, 06, 07)](https://caselaw.vn/van-ban-phap-luat/263985-thong-tu-28-2015-tt-btc-ve-tieu-chuan-tham-dinh-gia-viet-nam-so-05-06-va-07-do-bo-truong-bo-tai-chinh-ban-hanh); [Thông tư 126/2015/TT-BTC (TĐGVN 08, 09, 10)](https://caselaw.vn/van-ban-phap-luat/263552-thong-tu-126-2015-tt-btc-ve-tieu-chuan-tham-dinh-gia-viet-nam-so-08-09-va-10-do-bo-truong-bo-tai-chinh-ban-hanh); [Thông tư 42/2024/TT-BTC (LuatVietnam)](https://luatvietnam.vn/tai-chinh/thong-tu-42-2024-tt-btc-chuan-muc-tham-dinh-gia-viet-nam-ve-tham-dinh-gia-bat-dong-san-355389-d1.html)

## Cụm 2. Định giá bằng dòng tiền

### DCF, FCF, giá trị cuối kỳ (Gordon, exit multiple), chiết khấu dòng tiền về hiện tại

**Thầy nhắc ở:** B2 02:34, B2 02:42, B4 01:28, B7 02:13, B7 02:34, B7 04:02 - "Cách định giá 2", thầy chỉ nói rủi ro giả định xa và cảnh báo giá trị cuối kỳ chiếm 90% giá trị DCF.

**Là gì:** DCF (Discounted Cash Flow, chiết khấu dòng tiền) tính giá trị doanh nghiệp bằng tổng dòng tiền tự do dự báo (FCF) đã chiết khấu về hiện tại, cộng giá trị cuối kỳ (terminal value) đại diện cho mọi dòng tiền sau giai đoạn dự báo. Hai cách tính giá trị cuối kỳ phổ biến: tăng trưởng Gordon và bội số thoát (exit multiple).

**Giải thích:**
- Chiết khấu: giá trị hiện tại = dòng tiền năm t / (1 + r) mũ t, với r là tỷ suất chiết khấu. Với dòng tiền cho toàn bộ nguồn vốn, r là WACC = (E/V) x chi phí vốn chủ + (D/V) x lãi vay x (1 - thuế). Ví dụ: vốn chủ 600, nợ 400, chi phí vốn chủ 14%, lãi vay 9%, thuế 20%: WACC = 0,6 x 14% + 0,4 x 9% x 0,8 = 8,4% + 2,88% = 11,28%.
- Giá trị cuối kỳ Gordon: TV = FCF năm cuối x (1 + g) / (r - g). Bắt buộc r lớn hơn g; g gần r thì giá trị tiến tới vô hạn. g nên không vượt tăng trưởng danh nghĩa dài hạn của nền kinh tế.
- Exit multiple: TV = EBITDA năm cuối x bội số EV/EBITDA kỳ vọng.
- Ví dụ số (r = 10%, g = 3%): FCF ba năm là 100, 110, 120. Giá trị hiện tại: 100/1,1 + 110/1,21 + 120/1,331 = 90,91 + 90,91 + 90,16 = 271,98. TV = 120 x 1,03 / 0,07 = 1.765,7; chiết khấu 3 năm: 1.765,7 / 1,331 = 1.326,6. Giá trị doanh nghiệp = 271,98 + 1.326,6 = 1.598,6. Giá trị cuối kỳ chiếm 83%, gần với cảnh báo 90% của thầy. Nhạy cảm: tăng g lên 4% thì TV = 2.080, giá trị doanh nghiệp 1.834,7 (tăng 14,8%); g = 5% thì 2.165,3 (tăng 35,4%). Nếu dùng exit multiple 8 lần EBITDA 200 thì TV = 1.600, giá trị doanh nghiệp = 271,98 + 1.600/1,331 = 1.474.
- Sai lầm thường gặp: chọn g lớn gần r, dự báo tăng trưởng cao kéo dài quá lâu, dùng r quá thấp, trừ thiếu đầu tư duy trì (capex thấp hơn khấu hao vĩnh viễn), lẫn dòng tiền FCFF với chiết khấu bằng chi phí vốn chủ.
- Giới hạn ở Việt Nam: chi phí vốn khó ước lượng vì beta thị trường nhỏ, thanh khoản không đều và phần bù rủi ro quốc gia thay đổi theo thời điểm (một số bảng Damodaran cho tổng phần bù rủi ro cổ phiếu Việt Nam cao hơn 11% ở dữ liệu đầu năm 2023); các nguồn tôi tìm được không thống nhất, nên cần ghi rõ nguồn và thời điểm khi dùng.

**Liên hệ với bài học:** Thầy đưa DCF như "Cách định giá 2" nhưng nhấn rủi ro của các giả định xa; ví dụ trên cho thấy vì sao: một thay đổi nhỏ của g làm giá trị đổi hàng chục phần trăm. Thầy coi kết quả DCF là một khoảng và cần kết hợp độ nhạy, kịch bản.

**Đọc thêm:** [Discounted cash flow (Wikipedia)](https://en.wikipedia.org/wiki/Discounted%5Fcash%5Fflow); [Gordon growth model (Wikipedia)](https://en.wikipedia.org/wiki/Gordon%5Fgrowth%5Fmodel); [Terminal Value in DCF (Learnsignal)](https://www.learnsignal.com/blog/terminal-value-dcf-methods-formulas-guide/); [Gordon growth model vs. exit multiple (Acadifi)](https://www.acadifi.com/community/terminal-value-gordon-growth-vs-exit-multiple-cfa-level-2); [Country risk 2025 (Damodaran)](https://pages.stern.nyu.edu/~adamodar/pdfiles/blog/CountryRisk2025.pdf); [Vietnam total equity risk premium 11,13% tại 01/01/2023 (GuruFocus)](https://www.gurufocus.com/economic%5Findicators/6042/vietnam-total-equity-risk-premium)

### Dòng tiền tự do và giá trị doanh nghiệp (FCFF, FCFE, EV, DCF)

**Thầy nhắc ở:** B7 01:49, B7 02:09, B7 03:41 - xuất hiện trên bảng, công thức slide và mô-đun báo cáo mẫu.

**Là gì:** FCFF (free cash flow to the firm) là dòng tiền còn lại cho mọi nhà cung cấp vốn (cổ đông và chủ nợ) sau thuế, đầu tư và vốn lưu động. FCFE (free cash flow to equity) là phần dành riêng cho cổ đông. EV (enterprise value, giá trị doanh nghiệp) là giá trị toàn bộ hoạt động kinh doanh, còn giá trị vốn chủ là phần còn lại sau khi trừ các khoản nợ và quyền lợi khác.

**Giải thích:**
- FCFF = EBIT x (1 - thuế) + khấu hao - chi đầu tư (capex) - tăng vốn lưu động. Chiết khấu bằng WACC ra EV.
- FCFE = FCFF - lãi vay x (1 - thuế) + vay ròng. Chiết khấu bằng chi phí vốn chủ ra giá trị vốn chủ trực tiếp.
- Cầu nối từ EV sang vốn chủ: giá trị vốn chủ = EV - nợ vay - cổ phiếu ưu đãi - lợi ích cổ đông thiểu số (và các khoản giống nợ như nghĩa vụ hưu trí) + tiền và tương đương tiền (+ đầu tư vào công ty liên kết nếu chưa tính trong EV).
- Ví dụ số: EBIT 200, thuế 20%, khấu hao 50, capex 80, tăng vốn lưu động 20: FCFF = 160 + 50 - 80 - 20 = 110. Lãi vay 30, vay ròng 20: FCFE = 110 - 30 x 0,8 + 20 = 106. Nếu EV tính ra 1.600 tỷ, nợ 400 tỷ, tiền 100 tỷ (nợ ròng 300 tỷ), lợi ích thiểu số 50 tỷ thì giá trị vốn chủ = 1.600 - 300 - 50 = 1.250 tỷ; với 100 triệu cổ phiếu, giá trị mỗi cổ phiếu là 1.250 tỷ / 100 triệu = 12.500 đồng. Chọn nhất quán: FCFF đi với WACC và trừ nợ, FCFE đi với chi phí vốn chủ và không trừ nợ nữa.
- Giới hạn: FCFE biến động mạnh khi vay ròng đổi, nên với doanh nghiệp đòn bẩy cao dễ cho kết quả sai nếu giả định cơ cấu vốn không ổn định. Ở Việt Nam, nhiều doanh nghiệp có thu nhập từ công ty liên kết hoặc lợi ích thiểu số lớn (ví dụ tập đoàn), nên bước cầu nối dễ bị bỏ sót.

**Liên hệ với bài học:** Thầy nhắc các thuật ngữ này khi đọc mô-đun báo cáo mẫu; hiểu cầu nối EV sang vốn chủ giúp biết vì sao "giá trị doanh nghiệp" khác "giá một cổ phiếu".

**Đọc thêm:** [FCFF vs FCFE (Corporate Finance Institute)](https://corporatefinanceinstitute.com/resources/valuation/fcff-vs-fcfe); [Free cash flow to firm (Wall Street Prep)](https://www.wallstreetprep.com/knowledge/free-cash-flow-to-firm-fcff/); [Enterprise value (Wikipedia)](https://en.wikipedia.org/wiki/Enterprise%5Fvalue)

### Chuẩn hoá lợi nhuận qua chu kỳ (hệ số chu kỳ, P/E chu kỳ hoá)

**Thầy nhắc ở:** B2 02:52 - thầy nói điều chỉnh EPS theo hệ số chu kỳ nhưng không đưa công thức.

**Là gì:** Với doanh nghiệp có lợi nhuận lên xuống mạnh theo chu kỳ ngành (thép, dầu khí, hoá chất), lợi nhuận của một năm không đại diện được. Chuẩn hoá là thay EPS hiện tại bằng một mức EPS "trung bình chu kỳ" trước khi tính P/E hay DCF.

**Giải thích:** Không có công thức duy nhất; thầy không đưa công thức nên đây là các cách thông dụng.
- Trung bình nhiều năm: EPS chuẩn hoá = trung bình EPS qua một chu kỳ đầy đủ (thường 5 đến 10 năm). Hệ số chu kỳ = EPS chuẩn hoá / EPS hiện tại. Ví dụ: EPS đỉnh chu kỳ 5.000 đồng, trung bình 8 năm là 2.000 đồng, hệ số = 0,4; giá 40.000 đồng cho P/E truyền thống 8 lần nhưng P/E chu kỳ hoá là 20 lần, tức không rẻ như vẻ ngoài.
- Biên lợi nhuận chuẩn hoá: doanh thu hiện tại nhân biên lợi nhuận trung bình chu kỳ.
- Shiller CAPE (cyclically adjusted P/E): giá chia trung bình 10 năm lợi nhuận đã điều chỉnh lạm phát, thường dùng cho cả chỉ số. Graham và Dodd đã khuyên làm mượt lợi nhuận 5 đến 10 năm; Campbell và Shiller (1988) phát triển; trung bình CAPE của S&P 500 trong thế kỷ 20 khoảng 15,2. CAPE bị phê bình vì nhìn quá khứ, bỏ qua thay đổi chuẩn kế toán và không xét lãi suất.
- Giới hạn: xác định "chu kỳ đầy đủ" mang tính chủ quan; với thị trường Việt Nam, dữ liệu dài 10 năm có thể lẫn thay đổi cấu trúc ngành.

**Liên hệ với bài học:** Thầy dùng hệ số chu kỳ để tránh mua cổ phiếu chu kỳ lúc P/E thấp ở đỉnh lợi nhuận, ý này trùng với bẫy giá trị (xem mục "Đầu tư theo xu thế" ở phần sau).

**Đọc thêm:** [Cyclically adjusted price-to-earnings ratio (Wikipedia)](https://en.wikipedia.org/wiki/Cyclically%5Fadjusted%5Fprice-to-earnings%5Fratio); [A New Look on Shiller's CAPE Ratio (Quantpedia)](https://quantpedia.com/a-new-look-on-shillers-cape/)

### Định giá quyền chọn thực và mô hình Black-Scholes (real options)

**Thầy nhắc ở:** B7 03:01 - thầy nhắc dùng cho dầu khí và dòng tiền bất ổn.

**Là gì:** Quyền chọn thực (real option) là quyền, không phải nghĩa vụ, hành động kinh doanh như hoãn, mở rộng, thu hẹp hay bỏ dự án. Giá trị của sự linh hoạt đó được định giá bằng kỹ thuật định giá quyền chọn tài chính, tiêu biểu là Black-Scholes.

**Giải thích:** Black-Scholes (Black, Scholes, Merton; Scholes và Merton nhận Nobel Kinh tế 1997) tính giá quyền chọn mua kiểu châu Âu từ giá tài sản S, giá thực hiện K, thời hạn T, lãi suất phi rủi ro r và độ biến động sigma. Công thức: C = S x N(d1) - K x e mũ (-rT) x N(d2), với d1 = [ln(S/K) + (r + sigma bình phương / 2) x T] / (sigma x căn T), d2 = d1 - sigma x căn T. Ví dụ: S = K = 100, r = 5%, sigma = 20%, T = 1 năm: d1 = 0,35; d2 = 0,15; N(d1) = 0,6368; N(d2) = 0,5596; C = 63,68 - 95,12 x 0,5596 = khoảng 10,45. Áp dụng thực: mỏ dầu chưa khai thác giống quyền chọn mua, S là giá trị dòng tiền nếu khai thác, K là chi phí phát triển, sigma là biến động giá dầu. Damodaran dùng cách này cho trữ lượng chưa khai thác. Giới hạn: Black-Scholes giả định biến động hằng số và tài sản có thể nhân bản trong thị trường; với dự án thật điều này thường sai, độ biến động ước tính tuỳ tiện và quyết định kết quả. Vì vậy thực tế thường dùng cây nhị phân hoặc mô phỏng Monte Carlo thay vì công thức đóng. Nếu thị trường ổn định thì NPV truyền thống đủ.

**Liên hệ với bài học:** Thầy chỉ nhắc để nói rằng với dòng tiền bất ổn (dầu khí) có công cụ ngoài DCF, nhưng khá phức tạp để áp dụng đại trà. Hiểu ví dụ trên đủ để không bị rối khi nghe thuật ngữ.

**Đọc thêm:** [Real options valuation (Wikipedia)](https://en.wikipedia.org/wiki/Real%5Foptions%5Fvaluation); [Damodaran, bài giảng quyền chọn thực](https://pages.stern.nyu.edu/~adamodar/pdfiles/valonlineslides/session20.pdf); [Fernández, Valuing real options: frequent errors](https://ucema.edu.ar/u/jd/Inversiones/Articulos/Paper%5FValuing%5FReal%5FOptions%5FFrequent%5Ferrors.pdf); [How options became calculable (Risknet)](https://www.risknet.de/en/topics/news-details/how-options-became-calculable/)

## Cụm 3. Định giá tương đối, lợi thế cạnh tranh và loại cổ phiếu

### Các bội số định giá (P/E, P/S, P/B, EV/EBITDA, tỷ suất cổ tức, earnings yield, PEG, CAGR, P/E tương đối)

**Thầy nhắc ở:** B7 00:15, B7 01:50, B7 03:29, B7 03:32, B7 03:42, B8 00:05, B8 03:09 - thầy xếp nhóm so sánh, PEG bằng P/E chia CAGR 2 năm, báo cáo mẫu có Forward PE, PBV, P/E relative, peer group.

**Là gì:** Bội số định giá là tỷ lệ giữa giá (hoặc giá trị doanh nghiệp) và một chỉ tiêu tài chính, dùng để so sánh doanh nghiệp này với doanh nghiệp khác hoặc với chính nó trong quá khứ. Đây là cách định giá theo cách tiếp cận thị trường.

**Giải thích:** Công thức chuẩn:
- P/E = giá / EPS. EPS cơ bản chia lợi nhuận cho số cổ phiếu hiện có; EPS pha loãng (diluted) tính cả cổ phiếu có thể phát sinh từ trái phiếu chuyển đổi, quyền chọn, nên EPS thấp hơn. Trailing P/E dùng EPS 4 quý gần nhất, forward P/E dùng EPS dự báo. Ví dụ: giá 30.000 đồng, EPS 2.000 đồng thì P/E = 15. Lợi nhuận 200 tỷ, 100 triệu cổ phiếu cho EPS cơ bản 2.000; nếu có thêm 10 triệu cổ phiếu tiềm năng thì EPS pha loãng = 200 tỷ / 110 triệu = 1.818 đồng.
- Earnings yield = EPS / giá, nghịch đảo của P/E: 2.000 / 30.000 = 6,67%. Có thể so thẳng với lãi suất trái phiếu hoặc tiền gửi; Fed model dùng so sánh này nhưng bị tranh cãi.
- P/B = giá / giá trị sổ sách mỗi cổ phiếu (sổ sách 20.000 thì P/B = 1,5), P/S = vốn hoá / doanh thu, tỷ suất cổ tức = cổ tức / giá (1.000 / 30.000 = 3,33%).
- EV/EBITDA = (vốn hoá + nợ vay + cổ phiếu ưu đãi + lợi ích thiểu số - tiền) / EBITDA. EV/EBITDA trung lập với cơ cấu vốn nên so được giữa công ty vay nhiều và vay ít. Ví dụ EV 1.600 và EBITDA 250 cho 6,4 lần.
- CAGR (tốc độ tăng trưởng kép) = (giá trị cuối / giá trị đầu) mũ (1/số năm) - 1. EPS 1.500 lên 2.000 sau 2 năm: (2.000/1.500) mũ 0,5 - 1 = 15,47%.
- PEG = P/E / tốc độ tăng trưởng EPS (viết bằng số phần trăm). Peter Lynch phổ biến chỉ số này trong One Up on Wall Street (1989): PEG dưới 1 có thể rẻ, trên 1 có thể đắt. Với P/E 15 và CAGR 15,47% thì PEG = 0,97. PEG sai khi tăng trưởng âm hoặc rất thấp (kết quả vô nghĩa hoặc âm), khi dự báo tăng trưởng 5 năm của giới phân tích quá lạc quan, và khi so sánh công ty có mức tăng trưởng quá khác nhau. Nguồn khác nhau dùng kỳ hạn tăng trưởng khác nhau (1 năm, 3 đến 5 năm), nên cần ghi rõ cách tính.
- P/E tương đối = P/E của cổ phiếu / P/E của ngành (hoặc thị trường): 15 / 12 = 1,25 nghĩa là đang đắt hơn nhóm 25%. Chọn nhóm so sánh (peer group): cùng mô hình kinh doanh, quy mô, tăng trưởng, rủi ro, đòn bẩy; khi tính trung bình nên loại các ngoại lệ hoặc dùng trung vị. Một bài báo VnEconomy cho thấy loại nhóm Vingroup ra thì mặt bằng P/E của khối phi tài chính thay đổi đáng kể, minh hoạ rằng vài mã lớn có thể làm méo bội số chung.
- Tổng hợp nhiều bội số theo trọng số: giá P/E = 15 x EPS dự phóng 2.200 = 33.000; giá P/B = 1,6 x 20.000 = 32.000; giá EV/EBITDA quy ra 36.000. Trọng số 50%, 25%, 25% cho 0,5 x 33.000 + 0,25 x 32.000 + 0,25 x 36.000 = 33.500 đồng. Trọng số là lựa chọn chủ quan, cần nêu rõ lý do (P/B hợp ngân hàng, EV/EBITDA hợp công ty nặng vốn, P/E hợp công ty lợi nhuận ổn định).
- Giới hạn ở Việt Nam: lợi nhuận bất thường (thoái vốn, đánh giá lại) làm P/E sai lệch; tính thanh khoản và tỷ lệ cổ phiếu tự do chuyển nhượng thấp làm bội số khó so với thị trường phát triển.

**Liên hệ với bài học:** Thầy xếp các doanh nghiệp vào nhóm so sánh rồi dùng bội số của nhóm để suy ra giá; hiểu mẫu số và tử số của từng bội số giúp không so nhầm (ví dụ P/E của ngân hàng và của công ty bán lẻ). Chỉ số PEG của thầy lấy CAGR hai năm, ngắn hơn so với kỳ hạn 3 đến 5 năm thường thấy.

**Đọc thêm:** [PEG ratio (Wikipedia)](https://en.wikipedia.org/wiki/PEG%5Fratio); [Earnings yield (Wikipedia)](https://en.wikipedia.org/wiki/Earnings%5Fyield); [Enterprise value (Wikipedia)](https://en.wikipedia.org/wiki/Enterprise%5Fvalue); [Damodaran, slide về bội số định giá](https://pages.stern.nyu.edu/~adamodar/pdfiles/valonlineslides/session16.pdf); [Damodaran on Valuation, Part II Relative Valuation (O'Reilly)](https://www.oreilly.com/library/view/damodaran-on-valuation/9780471751212/9780471751212%5Frelative%5Fvaluation-017.html); [Loại Vingroup và Gelex, định giá khối phi tài chính (VnEconomy)](https://vneconomy.vn/neu-loai-tru-nhom-vingroup-va-gelex-dinh-gia-nhom-phi-tai-chinh-o-muc-thap-nhat-5-nam.htm)

### Con hào kinh tế và quyền định giá (economic moat, pricing power)

**Thầy nhắc ở:** B7 01:30 - thầy gọi là "khả năng phòng thủ độc đáo", "độc quyền về giá".

**Là gì:** Con hào kinh tế (economic moat) là lợi thế cạnh tranh bền vững giúp doanh nghiệp giữ được lợi nhuận cao trên vốn trong thời gian dài, như hào nước bảo vệ lâu đài. Quyền định giá (pricing power) là khả năng tăng giá mà không mất nhiều khách.

**Giải thích:** Thuật ngữ thường được gán cho Warren Buffett, người dùng chữ "moat" trong thư cổ đông Berkshire Hathaway hơn 20 lần từ 1986 đến 2016 (theo Wikipedia). Morningstar chia nguồn của con hào thành năm loại:
- Tài sản vô hình: thương hiệu, bằng sáng chế, giấy phép nhà nước.
- Chi phí chuyển đổi: khách hàng ở lại vì đổi sang đối thủ tốn tiền hoặc công sức.
- Hiệu ứng mạng: giá trị tăng khi có thêm người dùng.
- Lợi thế chi phí: chi phí thấp hơn đối thủ, thường nhờ quy mô.
- Quy mô hiệu quả: thị trường nhỏ chỉ đủ chỗ cho vài đối thủ (điện, nước, đường ống).
Dấu hiệu thực nghiệm của con hào: tỷ suất lợi nhuận trên vốn đầu tư (ROIC) cao hơn chi phí vốn trong nhiều năm; ví dụ ROIC 18% so với WACC 10% cho chênh lệch 8 điểm phần trăm và nếu chênh lệch giữ được thì doanh nghiệp xứng đáng bội số cao hơn. Quyền định giá thể hiện ở biên lợi nhuận gộp ổn định khi chi phí đầu vào tăng. Hạn chế: con hào có thể bị xói mòn bởi công nghệ hoặc thay đổi quy định; Wikipedia ghi nhận chỉ trích rằng đặt niềm tin quá lớn vào con hào có rủi ro (bài Sunday Times, 2011). Không phải mọi doanh nghiệp được thị trường định giá cao đều có con hào.

**Liên hệ với bài học:** Thầy coi con hào là một lý do để chấp nhận bội số cao hoặc giả định tăng trưởng bền; phần định tính này khó đưa vào công thức DCF nhưng quyết định độ tin cậy của giả định g.

**Đọc thêm:** [Economic moat (Wikipedia)](https://en.wikipedia.org/wiki/Economic%5Fmoat); [What is an economic moat? (Morningstar)](https://morningstar.co.uk/uk/news/120912/what-is-an-economic-moat.aspx); [How to measure a company's competitive advantage (Morningstar)](https://www.morningstar.com/stocks/how-measure-companys-competitive-advantage)

### Cổ phiếu phòng thủ, cổ phiếu tăng trưởng và chu kỳ ngành

**Thầy nhắc ở:** B6 03:15, B8 00:59 - học viên xếp điện, nước, y tế là phòng thủ.

**Là gì:** Cổ phiếu phòng thủ (defensive) thuộc ngành nhu cầu ít co giãn theo kinh tế (điện, nước, thực phẩm thiết yếu, y tế), thường ít biến động hơn thị trường. Cổ phiếu chu kỳ (cyclical) lên xuống theo chu kỳ kinh tế (thép, bất động sản, ô tô). Cổ phiếu tăng trưởng (growth) là cổ phiếu kỳ vọng tăng nhanh hơn trung bình, thường P/E cao.

**Giải thích:** Theo Britannica, cổ phiếu chu kỳ thường tốt khi kinh tế mở rộng và kém khi suy thoái; cổ phiếu tăng trưởng có thể nằm trong cả nhóm chu kỳ lẫn phòng thủ. Các nguồn lưu ý y tế và hàng tiêu dùng thiết yếu không phải lúc nào cũng phòng thủ (ví dụ thay đổi quy định giá thuốc làm yếu độ phòng thủ của ngành dược). Phòng thủ nghĩa là rủi ro giảm sâu thấp hơn chứ không phải không lỗ, và thường tăng chậm. Theo hiểu biết chung (không có nguồn riêng trong kết quả tìm kiếm), với điện và nước ở Việt Nam, giá bán do cơ quan nhà nước quản lý và điện thuỷ điện còn phụ thuộc thời tiết, nên độ phòng thủ có điều kiện riêng.

**Liên hệ với bài học:** Phân loại này giúp đọc khi thầy nói về chọn ngành theo pha chu kỳ: pha suy thoái nghiêng phòng thủ, pha hồi phục nghiêng chu kỳ. Khác biệt với cách học viên xếp: nhãn "phòng thủ" nên được kiểm bằng dữ liệu biến động và lợi nhuận của chính mã đó.

**Đọc thêm:** [Cyclical stocks and defensive investing (Britannica Money)](https://www.britannica.com/money/cyclical-stocks-defensive-investing); [Defensive versus cyclical stocks (AAII)](https://www.aaii.com/journal/article/14780-defensive-versus-cyclical-stocks)

## Cụm 4. Định giá đặc thù, theo phần và theo kịch bản

### Định giá theo tổng các phần (SOTP), theo tài sản, phân tích độ nhạy và kịch bản; nguyên tắc "chia để trị"

**Thầy nhắc ở:** B2 02:53, B5 02:26, B5 02:30, B7 02:53, B7 02:56 - thầy dùng nhưng không gọi tên, ví dụ nhạy lợi nhuận theo giá dầu; thầy dẫn "chia để trị" từ tin học và ví dụ Kinh Đô tách mảng.

**Là gì:** SOTP (sum of the parts) định giá từng mảng kinh doanh riêng rồi cộng lại, trừ nợ cấp tập đoàn để ra giá trị vốn chủ. Định giá theo tài sản đánh giá lại tài sản và trừ nợ (NAV, RNAV). Phân tích độ nhạy thay đổi một biến để xem kết quả đổi bao nhiêu; phân tích kịch bản thay đổi nhiều biến cùng lúc theo từng câu chuyện.

**Giải thích:**
- Các bước SOTP: (1) tách doanh nghiệp thành các mảng; (2) chọn phương pháp riêng cho mỗi mảng (bội số của đối thủ cùng ngành, DCF, giá thị trường nếu là công ty niêm yết); (3) cộng giá trị; (4) trừ nợ ròng và chi phí cấp công ty mẹ; (5) trừ lợi ích cổ đông thiểu số; (6) áp chiết khấu tập đoàn nếu có. Ví dụ: mảng A EBITDA 100 x 8 = 800; mảng B 50 x 12 = 600; cổ phần 30% trong công ty niêm yết vốn hoá 2.000 là 600, chiết khấu thanh khoản 20% còn 480. Tổng = 1.880. Trừ nợ cấp holding 500 còn 1.380; chiết khấu holding 15% còn 1.173.
- Rủi ro: cộng trùng (ví dụ cộng cả mảng được hợp nhất lẫn phần sở hữu trong mảng đó; hoặc doanh thu nội bộ giữa các mảng), quên trừ nợ ở cấp mẹ, dùng bội số của đối thủ không tương thích, và giả định thị trường sẽ "mở khoá" giá trị. Wikipedia nêu chiết khấu tập đoàn (conglomerate discount) ở nền kinh tế phát triển có thể 13 đến 15% so với đối thủ đơn ngành, thường lớn hơn ở Mỹ và Tây Âu so với châu Á; tách mảng là cách có thể thu hẹp chiết khấu.
- Kinh Đô: theo Báo Đầu tư và Brands Vietnam, cuối năm 2014 Kinh Đô bán 80% mảng bánh kẹo cho Mondelez International, giá khoảng 370 triệu USD (gần 8.000 tỷ đồng); đại hội cổ đông tháng 6/2014 thông qua chuyển mảng cho Công ty Kinh Đô Bình Dương, bàn giao cho Mondelez từ 30/6/2015; giữa 2016 bán nốt 20%. KIDO chuyển sang dầu ăn, mì, kem; cam kết không làm bánh kẹo hết hạn tháng 7/2020 và năm 2020 quay lại với thương hiệu Kingdom. Ví dụ này minh hoạ "chia để trị": tách một mảng có thể làm lộ giá trị từng phần.
- Độ nhạy: giả định mỏ dầu sản xuất 1 triệu thùng/năm, chi phí 40 USD/thùng. Lợi nhuận trước thuế ở giá 60 USD là 20 triệu USD; giá 70 USD cho 30 triệu USD (tăng 50%); giá 50 USD cho 10 triệu USD (giảm 50%). Giá dầu đổi 17% làm lợi nhuận đổi 50% vì đòn bẩy hoạt động. Kịch bản: kết hợp giá dầu, sản lượng, tỷ giá cùng lúc (xem mục "Kịch bản A/B/C").
- Chiết khấu thanh khoản: cổ phần trong công ty có thanh khoản thấp hoặc cổ phần kiểm soát không bán được ngay nên giá trị ghi nhận thấp hơn giá thị trường niêm yết.

**Liên hệ với bài học:** Thầy dùng đúng các kỹ thuật này mà không gọi tên; đọc mục này để nhận ra khi thầy cộng từng mảng hay chạy lợi nhuận theo giá dầu. Khác với cách dùng phổ thông: "chia để trị" trong tin học là chia bài toán thành bài toán nhỏ, còn ở định giá nó có thêm vấn đề cộng trùng.

**Đọc thêm:** [Sum-of-the-parts analysis (Wikipedia)](https://en.wikipedia.org/wiki/Sum-of-the-parts%5Fanalysis); [Conglomerate discount (Wikipedia)](https://en.wikipedia.org/wiki/Conglomerate%5Fdiscount); [Kinh Đô hậu M&A (Brands Vietnam)](https://www.brandsvietnam.com/6700-kinh-do-hau-m-amp-a); [Kinh Đô hậu M&A ra sao (Báo Đầu tư)](https://baodautu.vn/kinh-do-hau-ma-ra-sao-d25982.html); [KDC sắp hoàn tất chuyển giao mảng bánh kẹo cho Mondelez (Báo Đầu tư)](https://baodautu.vn/kdc-sap-hoan-tat-chuyen-giao-mang-banh-keo-cho-mondelz-international-d29600.html)

### Định giá tập đoàn đa ngành nợ cao (ví dụ Masan) và NAV (net asset value)

**Thầy nhắc ở:** B13 02:25, B18 02:28, B18 02:37 - thầy chê bài định giá áp máy móc cho MSN, nhãn NAV trên sơ đồ IPO.

**Là gì:** Tập đoàn đa ngành (holding) sở hữu nhiều công ty con ở nhiều lĩnh vực và thường vay nợ ở cấp công ty mẹ. NAV (net asset value) là giá trị thị trường của tài sản trừ nợ phải trả, chia cho số cổ phiếu hoặc đơn vị.

**Giải thích:** Với holding như Masan Group (MSN), áp P/E hay EV/EBITDA hợp nhất một con số dễ sai vì các mảng có tăng trưởng, rủi ro và thanh khoản khác nhau, và lợi nhuận hợp nhất khác với dòng tiền thực sự về mẹ. Các công ty chứng khoán thường định giá MSN theo SOTP, tách riêng Masan Consumer, WinCommerce, Masan MEATLife, Masan High-Tech Materials, Techcombank và Phúc Long Heritage (báo cáo KB Securities, Shinhan, SSI giai đoạn 2025 đến 2026, sau thời điểm khoá học). Cần trừ nợ cấp mẹ, lợi ích cổ đông thiểu số và nghĩa vụ liên quan đến quyền chọn bán (put option) nếu có. Giá mục tiêu các nơi lệch nhau nhiều: KB Securities 98.800 đồng, Shinhan 105.300 đồng (giá 73.000 đồng ngày 11/03/2026), SSI 81.600 đồng, theo các báo cáo này; CEO Masan nói cổ phiếu đang thấp hơn giá trị nội tại khoảng 60% (nguồn từ phía công ty, cần kiểm chứng). NAV theo kiểu RNAV: đánh giá lại tài sản theo giá thị trường; công ty địa ốc ở Singapore và Malaysia thường được môi giới áp chiết khấu 20 đến 60% trên RNAV (ví dụ CIMB 50% cho Sime Darby Property theo bài báo The Star), vì thanh khoản thấp, cấu trúc holding và nghi ngờ về việc mở khoá giá trị. Ví dụ NAV: tài sản đánh giá lại 1.500 tỷ, nợ 600 tỷ thì NAV = 900 tỷ; 100 triệu cổ phiếu cho NAV 9.000 đồng; áp chiết khấu 30% thì giá mục tiêu 6.300 đồng.

**Liên hệ với bài học:** Thầy chê bài định giá dùng công thức máy móc cho MSN vì bỏ qua cấu trúc holding và nợ; nhãn NAV trên sơ đồ IPO của thầy có nghĩa là giá trị tài sản ròng, không phải giá thị trường.

**Đọc thêm:** [KBSV, báo cáo MSN 3Q25](https://www.kbsec.com.vn/pic/Service/KBSV%5FMSN%5F3Q25Update%5FEng.pdf); [Masan shares undervalued by 60%: CEO (The Investor)](https://theinvestor.vn/masan-shares-undervalued-by-60-ceo-d18934.html); [Sime Darby Property valued at RM1.85 at CIMB Research (The Star)](https://www.thestar.com.my/business/business-news/2018/03/19/sime-darby-property-valued-at-rm1pt85-at-cimb-research); [How to use NAV and RNAV (bài tổng hợp)](https://forex.in.rs/rnav-revalued-net-asset-value)

### Định giá trong M&A, quỹ tương hỗ, quỹ hưu trí, ngân hàng, bảo hiểm

**Thầy nhắc ở:** B7 01:42, B7 02:08 - thầy nói thuộc môn khác hoặc nhắc khi phân loại loại hình doanh nghiệp.

**Là gì:** Mỗi loại hình có đặc thù riêng nên không dùng được chung một mô hình.

**Giải thích:**
- M&A: người mua thường trả phần bù kiểm soát (control premium) = giá chào / giá chưa bị ảnh hưởng bởi tin thâu tóm - 1; điều kiện hợp lý là giá trị hiện tại của giá trị cộng hưởng (synergy) lớn hơn phần bù. Nghiên cứu BCG trên 167 công ty cho thấy phần bù trung bình 34%. Ví dụ: giá chưa ảnh hưởng 100, giá chào 130 nên phần bù 30%; nếu giá trị hiện tại của cộng hưởng là 45 mỗi cổ phiếu thì người mua còn lại 15.
- Quỹ tương hỗ: giá trị tài sản ròng một chứng chỉ quỹ = (tổng tài sản - nợ phải trả) / số chứng chỉ quỹ; quỹ đóng giao dịch dưới hoặc trên NAV. Quỹ hưu trí quan tâm tình trạng tài trợ: tài sản so với giá trị hiện tại của nghĩa vụ trả lương hưu.
- Ngân hàng: nợ là nguyên liệu nên không dùng EV; thường dùng P/B và ROE. P/B hợp lý = (ROE - g) / (r - g); ví dụ ROE 18%, g 8%, r 14% thì (0,18 - 0,08) / (0,14 - 0,08) = 1,67. Đây là công thức tiêu chuẩn của lý thuyết định giá, chưa tìm thấy nguồn cụ thể trong lượt tra cứu này.
- Bảo hiểm: thường dùng giá trị nội tại hiện hữu (embedded value) và bội số P/EV; kiến thức chung, chưa tra nguồn riêng.

**Liên hệ với bài học:** Thầy nói đây thuộc môn khác nên không giảng; chỉ cần nhớ rằng công thức DCF và EV/EBITDA ở các mục trước không áp được máy móc cho ngân hàng và bảo hiểm.

**Đọc thêm:** [Control premium (Wall Street Prep)](https://www.wallstreetprep.com/knowledge/control-premium/); [Takeover premium (Corporate Finance Institute)](https://corporatefinanceinstitute.com/resources/knowledge/deals/takeover-premium); [Real deal: M&A synergies (BCG)](https://www.bcg.com/en-gb/publications/2016/merger-acquisitions-corporate-finance-real-deal-m-a-synergies-value)

### Kịch bản A/B/C, mô hình định giá trên Excel và dashboard theo dõi đầu tư

**Thầy nhắc ở:** B13 02:00, B13 03:55, B13 03:58 - thầy khuyên học Excel và lập kịch bản nhiều nhánh.

**Là gì:** Phân tích kịch bản lập vài (thường ba) bức tranh khả dĩ kết hợp nhiều biến, mỗi bức tranh có xác suất và giá trị riêng. Dashboard là bảng tổng hợp các chỉ tiêu theo dõi danh mục.

**Giải thích:** Theo mô tả của Wikipedia, phân tích kịch bản khác dự báo (không ngoại suy quá khứ), thường dùng khoảng ba kịch bản, và khác phân tích độ nhạy ở chỗ thay đổi nhiều yếu tố cùng nhau. Quy trình gợi ý: xác định các động lực chính, gom thành khung, tạo vài kịch bản nhỏ rồi rút còn 2 đến 3, mô tả từng kịch bản. Hạn chế: chủ quan, và gán xác suất dễ làm người ta chỉ tập trung vào kịch bản có xác suất cao nhất. Ví dụ định giá: kịch bản A (xấu) 80.000 đồng xác suất 25%, B (cơ sở) 110.000 đồng xác suất 50%, C (tốt) 140.000 đồng xác suất 25%: giá trị kỳ vọng = 0,25 x 80 + 0,5 x 110 + 0,25 x 140 = 110 nghìn đồng. So với giá thị trường 90.000 thì biên an toàn theo kịch bản cơ sở là (110 - 90)/110 = 18%. Trong Excel, công cụ Data Table (What-if analysis) cho phép quét một hoặc hai biến để tạo bảng độ nhạy. Các chỉ tiêu dashboard theo gợi ý chung (không có nguồn riêng): giá vốn bình quân, lãi lỗ chưa thực hiện theo phần trăm, tỷ trọng từng mã, giá trị nội tại so với giá, mức cắt lỗ, tỷ trọng tiền mặt, hiệu suất so với VN-Index.

**Liên hệ với bài học:** Thầy khuyên lập kịch bản để thay câu hỏi "giá sẽ lên hay xuống" bằng "nếu A thì làm gì, nếu C thì làm gì"; Excel là công cụ để làm việc đó mà không phụ thuộc phần mềm đóng gói.

**Đọc thêm:** [Scenario analysis (Wikipedia)](https://en.wikipedia.org/wiki/Scenario%5Fanalysis)

## Cụm 5. Thị trường hiệu quả, danh mục và bài học thất bại

### Giả thuyết thị trường hiệu quả và bước đi ngẫu nhiên (EMH, random walk)

**Thầy nhắc ở:** B10 01:58 - thầy chê nền tảng coi giá là ngẫu nhiên, nhắc cả nghiên cứu đoạt Nobel.

**Là gì:** Giả thuyết thị trường hiệu quả (efficient market hypothesis) cho rằng giá chứng khoán đã phản ánh thông tin sẵn có, nên không thể liên tục thắng thị trường bằng cách dùng thông tin đó. Bước đi ngẫu nhiên (random walk) là mô tả thống kê đi kèm: thay đổi giá ngày mai không dự đoán được từ lịch sử giá.

**Giải thích:** Ý tưởng có từ luận án của Louis Bachelier năm 1900; Paul Samuelson (1965) và Benoit Mandelbrot (1963) cũng chỉ ra lợi suất tài chính khó dự đoán. Eugene Fama đưa ra khung hiện đại trong bài tổng quan năm 1970 với ba dạng, phân theo loại thông tin: dạng yếu (lịch sử giá), dạng bán mạnh (mọi thông tin công khai), dạng mạnh (cả thông tin nội bộ). Ví dụ số: giá đang 100 vì thị trường tin giá trị là 100; công ty công bố tin tốt nâng giá trị lên 110. Nếu thị trường hiệu quả, giá nhảy ngay lên 110 và sau đó chỉ dao động ngẫu nhiên, nên người mua sau tin không có lợi thế. Nếu giá lên chậm từ 100 đến 110 trong nhiều tuần thì có thể "đi theo xu thế" để kiếm lời, tức là dạng yếu bị vi phạm. Burton Malkiel (A Random Walk Down Wall Street, 1973) cho rằng bằng chứng thống kê nhìn chung ủng hộ giả thuyết.
Phê bình chính: (1) tài chính hành vi (Kahneman, Tversky, Thaler) cho rằng quá tự tin và phản ứng thái quá làm giá lệch; (2) các dị thường như hiệu ứng cổ phiếu nhỏ, cổ phiếu giá trị, động lượng (momentum) mà mô hình rủi ro chuẩn không giải thích hết, dẫn tới mô hình đa nhân tố của Fama và French; (3) vấn đề giả thuyết kép: muốn kiểm định hiệu quả phải có mô hình lợi suất kỳ vọng, nên kết quả bất thường có thể do mô hình sai chứ chưa chắc thị trường kém hiệu quả; (4) bong bóng, như cơn sốt đường sắt Anh thập niên 1840. Sau khủng hoảng 2008, Jeremy Grantham và Paul Volcker đổ lỗi một phần cho niềm tin vào thị trường hiệu quả, còn Fama cho rằng khủng hoảng vẫn phù hợp với thị trường hiệu quả. Theo hiểu biết chung (không có trong trang tôi mở): Fama nhận Nobel Kinh tế 2013, chia với Robert Shiller và Lars Peter Hansen; Shiller là người phê bình mạnh giả thuyết này nên giải Nobel năm đó trao cho cả hai phía. Nghịch lý Grossman-Stiglitz (1980): nếu giá đã phản ánh hết thông tin thì không ai có động cơ bỏ tiền thu thập thông tin, nên thị trường không thể hiệu quả hoàn hảo.
Giới hạn ở Việt Nam: tôi chưa tìm được nghiên cứu đáng tin về mức hiệu quả dạng yếu của thị trường chứng khoán Việt Nam; hãy tìm với từ khoá "weak-form efficiency Vietnam stock market".

**Liên hệ với bài học:** Thầy bác nền tảng "giá là ngẫu nhiên" để dựng các phương pháp dự báo từ giá và xu thế (xem mục xu thế và mục ARIMA, GARCH). Hiểu EMH giúp phân biệt: phê bình của thầy nhắm vào dạng yếu; ngay cả giới học thuật cũng không coi đó là kết luận cuối cùng.

**Đọc thêm:** [Efficient-market hypothesis (Wikipedia)](https://en.wikipedia.org/wiki/Efficient-market%5Fhypothesis); [Financial market efficiency (Wikipedia)](https://Www.wikipedia.org/wiki/Financial%5Fmarket%5Fefficiency); [Fama 1970, Efficient Capital Markets (bản PDF)](https://datagolf.com/static/blogs/fl%5Fbias/fama%5F1970.pdf); [Efficient Market Hypothesis (FE Training)](https://fe.training/free-resources/portfolio-management/efficient-market-hypothesis)

### Beta, alpha, CAPM và mô hình thị trường (market model)

**Thầy nhắc ở:** B10 01:44, B10 01:47, B10 01:51 - thầy giảng beta là hệ số góc, nhắc săn alpha, nói phương sai là độ phân tán quanh đường hồi quy.

**Là gì:** CAPM (capital asset pricing model) nói lợi suất kỳ vọng của một tài sản bằng lãi suất phi rủi ro cộng beta nhân phần bù rủi ro thị trường. Beta đo độ nhạy của tài sản với biến động thị trường. Alpha (Jensen) là phần lợi suất vượt mức CAPM dự đoán.

**Giải thích:**
- CAPM: lợi suất kỳ vọng = Rf + beta x (E(Rm) - Rf). Beta = hiệp phương sai (lợi suất cổ phiếu, lợi suất thị trường) / phương sai lợi suất thị trường; cũng bằng hệ số tương quan x độ lệch chuẩn cổ phiếu / độ lệch chuẩn thị trường. CAPM do Treynor (1961-62), Sharpe (1964), Lintner (1965), Mossin (1966) phát triển; Sharpe nhận Nobel 1990.
- Mô hình thị trường (dạng hồi quy theo thời gian): (R cổ phiếu - Rf) = alpha + beta x (R thị trường - Rf) + sai số. Beta là hệ số góc, alpha là hệ số chặn, đúng như thầy vẽ trên đường hồi quy. R bình phương là tỷ lệ phương sai của cổ phiếu giải thích được bởi thị trường; phần còn lại là rủi ro riêng (phương sai phần dư).
- Ví dụ số: Rf 3%, thị trường kỳ vọng 10%, beta 1,2: lợi suất kỳ vọng = 3% + 1,2 x 7% = 11,4%. Nếu thực tế cổ phiếu đạt 13% thì alpha = 13% - 11,4% = 1,6%. Tính beta: hiệp phương sai 0,0036 và phương sai thị trường 0,0030 cho beta 1,2. Nếu phương sai cổ phiếu là 0,0072 thì R bình phương = 1,44 x 0,0030 / 0,0072 = 0,6, tức 60% độ biến động đến từ thị trường và phương sai phần dư = 0,4 x 0,0072 = 0,00288.
- Quy ước 252 phiên một năm là số ngày giao dịch trung bình ở Mỹ dùng để đổi độ lệch chuẩn ngày sang năm: nhân với căn bậc hai của 252 (khoảng 15,87). Độ lệch chuẩn ngày 1,5% tương ứng khoảng 23,8% một năm. Số phiên thực tế ở từng thị trường có thể khác chút ít.
- Giới hạn: CAPM giả định nhà đầu tư hợp lý, vay cho vay không giới hạn ở lãi suất phi rủi ro, không phí và thuế. Thực nghiệm cho thấy cổ phiếu beta thấp thường sinh lời cao hơn CAPM dự đoán; kích thước và giá trị giải thích thêm lợi suất (dẫn tới mô hình Fama-French); beta không hằng số theo thời gian; phê bình của Roll cho rằng danh mục thị trường thật không quan sát được nên mọi chỉ số chỉ là xấp xỉ. Alpha chỉ có nghĩa khi mô hình và chỉ số chuẩn được chọn đúng. Ở Việt Nam, tôi chưa tìm được nguồn riêng; theo lẽ thường, beta so với VN-Index chịu ảnh hưởng của thanh khoản mỏng và chỉ số có vài mã vốn hoá lớn chiếm tỷ trọng cao, nên cần thận trọng.

**Liên hệ với bài học:** Thầy dùng hồi quy lợi suất cổ phiếu trên lợi suất thị trường để lấy beta và tìm alpha. Hiểu mô hình thị trường giúp đọc đúng các bảng hồi quy ở các buổi sau: hệ số góc là beta, hệ số chặn là alpha, R bình phương là mức thị trường giải thích.

**Đọc thêm:** [Capital asset pricing model (Wikipedia)](https://en.wikipedia.org/wiki/Capital%5Fasset%5Fpricing%5Fmodel); [Alpha (finance) (Wikipedia)](https://Www.wikipedia.org/wiki/Excess%5Freturn); [Jensen's measure (Wall Street Prep)](https://wallstreetprep.com/knowledge/jensens-measure-alpha); [CAPM lecture notes (ECU)](https://core.ecu.edu/rothmanp/ec3343%5Fcapm.pdf)

### Đầu tư theo chỉ số (index investing)

**Thầy nhắc ở:** B12 00:35 - thầy chê là phương pháp kém.

**Là gì:** Đầu tư theo chỉ số là mua quỹ (quỹ mở hoặc ETF) cố gắng sao chép một chỉ số như S&P 500 hay VN30, thay vì chọn từng cổ phiếu. Đây là đầu tư thụ động.

**Giải thích:** Theo Wikipedia: Qualidex (1970) là quỹ chỉ số mở đầu tiên cho nhà đầu tư cá nhân; năm 1973 Burton Malkiel ủng hộ quỹ rẻ mua cả thị trường; John Bogle lập Vanguard năm 1974 và ra quỹ chỉ số S&P 500 ngày 31/12/1975, bị giễu là "Bogle's folly". Ưu điểm: phí thấp, đơn giản, ít giao dịch, không lệch phong cách. Nhược điểm: sai lệch bám chỉ số (tracking error), việc cơ cấu lại rổ chỉ số bị người khác đón đầu, tập trung vào vài mã lớn, và quỹ tập trung sở hữu ở vài công ty quản lý lớn. Lập luận chính của phe ủng hộ là số liệu SPIVA của S&P: trong 15 năm đến tháng 12/2024, không nhóm quỹ chủ động nào ở Mỹ có đa số quỹ thắng chỉ số chuẩn; quỹ cổ phiếu vốn hoá lớn thua S&P 500 trên 90% (các nguồn lệch nhau chút ít, ví dụ 92,2% tại một số kỳ). Ví dụ số: giả sử thị trường sinh lời 10% mỗi năm. Quỹ chỉ số thu phí 0,65% (mức phí của E1VFVN30 theo báo cáo của DCVFM) còn 9,35%: 100 tăng thành khoảng 598 sau 20 năm. Quỹ chủ động thu phí 2% và chỉ thắng gộp thị trường bằng 0 thì còn 8%: 100 thành khoảng 466. Phê bình của phía thầy (và các nhà đầu tư chủ động): chỉ số có cổ phiếu kém, và nếu ai cũng thụ động thì không còn ai định giá.
Giới hạn ở Việt Nam: tôi không tìm được số liệu SPIVA tương đương cho thị trường Việt Nam, và không có bảng so sánh trực tiếp E1VFVN30 với các quỹ chủ động cùng kỳ; nên đối chiếu NAV từng năm trong báo cáo của công ty quản lý quỹ.

**Liên hệ với bài học:** Thầy xếp đầu tư theo chỉ số vào nhóm "phương pháp kém" vì lợi suất chỉ bằng thị trường, trong khi mục tiêu khoá học là vượt thị trường. Cần hiểu lập luận của phe chỉ số (số liệu SPIVA ở Mỹ) để đánh giá câu hỏi này một cách cân bằng.

**Đọc thêm:** [Index fund (Wikipedia)](https://en.wikipedia.org/wiki/Index%5Ffund); [SPIVA US Year-End 2024 (S&P Dow Jones Indices)](https://spglobal.com/spdji/en/spiva/article/spiva-us-year-end-2024); [Active Stock Funds Largely Lose to Index Funds (ETF.com)](https://www.etf.com/sections/news/active-stock-funds-largely-lose-index-funds-spiva); [VFMVN30 ETF (Investing.com)](https://vn.investing.com/etfs/vfmvn30)

### LTCM và sách "Khi các thiên tài thất bại" (Roger Lowenstein)

**Thầy nhắc ở:** B2 02:27 - dẫn chứng thất bại của mô hình.

**Là gì:** Long-Term Capital Management (LTCM) là quỹ phòng hộ (hedge fund) ở Greenwich, Connecticut, do John Meriwether lập, với hai người đoạt Nobel Robert Merton và Myron Scholes trong hội đồng. Quỹ sụp đổ năm 1998 và bị các ngân hàng cứu dưới sự điều phối của Cục Dự trữ Liên bang New York. When Genius Failed (Roger Lowenstein, 2000) kể lại câu chuyện này.

**Giải thích:** Diễn biến theo Wikipedia: quỹ lập năm 1994 (cuốn sách ghi 1993); lợi suất sau phí khoảng 21%, 43%, 41% trong ba năm đầu. Đầu 1998 vốn chủ khoảng 4,7 tỷ USD, vay hơn 124,5 tỷ USD (đòn bẩy trên 25 lần), vị thế phái sinh danh nghĩa khoảng 1.250 tỷ USD. Nga vỡ nợ ngày 17/08/1998; đến cuối tháng 8 quỹ mất 1,85 tỷ USD; ba tuần đầu tháng 9 vốn chủ từ 2,3 tỷ còn khoảng 400 triệu USD (đến 25/09). Ngày 23/09/1998, 14 định chế (Goldman Sachs, Merrill Lynch, J.P. Morgan và các ngân hàng khác) đồng ý bơm khoảng 3,6 tỷ USD để đổi lấy 90% quỹ; không có tiền công. Quỹ bị thanh lý đầu năm 2000. Ví dụ số: vốn 4,7 tỷ trên tổng tài sản khoảng 129,2 tỷ (4,7 + 124,5), nghĩa là chỉ cần tài sản mất khoảng 3,6% giá trị là hết sạch vốn chủ. Mô hình của quỹ giả định chênh lệch giá giữa các trái phiếu tương tự sẽ hội tụ; khi hoảng loạn, các chênh lệch tách xa hơn, đòn bẩy lớn làm lỗ khuếch đại, và thanh khoản biến mất khi cần bán. Merrill Lynch sau đó cảnh báo trong báo cáo thường niên rằng các mô hình rủi ro có thể tạo cảm giác an toàn hơn thực tế. Về cuốn sách: BusinessWeek xếp vào nhóm sách kinh doanh hay nhất năm 2000; chỉ có Publishers Weekly nhận xét tác giả dùng nhiều số liệu và văn phong nặng. Chưa tìm được nguồn đáng tin về các tranh luận chi tiết xoay quanh vai trò riêng của Merton và Scholes trong việc thiết kế chiến lược (hai ông ở hội đồng, không tìm thấy nguồn mô tả cụ thể phần việc); từ khoá gợi ý: "Merton Scholes role LTCM trading strategy".

**Liên hệ với bài học:** Thầy dùng LTCM làm ví dụ rằng mô hình do người giỏi lập vẫn thất bại khi giả định không còn đúng và khi đòn bẩy quá cao. Bài học liên quan đến các mục Backtest và Martingale: mô hình đẹp trên dữ liệu quá khứ chưa chắc sống sót khi điều kiện đổi.

**Đọc thêm:** [Long-Term Capital Management (Wikipedia)](https://en.wikipedia.org/wiki/Long-Term%5FCapital%5FManagement); [When Genius Failed (Wikipedia)](https://en.wikipedia.org/wiki/When%5FGenius%5FFailed); [Hedge funds and the collapse of LTCM (CFA Institute)](https://rpc.cfainstitute.org/research/cfa-digest/2000/02/hedge-funds-and-the-collapse-of-long-term-capital-management-digest-summary); [Too big to fail? LTCM and the Federal Reserve (Cato Institute)](https://www.cato.org/publications/briefing-paper/too-big-fail-longterm-capital-management-federal-reserve)

## Cụm 6. Chiến lược đầu tư và quản trị vị thế

### Đầu tư theo xu thế, "xu thế là bạn" và tranh luận với đầu tư giá trị

**Thầy nhắc ở:** B10 01:17, B10 01:18, B10 01:22 - thầy nêu trend following là chiến lược hiệu quả nhất và bác mạnh trường phái giá trị.

**Là gì:** Đầu tư theo xu thế (trend following) là mua khi giá đang tăng và bán hoặc bán khống khi giá đang giảm, kỳ vọng xu thế tiếp diễn, không cố dự đoán mức giá hay định giá doanh nghiệp. Đầu tư giá trị (value investing) là mua khi giá thấp hơn giá trị nội tại ước tính.

**Giải thích:** Theo Wikipedia, câu "xu thế là bạn" (the trend is your friend) là châm ngôn của giới giao dịch, gần với "đừng đi ngược dòng thị trường" (don't fight the tape); tôi chưa tìm được người đầu tiên nói câu này. Nguyên tắc điển hình: vào lệnh theo tín hiệu cố định (ví dụ đường trung bình 50 và 100 phiên cắt nhau), đặt mức cắt lỗ dựa trên biên độ giá, cắt lỗ nhanh, để lãi chạy, rủi ro mỗi lệnh thường 1 đến 5% vốn, và đa dạng hoá nhiều thị trường. Ví dụ số: vào ở 120; thoát khi giá giảm 10% từ đỉnh. Nếu giá lên đỉnh 180 thì thoát ở 162, lãi 35%; nếu đột phá giả và giá rơi, thoát ở 108, lỗ 10%. Thắng 1 trong 3 lệnh vẫn có lãi: +35% - 10% - 10% = +15%.
Bằng chứng: bài "A Century of Evidence on Trend-Following Investing" của Hurst, Ooi và Pedersen (AQR) dựng chiến lược động lượng chuỗi thời gian từ năm 1880 và báo cáo sinh lời ổn định hơn một thế kỷ, tương quan thấp với cổ phiếu và trái phiếu, mạnh nhất trong những năm thị trường cổ phiếu biến động cực đoan; kết quả sau 2008 yếu nhưng tác giả không thấy bất thường so với lịch sử. Lưu ý đó là kết quả giả lập chứ không phải tiền thật, và nghiên cứu do một hãng quản lý quỹ thực hiện. Wikipedia ghi thêm: hàng hoá có xu thế rõ hơn cổ phiếu (cổ phiếu hay quay về trung bình), và phần lớn lệnh có thể thua mà chiến lược vẫn lãi.
Phía giá trị: Graham, Buffett cho rằng giá ngắn hạn là tiếng ồn, cần mua rẻ so với giá trị với biên an toàn. Bẫy giá trị (value trap) là cổ phiếu trông rẻ theo P/E hay P/B nhưng rẻ vì doanh nghiệp xấu đi; P/E tính trên lợi nhuận quá khứ nên che đi suy giảm, và cổ phiếu chu kỳ trông rẻ nhất ở đỉnh chu kỳ (xem mục chuẩn hoá lợi nhuận). Về học thuật, hiệu ứng giá trị và động lượng đều được ghi nhận như dị thường so với CAPM. Do đó câu "xu thế hiệu quả nhất" của thầy là nhận định của thầy, chưa phải kết luận chung; số liệu trên chỉ nói xu thế có sinh lời trong mô phỏng, không nói là tốt nhất.
Giới hạn ở Việt Nam: tôi chưa tìm được nghiên cứu độc lập về hiệu quả của chiến lược xu thế ở thị trường Việt Nam.

**Liên hệ với bài học:** Thầy xếp xu thế lên trên giá trị; để hiểu, cần nắm cả hai trường phái và cả bẫy giá trị. Phần quản lý rủi ro (cắt lỗ, quy mô lệnh) là phần cốt lõi của xu thế, không phải chỉ là dự đoán hướng giá.

**Đọc thêm:** [Trend following (Wikipedia)](https://en.wikipedia.org/wiki/Trend%5Ffollowing); [A Century of Evidence on Trend-Following Investing (AQR)](https://www.aqr.com/Insights/Research/Journal-Article/A-Century-of-Evidence-on-Trend-Following-Investing); [Value traps (SuperMoney)](https://supermoney.com/encyclopedia/value-trap); [What is a value trap? (Capital.com)](https://capital.com/en-gb/learn/trading-psychology/value-trap)

### CAN SLIM của William O'Neil

**Thầy nhắc ở:** B11 02:56 - thầy chê, nói cần mua tạp chí cho thị trường Mỹ.

**Là gì:** CAN SLIM là hệ thống chọn cổ phiếu tăng trưởng của William O'Neil, người sáng lập Investor's Business Daily (IBD), trình bày trong cuốn How to Make Money in Stocks.

**Giải thích:** Mỗi chữ cái là một tiêu chí. C: lợi nhuận mỗi cổ phiếu quý hiện tại tăng ít nhất 25% so với cùng kỳ; A: lợi nhuận hằng năm tăng từ 25% trong 3 năm, ROE từ 17%; N: sản phẩm, dịch vụ hoặc quản lý mới và giá phá vỡ mô hình nền; S: cung cầu, khối lượng tăng khi giá tăng; L: mua cổ phiếu dẫn đầu của ngành dẫn đầu, đo bằng sức mạnh giá tương đối 12 tháng so với S&P 500; I: có tổ chức lớn mua; M: chỉ mua khi thị trường chung đang trong xu thế tăng đã xác nhận. Điểm mua là khi giá thoát khỏi vùng tích luỹ (thường mô hình "cốc có quai" từ 7 tuần), và cắt lỗ 7 đến 8% dưới điểm mua. Ví dụ số: EPS quý này 1.300 đồng so với 1.000 đồng cùng kỳ là tăng 30%, đạt tiêu chí C; mua ở 50.000 đồng thì cắt lỗ ở khoảng 46.000 đến 46.500 đồng. Theo Wikipedia, hiệp hội AAII xếp CAN SLIM là chiến lược tốt nhất giai đoạn 1998 đến 2009; nhưng cột báo của Jason Zweig (WSJ, 2026) nhận xét kết quả giả lập rất tốt trong khi hai quỹ của O'Neil không đạt lợi suất tốt, nên hiệu quả thực tế còn tranh luận. Yêu cầu dữ liệu: xếp hạng sức mạnh tương đối, tỷ lệ sở hữu tổ chức và dữ liệu lịch sử thị trường, thường lấy từ IBD, vốn thiết kế cho thị trường Mỹ; tôi không tìm được nguồn về việc áp dụng ở Việt Nam, và theo lẽ thường dữ liệu sở hữu tổ chức công khai ở Việt Nam không đầy đủ như vậy.

**Liên hệ với bài học:** Thầy chê vì CAN SLIM đòi hỏi dữ liệu và công cụ của thị trường Mỹ, chứ không phải vì logic của nó; một số nội dung (xu thế thị trường, cắt lỗ) trùng với tư tưởng thầy giảng.

**Đọc thêm:** [CAN SLIM (Wikipedia)](https://en.wikipedia.org/wiki/CAN%5FSLIM); [William O'Neil's CAN SLIM trading strategy explained (Hedge Fund Alpha)](https://hedgefundalpha.com/strategies/william-oneils-can-slim-trading-strategy-explained/); [CAN SLIM investing (Stockopedia)](https://www.stockopedia.com/content/how-does-can-slim-investing-work-55881)

### Chỉ báo tâm lý ngược chiều (contrarian sentiment) và chỉ số VIX

**Thầy nhắc ở:** B16 01:05, B17 02:48 - thầy dùng đồng thuận của công ty chứng khoán làm tín hiệu ngược, học viên nhắc VIX.

**Là gì:** Chỉ báo tâm lý ngược chiều coi sự lạc quan hoặc bi quan quá mức của đám đông là tín hiệu ngược. VIX là chỉ số do sàn Cboe công bố đo mức biến động kỳ vọng của S&P 500 trong 30 ngày tới, thường gọi là "chỉ số sợ hãi".

**Giải thích:** VIX được Cboe công bố từ 19/01/1993 (công thức do Robert Whaley xây dựng); từ 2003 dùng quyền chọn S&P 500 thay vì S&P 100. Cboe tính từ giá chào mua và chào bán của quyền chọn S&P 500 có hạn khoảng 23 đến 37 ngày, không dùng công thức Black-Scholes mà suy phương sai trực tiếp từ giá quyền chọn, rồi lấy căn bậc hai và quy ra phần trăm theo năm. Cách đọc: VIX 20 hàm ý biến động kỳ vọng 20% một năm, tương ứng khoảng 20 / căn 12 = 5,8% một tháng (một độ lệch chuẩn); VIX 82,69 hàm ý khoảng 23,9% một tháng. Số liệu: VIX đạt đỉnh trong ngày 89,53 ngày 24/10/2008, đóng cửa kỷ lục 80,74 ngày 21/11/2008, rồi đóng cửa 82,69 ngày 16/03/2020, mức cao nhất từ khi có chỉ số theo Wikipedia. Đợt tăng 2020 trùng thời điểm thị trường cổ phiếu rơi mạnh đầu tháng 3/2020. Phê bình: VIX chỉ phản ánh giá quyền chọn hiện tại và không phải dự báo chắc chắn. Với mục tín hiệu ngược: khi giới chuyên môn và đám đông cùng lạc quan, sức mua đã dùng hết nên rủi ro đảo chiều; khi cùng bi quan thì ngược lại. Đây là hiểu biết chung (không tra nguồn riêng trong lượt này); nhiều khảo sát như AAII dùng ý này, nhưng tín hiệu ngược chiều thường sai khi xu thế kéo dài. Việt Nam: tôi chưa tìm được chỉ số tương đương VIX do sàn trong nước công bố.

**Liên hệ với bài học:** Thầy dùng mức đồng thuận của công ty chứng khoán như một dạng chỉ báo tâm lý ngược chiều (xem mục ba lớp giá). VIX là ví dụ chuẩn của chỉ báo tâm lý đo được bằng số.

**Đọc thêm:** [VIX (Wikipedia)](https://en.wikipedia.org/wiki/VIX); [Cboe VIX Methodology (PDF)](https://cdn.cboe.com/resources/vix/VIX%5FMethodology.pdf); [VIX calculation explained (Macroption)](https://www.macroption.com/vix-calculation/); [Cboe VIX FAQ](https://markets.cboe.com/tradable%5Fproducts/vix/faqs)

### Đánh gấp thếp (Martingale), anti-Martingale và nhồi lệnh thuận xu hướng (pyramiding)

**Thầy nhắc ở:** B16 00:33 - thầy ví cách chồng margin của mình với gấp thếp.

**Là gì:** Martingale là chiến lược gấp đôi mức cược sau mỗi lần thua, hy vọng lần thắng đầu tiên bù hết lỗ trước đó. Anti-Martingale ngược lại: tăng quy mô sau khi thắng và giảm sau khi thua. Pyramiding là nhồi thêm vị thế khi lệnh đang lãi, tức anti-Martingale áp dụng trong một lệnh.

**Giải thích:** Martingale có nguồn gốc từ Pháp thế kỷ 18. Wikipedia ví dụ: bankroll 63 đơn vị, cược 1 rồi gấp đôi sau mỗi lần thua; sáu lần thua liên tiếp tốn 1+2+4+8+16+32 = 63 và hết vốn. Nếu xác suất thua mỗi ván là 10/19 thì sáu lần thua liên tiếp xảy ra khoảng 2,13% mỗi chu kỳ; kỳ vọng mỗi chu kỳ khoảng -0,36 đơn vị. Chuỗi thua dài phổ biến hơn trực giác: trên bàn roulette một số không, trong 200 ván có chuỗi 6 lần thua ít nhất một lần khoảng 84%. Thực tế còn có mức cược tối đa của sòng bạc, nên lý thuyết "cuối cùng luôn thắng" không thành. Công thức lợi nhuận kỳ vọng mỗi vòng là B x (1 - (2q) mũ n), với B là cược đầu, q xác suất thua, n số lần gấp có thể trả; khi q lớn hơn 1/2 thì kỳ vọng là âm. Trong giao dịch, "gấp thếp" tương đương mua thêm gấp đôi khi giá giảm (trung bình giá xuống), hoặc dùng margin chồng lên vị thế đang lỗ; rủi ro là lệnh gọi ký quỹ hoặc hết vốn.
Pyramiding theo chiều thắng: mua 40 cổ phiếu ở 100, thêm 30 ở 105, thêm 20 ở 110, thêm 10 ở 115: giá vốn bình quân = (4.000 + 3.150 + 2.200 + 1.150) / 100 = 105. Lượng nhồi giảm dần giúp giá vốn không bị kéo lên quá nhanh, và nếu giá quay đầu thì lệnh ban đầu còn lãi đệm. Các trang đào tạo giao dịch thường coi anti-Martingale là cách quản lý tốt hơn nếu có trần rủi ro; Wikipedia thì cho rằng chuỗi "nóng" chỉ là ngụy biện của con bạc và anti-Martingale không tạo ra lợi nhuận trong cờ bạc có kỳ vọng âm. Khác biệt chính: thị trường chứng khoán có thể có kỳ vọng dương và có xu thế, còn ván bạc thì không, nên so sánh chỉ mang tính hình thức. Quy định ký quỹ cụ thể ở Việt Nam do từng công ty chứng khoán đặt ra; tôi chưa tra nguồn.

**Liên hệ với bài học:** Thầy tự nhận cách chồng margin của mình giống gấp thếp để cảnh báo rủi ro: thêm vị thế theo hướng lỗ làm quy mô tăng đúng lúc vốn cạn. Pyramiding thuận xu hướng (thêm khi lãi) khác hẳn về cấu trúc rủi ro và thường được xem là an toàn hơn.

**Đọc thêm:** [Martingale (betting system) (Wikipedia)](https://en.wikipedia.org/wiki/Martingale%5F(betting%5Fsystem)); [Martingale and anti-Martingale (LuxAlgo)](https://www.luxalgo.com/library/concept/martingale-anti-martingale/); [How to trade with the anti-Martingale (Unger Academy)](https://ungeracademy.com/posts/how-to-trade-with-the-anti-martingale); [Martingale strategy and averaging down (Capital.com)](https://capital.com/the-martingale-approach-and-averaging-down)

### Lệnh cắt lỗ, chốt lời (stop-loss, take-profit) và trượt giá (slippage)

**Thầy nhắc ở:** B17 00:45 - thầy và học viên bàn cách đặt lệnh.

**Là gì:** Lệnh cắt lỗ (stop-loss) là lệnh tự động bán khi giá chạm mức chỉ định để giới hạn thua lỗ; chốt lời (take-profit) bán khi giá chạm mức lãi mục tiêu. Trượt giá (slippage) là chênh lệch giữa giá kỳ vọng và giá khớp thực tế.

**Giải thích:** Theo bản tin của SEC (investor.gov), khi giá chạm mức dừng thì lệnh dừng thành lệnh thị trường, nên giá khớp có thể lệch đáng kể so với giá dừng, nhất là khi thị trường chạy nhanh. Lệnh dừng giới hạn (stop-limit) tránh khớp ở giá bất ngờ nhưng có thể không khớp. Ví dụ số: giá đóng cửa 50, đặt cắt lỗ ở 48, hôm sau mở cửa ở 39 do tin xấu: lệnh khớp gần 39, lỗ gần 22% thay vì 4% như dự tính. Slippage còn phát sinh từ thanh khoản mỏng và quy mô lệnh lớn; Wikipedia ghi là không thể loại bỏ hoàn toàn. Ở Việt Nam, theo hiểu biết chung (chưa tra nguồn): thị trường dùng lệnh khớp theo giá và thời gian, có biên độ giá sàn trần mỗi phiên; khi giá kịch sàn, lệnh bán có thể không khớp, nên cắt lỗ có thể không thực hiện được. Việc dùng "lệnh điều kiện" của từng công ty chứng khoán cần xem quy định của công ty đó.

**Liên hệ với bài học:** Thầy và học viên bàn cách đặt mức cắt lỗ; thông tin này giải thích vì sao mức cắt lỗ chỉ là mức kích hoạt chứ không bảo đảm giá khớp, và cần tính slippage vào backtest.

**Đọc thêm:** [Investor Bulletin: Stop, stop-limit, trailing stop orders (SEC / investor.gov)](https://www.investor.gov/additional-resources/news-alerts/alerts-bulletins/investor-bulletin-stop-stop-limit-trailing-stop); [Slippage (finance) (Wikipedia)](https://en.wikipedia.org/wiki/Slippage%5F(finance)); [Stop-loss order (Corporate Finance Institute)](https://corporatefinanceinstitute.com/resources/capital-markets/stop-loss-order/)

### Giá vốn bình quân và trung bình giá

**Thầy nhắc ở:** B14 00:20 - thầy viết công thức tay không rõ.

**Là gì:** Giá vốn bình quân là tổng tiền đã bỏ ra (kể cả phí) chia cho tổng số cổ phiếu mua được; đó là trung bình gia quyền theo số lượng. Trung bình giá (dollar-cost averaging) là mua định kỳ bằng một số tiền cố định.

**Giải thích:** Công thức: giá vốn bình quân = (tổng của giá mua x số lượng + phí mua) / tổng số lượng. Ví dụ: mua 1.000 cổ phiếu giá 30.000 đồng rồi 500 cổ phiếu giá 24.000 đồng: (30.000.000 + 12.000.000) / 1.500 = 28.000 đồng. Nếu phí mua giả định 0,15% (giả định, phí tuỳ công ty chứng khoán) thì phí 63.000 đồng, giá vốn 42.063.000 / 1.500 = 28.042 đồng. Cá nhân bán chứng khoán nộp thuế thu nhập cá nhân 0,1% trên giá trị bán, bất kể lãi hay lỗ (Thông tư 111/2013 và 92/2015); các bài báo tháng 9/2025 cho biết Bộ Tài chính rút đề xuất thuế 20% trên lãi ròng và giữ 0,1%, tôi chưa kiểm được văn bản có hiệu lực ở tháng 11/2026. Giá hoà vốn S thoả mãn S x 1.500 x (1 - 0,001 - 0,0015) = 42.063.000, tức S khoảng 28.112 đồng (với phí bán giả định 0,15%). Khi mua cùng số tiền mỗi kỳ, giá vốn là trung bình điều hoà của các giá mua và luôn thấp hơn trung bình cộng: mua 3 triệu đồng ở 30.000 rồi 3 triệu đồng ở 24.000 được 100 + 125 = 225 cổ phiếu, giá vốn 6.000.000 / 225 = 26.667 đồng, thấp hơn trung bình cộng 27.000 đồng. Cảnh báo: bình quân giá xuống khi mã đang xấu đi là dạng Martingale (xem mục trên); và cần điều chỉnh khi có chia tách, cổ phiếu thưởng.

**Liên hệ với bài học:** Công thức tay của thầy là trung bình gia quyền nói trên; cần nhớ giá vốn thực tế gồm phí và thuế khi tính hoà vốn.

**Đọc thêm:** [Dollar-cost averaging formula (Stash)](https://www.stash.com/learn/dollar-cost-averaging-formula-calculation/); [Dollar-cost averaging (Wall Street Prep)](https://www.wallstreetprep.com/knowledge/dollar-cost-averaging-dca/); [Mức thu thuế 0,1% trên giá chuyển nhượng, Bộ Tài chính rút đề xuất 20% (VnEconomy)](https://vneconomy.vn/bo-tai-chinh-rut-de-xuat-ap-thue-20-doi-voi-lai-rong-chung-khoan.htm); [Thuế chuyển nhượng chứng khoán (DSC)](https://www.dsc.com.vn/kien-thuc/thue-chuyen-nhuong-chung-khoan-la-gi)

## Cụm 7. Thống kê, mô hình định lượng và kiểm thử

### Hồi quy tuyến tính, R và R bình phương, thống kê t, mức ý nghĩa, hồi quy giả

**Thầy nhắc ở:** B1 01:26, B3 00:23, B3 00:45, B3 02:44, B3 03:07 - xuất hiện trong mọi bảng hồi quy của thầy.

**Là gì:** Hồi quy tuyến tính tìm đường thẳng y = a + b x khớp nhất với dữ liệu (phương pháp bình phương nhỏ nhất). R bình phương (R2) là tỷ lệ biến thiên của y được giải thích bởi x; thống kê t của một hệ số bằng hệ số chia sai số chuẩn của nó, dùng để kiểm định hệ số có khác 0 hay không. Hồi quy giả (spurious regression) là hồi quy cho kết quả "có ý nghĩa" dù hai chuỗi không liên quan.

**Giải thích:**
- R2 = 1 - (tổng bình phương phần dư / tổng bình phương quanh trung bình). R2 bằng 0 nghĩa là mô hình không hơn việc dự đoán bằng trung bình; bằng 1 là khớp hoàn hảo. Trong hồi quy đơn, R2 bằng bình phương hệ số tương quan, còn R là hệ số tương quan. Hạn chế: thêm biến vô nghĩa vẫn làm R2 không giảm (nên dùng R2 hiệu chỉnh); R2 cao không có nghĩa là có quan hệ nhân quả; nó không nói gì về ngoại lệ hay biến bị bỏ sót.
- Thống kê t = hệ số / sai số chuẩn. Ví dụ: beta 1,2 với sai số chuẩn 0,4 cho t = 3. Ngưỡng thường dùng: giá trị tuyệt đối của t từ khoảng 2 trở lên (mẫu lớn, 1,96 tương ứng mức ý nghĩa 5%); với 20 quan sát (18 bậc tự do) ngưỡng theo bảng t chuẩn là khoảng 2,10, tức mẫu nhỏ đòi hỏi t lớn hơn. P-value dưới 5% nghĩa là nếu hệ số thật bằng 0 thì khả năng thấy kết quả cực đoan như vậy chưa tới 5%; không phải xác suất giả thuyết đúng.
- Hồi quy giả: Granger và Newbold (1974) mô phỏng hồi quy giữa các bước đi ngẫu nhiên độc lập và thấy R2 cao cùng t lớn xuất hiện thường xuyên; khi chuỗi không dừng, t và R2 không còn theo phân phối thường, và t giữa hai bước đi ngẫu nhiên độc lập tiến tới vô cùng khi mẫu tăng. Dấu hiệu: R2 cao nhưng thống kê Durbin-Watson (đo tự tương quan phần dư) rất thấp; quy tắc ngón tay cái là R2 lớn hơn Durbin-Watson thì nghi hồi quy giả. Cách khắc phục: dùng sai phân (lợi suất thay vì mức giá) hoặc kiểm định đồng liên kết. Vì vậy hồi quy mức giá cổ phiếu này trên mức giá cổ phiếu kia (R2 cao) kém tin cậy hơn hồi quy lợi suất ngày trên lợi suất ngày.
- Giới hạn khi áp dụng ở Việt Nam: tôi không tìm được nguồn riêng; theo lẽ thường, chuỗi lợi suất ngắn và nhiều ngày thanh khoản thấp làm hệ số kém ổn định.

**Liên hệ với bài học:** Mọi bảng hồi quy của thầy gồm hệ số, t và R2; đọc theo thứ tự: dấu và độ lớn hệ số, t có đủ lớn không, R2 giải thích bao nhiêu, rồi hỏi chuỗi có dừng không. Chỉ R2 cao ở chuỗi thời gian là chưa đủ.

**Đọc thêm:** [Coefficient of determination (Wikipedia)](https://en.wikipedia.org/wiki/Coefficient%5Fof%5Fdetermination); [More about spurious regressions (Dave Giles)](https://davegiles.blogspot.com/2012/05/more-about-spurious-regressions.html?m=1); [Time series chapter (Reed College)](https://www.reed.edu/economics/parker/s14/312/tschapters/S13%5FCh%5F2.pdf); [Spurious regression (MetricGate)](https://metricgate.com/blogs/spurious-regression-nonstationary-series/)

### Các mô hình chuỗi thời gian ARIMA, GARCH, VAR

**Thầy nhắc ở:** B7 03:47, B10 01:57, B10 02:00, B12 03:01 - thầy viết lên bảng rồi phê bình, báo cáo mẫu có GARCH(1,1) và ARIMA Forecast T+3.

**Là gì:** ARIMA(p, d, q) mô hình hoá một chuỗi bằng các giá trị quá khứ của nó (tự hồi quy, p), sai phân d lần để loại xu thế (d), và các sai số quá khứ (trung bình trượt, q). GARCH mô hình hoá phương sai thay đổi theo thời gian. VAR mô hình hoá nhiều chuỗi cùng lúc, mỗi chuỗi phụ thuộc vào quá khứ của tất cả các chuỗi.

**Giải thích:**
- ARIMA: giả định chuỗi dừng sau khi lấy sai phân; ví dụ giá 100, 102, 101, 105 có sai phân bậc một là 2, -1, 4. Với AR(1) y(t) = 0,5 x y(t-1) + sai số: nếu y hôm nay là 2 thì dự báo ngày mai là 1, ngày kia 0,5, tức dự báo tắt dần về trung bình. Khoảng dự báo (ví dụ 95%) rộng ra khi kỳ hạn dài hơn, như mục "ARIMA Forecast T+3". Hạn chế: mô hình tuyến tính, khoảng dự báo giả định sai số chuẩn và không tự tương quan, công cụ chọn bậc tự động có thể cho kết quả đáng ngờ.
- GARCH(1,1) (Engle 1982 cho ARCH, Bollerslev 1986 cho GARCH): phương sai(t) = omega + alpha x (cú sốc kỳ trước) bình phương + beta x phương sai kỳ trước. Ví dụ omega = 0,000002; alpha = 0,1; beta = 0,85; phương sai trước 0,0001 (độ lệch chuẩn 1%), cú sốc -2%: phương sai mới = 0,000002 + 0,1 x 0,0004 + 0,85 x 0,0001 = 0,000127, độ lệch chuẩn 1,13%. Phương sai dài hạn = omega / (1 - alpha - beta) = 0,00004, độ lệch chuẩn ngày 0,63%. Dùng để bắt hiện tượng "biến động tụ cụm" (sóng lớn kéo theo sóng lớn) và đo rủi ro.
- VAR (Christopher Sims đề xuất như phương pháp ít áp đặt lý thuyết): y(t) = c + A1 y(t-1) + ... + sai số, với y là vectơ nhiều biến, dùng cho dự báo và phân tích phản ứng xung (một cú sốc ở biến này tác động biến kia thế nào). Hạn chế: số tham số tăng rất nhanh (ví dụ 7 biến, 4 độ trễ cần 203 tham số), chọn độ trễ khó, các biến phải cùng bậc tích hợp, nếu đồng liên kết thì cần mô hình hiệu chỉnh sai số.
- Giới hạn ở Việt Nam: các mô hình đều cần chuỗi đủ dài và ổn định; ở thị trường nhỏ, thay đổi quy chế và biên độ giá làm chuỗi dễ đổi cấu trúc. Tôi chưa tìm được nghiên cứu riêng để dẫn.

**Liên hệ với bài học:** Thầy viết các tên này lên bảng để phê bình: các mô hình đều dựa trên quá khứ và giả định tuyến tính hoặc phân phối chuẩn nên dự báo giá yếu; GARCH hữu ích hơn cho rủi ro (độ biến động) hơn là cho hướng giá, điều này khớp với việc báo cáo mẫu dùng GARCH(1,1).

**Đọc thêm:** [ARIMA (Wikipedia)](https://en.wikipedia.org/wiki/Autoregressive%5Fintegrated%5Fmoving%5Faverage); [Autoregressive conditional heteroskedasticity (Wikipedia)](https://en.wikipedia.org/wiki/Autoregressive%5Fconditional%5Fheteroskedasticity); [Vector autoregression (Wikipedia)](https://en.wikipedia.org/wiki/Vector%5Fautoregression); [GARCH(p, q) models (QuantStart)](https://www.quantstart.com/articles/Generalised-Autoregressive-Conditional-Heteroskedasticity-GARCH-p-q-Models-for-Time-Series-Analysis/); [ARIMA, VAR and GARCH (Michael Tien)](https://michaeltien8901.github.io/puffin/09-time-series-models/arima-var-garch)

### ARIMA, Machine Learning, Deep Learning, phân tích cụm (clustering), AIQuant

**Thầy nhắc ở:** B1 03:11, B2 00:12, B2 00:37, B3 01:46 - thầy so sánh trong tài chính, hệ thống AIQuant chỉ lướt.

**Là gì:** Học máy (machine learning) là nhóm phương pháp để máy học quy luật từ dữ liệu. Học có giám sát dùng dữ liệu có nhãn để dự đoán kết quả đã biết (ví dụ dự đoán lợi suất, phân loại tăng hay giảm); học không giám sát tìm cấu trúc trong dữ liệu không nhãn (phân cụm). Học sâu (deep learning) là mạng nơ-ron nhiều tầng.

**Giải thích:** Theo các nguồn tìm được, các phương pháp có giám sát gồm cây quyết định và rừng ngẫu nhiên, máy vectơ hỗ trợ, mạng nơ-ron; mạng nơ-ron linh hoạt nhất nhưng khó giải thích nhất. Phân cụm là hướng chính của học không giám sát trong tài chính, với k-means thông dụng nhất; báo cáo của CFA Institute lưu ý k-means hợp với dữ liệu số, cụm gần tròn và cỡ đều nhau, và chỉ phát hiện được cụm tách bằng đường thẳng. Ứng dụng: gom cổ phiếu thành cụm để xây danh mục, phát hiện chế độ thị trường, phát hiện bất thường. Ví dụ số: sáu cổ phiếu theo (beta, P/E): A(0,8; 10), B(0,9; 12), C(1,0; 11), D(1,4; 25), E(1,5; 28), F(1,6; 26). Chọn A và F làm tâm ban đầu, B và C gần A, D và E gần F; tâm mới là (0,9; 11) và (1,5; 26,3). Thuật toán tách được nhóm "phòng thủ, P/E thấp" và nhóm "beta cao, P/E cao" mà không cần nhãn. So với ARIMA: ARIMA là mô hình tuyến tính một chuỗi với ít tham số, dễ giải thích nhưng yếu khi quan hệ phi tuyến; học máy và học sâu linh hoạt hơn nhưng dễ quá khớp và cần nhiều dữ liệu. Về AIQuant: tôi chưa tìm được nguồn đáng tin mô tả hệ thống này; từ khoá gợi ý: "AIQuant hệ thống định lượng" kèm tên đơn vị phát hành.

**Liên hệ với bài học:** Thầy lướt qua các thuật ngữ để so với mô hình thống kê cổ điển mình đang dạy; cần nhớ học máy không loại bỏ được nguy cơ quá khớp (xem mục Backtest ngay dưới).

**Đọc thêm:** [Supervised vs unsupervised learning in finance (Acadifi)](https://www.acadifi.com/community/supervised-vs-unsupervised-learning-finance-applications); [Unsupervised learning for trading (QuantInsti)](https://blog.quantinsti.com/unsupervised-learning); [AI in asset management: unsupervised learning (CFA Institute, PDF)](https://rpc.cfainstitute.org/sites/default/files/docs/research-reports/rf%5Faiinassetmanagement%5F01%5Funsupervisedlearningi%5Fonline.pdf)

### Backtest, tối ưu tham số, quá khớp và look-ahead bias

**Thầy nhắc ở:** B10 01:36, B10 02:06 - thầy nhắc kiểm thử và lỗi dùng dữ liệu sau thời điểm t.

**Là gì:** Backtest là chạy một chiến lược trên dữ liệu quá khứ để ước lượng nó sẽ cho kết quả thế nào. Quá khớp (overfitting) là chỉnh chiến lược khớp quá sát dữ liệu quá khứ đến mức học cả nhiễu. Look-ahead bias là dùng thông tin mà tại thời điểm ra quyết định chưa có.

**Giải thích:** Theo Wikipedia, backtest là một dạng kiểm định chéo trên giai đoạn quá khứ, và thường có thể tìm ra chiến lược đã chạy tốt trong quá khứ nhưng không tốt về sau. Các lỗi hay gặp:
- Look-ahead bias: dùng giá đóng cửa ngày t để phát tín hiệu rồi mua ngay ở giá đóng cửa ngày t; dùng báo cáo tài chính quý chưa công bố tại ngày đó (báo cáo thường công bố sau ngày kết thúc quý); dùng dữ liệu đã được hiệu chỉnh về sau. Cách tránh: gắn đúng mốc thời gian công bố cho mỗi dữ liệu, tín hiệu ngày t chỉ khớp ở ngày t+1.
- Tối ưu tham số quá mức: thử hàng trăm tổ hợp rồi chọn tổ hợp tốt nhất thì kết quả chủ yếu là may rủi. Ví dụ số: nếu mỗi chiến lược vô dụng có 5% khả năng "trông có ý nghĩa" do ngẫu nhiên, thử 100 chiến lược thì xác suất ít nhất một cái trông có ý nghĩa là 1 - 0,95 mũ 100, khoảng 99,4%, và kỳ vọng có 5 cái.
- Cách phòng: tách mẫu trong (để xây) và mẫu ngoài (để kiểm), kiểm tiến theo thời gian (walk-forward), tính phí và trượt giá, giữ ít tham số, thiết lập luật trước khi xem kết quả. Một nguồn blog nêu giới hạn 3 đến 5 tham số nhưng đó không phải chuẩn chung.
- Các nguồn tôi dùng chủ yếu là bài hướng dẫn và blog; Wikipedia không nhắc look-ahead bias nên phần này dựa vào các bài còn lại. Ở Việt Nam, dữ liệu lịch sử ngắn và giá chưa điều chỉnh theo cổ tức, chia tách, phát hành thêm làm backtest dễ sai; đây là lưu ý chung chưa tra nguồn riêng.

**Liên hệ với bài học:** Thầy nhắc lỗi dùng dữ liệu sau thời điểm t khi kiểm thử chiến lược; biết look-ahead bias và quá khớp là điều kiện để tin hoặc không tin một kết quả backtest, kể cả của chính thầy và của AIQuant.

**Đọc thêm:** [Backtesting (Wikipedia)](https://en.wikipedia.org/wiki/Backtesting); [The seven sins of quantitative investing (Portfolio Optimization book)](https://bookdown.org/palomar/portfoliooptimizationbook/8.2-seven-sins.html); [Why your backtest is lying to you (DEV Community)](https://dev.to/eedgee/why-your-backtest-is-lying-to-you-3-tests-that-catch-lookahead-bias-overfitting-and-fantasy-2bnc); [Backtesting bias feels good until you blow up (Robot Wealth)](https://robotwealth.com/backtesting-bias-feels-good-until-you-blow-up/)

## Cụm 8. Ngành quản lý quỹ và nghề phân tích

### Lợi nhuận bình quân của quỹ đầu tư Mỹ, quỹ quant và quỹ ngoại tại Việt Nam

**Thầy nhắc ở:** B7 02:59, B9 00:23 - thầy nêu lợi nhuận quỹ quant Mỹ 3-7%, quỹ Mỹ và ngoại tại Việt Nam 7-8%, 12%, 20% theo trí nhớ.

**Là gì:** Mục này so sánh các con số thầy nêu theo trí nhớ (bối cảnh 2021) với số liệu công khai tìm được.

**Giải thích:** Tôi chưa tìm được nguồn đáng tin cho các con số 3-7% của quỹ quant Mỹ nói chung hay 7-8%, 12%, 20% của quỹ ngoại ở Việt Nam, nên không xác nhận hay bác bỏ được; từ khoá gợi ý: "HFRI quantitative index annual return", "Vietnam fund annualised return Dragon Capital VEIL factsheet". Số liệu tham chiếu tìm được: (1) S&P 500 có tốc độ tăng trưởng kép khoảng 9,8% mỗi năm kể cả cổ tức từ 1926 (khoảng 6% sau lạm phát) theo Wikipedia; (2) quỹ Medallion của Renaissance Technologies, theo tiểu sử của Gregory Zuckerman, đạt khoảng 66% mỗi năm trước phí và 39% sau phí (giai đoạn 1988 đến 2018; số này là trung bình cộng, lãi kép gộp khoảng 63,3%, là ước tính của quỹ tư nhân chưa được kiểm toán công khai), nhưng đây là ngoại lệ chứ không phải quỹ quant điển hình. Ví dụ số: 10.000 USD sinh lời 5% mỗi năm trong 20 năm còn khoảng 26.500 USD, còn ở 9,8% là khoảng 64.900 USD. So sánh này chưa công bằng vì quỹ quant trung tính thị trường có rủi ro và mục tiêu khác chỉ số cổ phiếu. Ở Việt Nam chưa có nguồn nào trong lượt tra cứu so sánh trực tiếp.

**Liên hệ với bài học:** Thầy dùng các số này để đặt kỳ vọng thực tế về lợi suất của quỹ chuyên nghiệp; nên coi đó là ước lượng theo trí nhớ và đối chiếu với báo cáo quỹ từng năm trước khi dùng.

**Đọc thêm:** [S&P 500 (Wikipedia)](https://en.wikipedia.org/wiki/S%26P%5F500); [Medallion Fund (Wikipedia)](https://en.wikipedia.com/wiki/Medallion%5FFund); [Medallion fund history (Quantt)](https://www.quantt.co.uk/resources/medallion-fund-history)

### Chứng chỉ CFA (Chartered Financial Analyst)

**Thầy nhắc ở:** B13 02:23 - thầy và học viên trao đổi giá trị của CFA.

**Là gì:** CFA là chứng chỉ nghề phân tích đầu tư toàn cầu do CFA Institute cấp, gồm ba cấp thi và yêu cầu kinh nghiệm làm việc.

**Giải thích:** Chương trình có ba cấp (Level I, II, III), khuyến nghị khoảng 300 giờ học mỗi cấp. Cấp I gồm đạo đức nghề nghiệp, phương pháp định lượng, kinh tế và phân tích báo cáo tài chính; cấp II và III dựa trên 10 chủ đề cốt lõi, ngày càng khó. Theo các nguồn, từ khoảng 2024 đến 2025 chương trình có thêm các mô-đun kỹ năng thực hành ở cấp I và II. Muốn nhận danh hiệu Charterholder cần đỗ cả ba cấp, có tối thiểu 4.000 giờ kinh nghiệm liên quan đến quy trình ra quyết định đầu tư trong ít nhất 36 tháng, là hội viên và có thư giới thiệu. Thời gian hoàn thành thường 3 đến 4 năm; chi phí các kỳ thi 2026 khoảng 3.520 đến 4.600 USD tuỳ thời điểm đăng ký (theo nguồn thứ cấp; cần xem trang CFA Institute để biết con số hiện hành). Giá trị thực tế phụ thuộc vị trí công việc; tôi chưa tìm được nguồn so sánh mức công nhận của CFA trên thị trường lao động Việt Nam (từ khoá gợi ý: "CFA Vietnam charterholders số lượng").

**Liên hệ với bài học:** Thầy và học viên bàn xem CFA có đáng đầu tư không; thông tin trên giúp cân nhắc chi phí thời gian và tiền so với mục tiêu: CFA mạnh về khung lý thuyết (các mục định giá, danh mục, thống kê trong phụ lục này nằm trong chương trình) nhưng không dạy một phương pháp giao dịch cụ thể.

**Đọc thêm:** [CFA Program (CFA Institute)](https://www.cfainstitute.org/programs/cfa); [Chartered Financial Analyst (Wikipedia)](https://Www.Wikipedia.org/wiki/Chartered%5FFinancial%5FAnalyst); [CFA exams quick summary (300 Hours)](https://300hours.com/what-is-cfa-exam/)

## Phần kết

Phần 1 của phụ lục này đi từ khái niệm nền (giá trị và giá cả) qua các cách định giá, rồi sang lý thuyết thị trường, các chiến lược và công cụ định lượng. Gợi ý đọc: nắm trước các mục ở Cụm 1 và Cụm 2 (giá trị nội tại, DCF, FCFF, giá trị cuối kỳ), sau đó Cụm 3 và 4 khi đọc báo cáo định giá; Cụm 5 đến 7 hữu ích khi nghe thầy phê bình các mô hình và phương pháp kiểm thử. Có một số điểm tôi không tìm được nguồn đáng tin và đã ghi rõ trong từng mục: hệ thống AIQuant, vai trò cụ thể của Merton và Scholes trong LTCM, lợi nhuận bình quân của quỹ quant Mỹ và quỹ ngoại ở Việt Nam, và nghiên cứu về mức hiệu quả của thị trường Việt Nam. Các ví dụ số đều là số giả định để người đọc tự tính lại; mọi nội dung chỉ nhằm giải thích khái niệm, không phải lời khuyên đầu tư.
