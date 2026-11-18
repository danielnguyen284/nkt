# Phụ lục PL05 - Phân tích kỹ thuật

> Phụ lục của Bộ kiến thức NKT. Giải thích những khái niệm thầy nhắc tới trong bài giảng mà chưa giảng đầy đủ. Nội dung được tra cứu từ các nguồn bên ngoài (thời điểm tra cứu: tháng 11/2026), không phải lời thầy.

> Lưu ý chung: phụ lục chỉ giải thích khái niệm, không phải khuyến nghị mua bán. Nhiều công cụ trong phụ lục này (Fibonacci, sóng Elliott, Gann, mẫu hình, nến Nhật) có bằng chứng thực nghiệm yếu hoặc gây tranh cãi; phần "Giải thích" của từng mục ghi rõ người theo nó nói gì và giới học thuật đánh giá ra sao.

## Danh sách mục

**Cụm 1. Nền tảng: xu hướng, hỗ trợ kháng cự, bẫy, độ rộng, liên thị trường**
1. Giao dịch theo xu hướng (trend following) và day trading
2. Hỗ trợ, kháng cự, trendline, breakout và kênh hồi quy tuyến tính
3. Bẫy tăng giá (bull trap)
4. Độ rộng thị trường (market breadth)
5. Phân tích liên thị trường (intermarket analysis)

**Cụm 2. Chỉ báo kỹ thuật**
6. Đường trung bình động (SMA, EMA), MA 50 và MA 200, giao cắt vàng, giao cắt tử thần
7. MACD
8. Chỉ báo dao động và quá mua quá bán (RSI, Stochastic, CCI)
9. Bollinger Bands, Parabolic SAR, ADX, Chaikin Money Flow và các nhóm chỉ báo
10. Ichimoku Kinko Hyo (vùng mây)
11. Momentum, giao dịch tần suất cao (HFT) và scalping

**Cụm 3. Fibonacci, sóng Elliott, fractal**
12. Leonardo Fibonacci và dãy số Fibonacci
13. Các mức Fibonacci thoái lui và mở rộng
14. Fibonacci Time Zone, đường chu kỳ, quạt Fibonacci và cung Gann
15. Lý thuyết sóng Elliott và tiểu sử Ralph Nelson Elliott
16. Fractal, tự đồng dạng và sóng lồng sóng (Mandelbrot)

**Cụm 4. Mẫu hình giá, nến Nhật, price action**
17. Mẫu hình giá đảo chiều (vai đầu vai, cốc tay cầm) và sách của Bulkowski
18. Mẫu hình tiếp diễn (tam giác, nêm, cờ, cờ đuôi nheo, chữ nhật, ABCD)
19. Mark Minervini, SEPA và VCP
20. Mẫu nến Nhật (Hanging Man, Hammer)
21. Price action (PA)

**Cụm 5. Wyckoff, giá - khối lượng, cấu trúc lệnh**
22. Phương pháp Wyckoff
23. Phân tích giá và khối lượng (VSA), phiên phân phối, churning, test cung cầu
24. Market Profile và Volume Profile
25. Độ sâu thị trường và danh sách lệnh khớp
26. Khối lượng mua chủ động, bán chủ động

**Cụm 6. Công cụ, sách, chứng chỉ, chiến lược nhắc đến**
27. Công cụ: AmiBroker (AFL), TradingView (Pine Script, Replay), FireAnt
28. Chứng chỉ CMT
29. Sách của Alexander Elder (nguồn chưa chắc)
30. Chiến lược London breakout (forex) (đã chuyển sang folder ngoai-dau-tu)

## Cụm 1. Nền tảng: xu hướng, hỗ trợ kháng cự, bẫy, độ rộng, liên thị trường

### Giao dịch theo xu hướng (trend following) và day trading

**Thầy nhắc ở:** B1 00:19, B2 01:43 - chiến lược đuổi theo trend và các sách về giao dịch trong ngày.

**Là gì:** Trend following là cách giao dịch mua khi xu hướng giá đang lên và bán khi xu hướng đang xuống, không cố đoán đỉnh đáy. Day trading là mua bán trong cùng một phiên, đóng hết vị thế trước khi thị trường đóng cửa.

**Giải thích:** Người theo trend following chấp nhận vào lệnh muộn, bỏ lỡ đoạn đầu của xu hướng, đổi lại là có quy tắc rõ ràng. Quy tắc điển hình: dùng đường trung bình động để nhận diện xu hướng (ví dụ MA50 cắt lên MA100 thì mua, cắt xuống thì thoát), đặt cắt lỗ theo biên độ biến động (ví dụ cắt lỗ bằng 4 lần ATR 10 ngày; nếu ATR 10 ngày bằng 0,5% giá thì mức cắt lỗ là 2%), giảm khối lượng khi biến động cao. Đặc điểm: phần lớn lệnh có thể lỗ, lợi nhuận đến từ việc cắt lỗ nhanh và để lệnh thắng chạy. Rủi ro chính là "whipsaw", tức thị trường đi ngang lắc qua lắc lại làm hàng loạt tín hiệu sai. Day trading thì bị chi phí giao dịch, chênh lệch giá mua bán và đòn bẩy bào mòn. Nghiên cứu của Barber, Lee, Liu, Odean trên dữ liệu Đài Loan cho thấy hơn 8 trong 10 day trader thua lỗ trong một kỳ nửa năm điển hình, chỉ một phần rất nhỏ (dưới 1% số day trader) kiếm lời bền vững. Một nghiên cứu năm 2019 trên nhà giao dịch hợp đồng tương lai cổ phiếu Brazil cho thấy 97% người kiên trì hơn 300 ngày bị lỗ (theo tổng hợp trên Wikipedia).

**Liên hệ với bài học:** Thầy dùng hai khái niệm này làm nền để so sánh với cách nhìn của ông về chu trình đè, gom, đẩy, xả: đuổi theo trend là đi sau người dẫn dắt, còn giao dịch trong ngày là cuộc chơi chi phí cao. Hiểu biết phổ thông coi trend following là một chiến lược hợp lệ có quy tắc; thầy phê bình cách áp dụng máy móc.

**Đọc thêm:** [Trend following - Wikipedia](https://en.wikipedia.org/wiki/Trend_following); [Day trading - Wikipedia](https://en.wikipedia.org/wiki/Day_trading); [Barber, Lee, Liu, Odean - Do day traders rationally learn about their ability?](https://faculty.haas.berkeley.edu/odean/papers/day%20traders/day%20trading%20and%20learning%20110217.pdf); [Trend trading - CMC Markets](https://www.cmcmarkets.com/en-gb/trading-strategies/trend-trading)

### Hỗ trợ, kháng cự, trendline, breakout và kênh hồi quy tuyến tính

**Thầy nhắc ở:** B9 01:47, B10 01:50, B11 01:55 - slide "Support level" và kênh "Regression Trend" thầy kéo trên mã L14.

**Là gì:** Hỗ trợ (support) là vùng giá mà lực mua thường đủ mạnh để chặn đà giảm; kháng cự (resistance) là vùng giá mà lực bán thường chặn đà tăng. Trendline là đường nối các đáy (xu hướng lên) hoặc các đỉnh (xu hướng xuống). Breakout là khi giá vượt dứt khoát khỏi vùng hoặc đường đó. Kênh hồi quy tuyến tính là một đường thẳng khớp nhất với giá, kèm hai đường song song cách đều.

**Giải thích:** Quy tắc "đổi vai" thường được nêu: kháng cự bị phá thường trở thành hỗ trợ và ngược lại. Độ mạnh của một vùng thường được đo bằng số lần giá chạm và bật lại, thời gian vùng đó tồn tại, và khối lượng giao dịch tại đó. Breakout có khối lượng thấp thường kém tin cậy và dễ thành breakout giả (giá chui ra rồi quay lại vùng cũ); giới giao dịch hay chờ "phá vỡ rồi kiểm tra lại" (retest) để xác nhận. Kênh hồi quy: chọn số phiên N, dùng bình phương tối thiểu để tìm đường thẳng khớp nhất với giá đóng cửa, rồi vẽ đường trên và đường dưới cách đường giữa một số lần độ lệch chuẩn của phần dư (thường 2 lần). Các nền tảng khác nhau dùng độ lệch chuẩn tổng thể hay mẫu nên con số có thể lệch nhẹ. Về bằng chứng: nghiên cứu của Carol Osler (Fed New York, 2000) cho thấy các mức hỗ trợ kháng cự do các công ty ngoại hối công bố dự báo điểm gián đoạn xu hướng trong ngày tốt hơn ngẫu nhiên, và bà giải thích bằng việc các lệnh cắt lỗ, chốt lời tập trung quanh những mức giá tròn.

**Liên hệ với bài học:** Thầy kéo kênh hồi quy để mô tả vùng giá hợp lý của một giai đoạn, không phải để dự báo chính xác. Cách hiểu của thầy gắn vùng hỗ trợ kháng cự với hành vi của người gom và người xả, chứ không coi chúng là đường kẻ có sẵn ý nghĩa.

**Đọc thêm:** [Trend lines - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/chart-analysis/trend-lines); [Breakouts and fakeouts - IG](https://www.ig.com/en/ig-academy/the-basics-of-technical-analysis/breakouts-and-fakeouts); [Linear Regression - TradingView](https://www.tradingview.com/support/solutions/43000644936-linear-regression/); [Osler - Currency orders and exchange rate dynamics (FRBNY)](https://www.newyorkfed.org/medialibrary/media/research/staff_reports/sr125.pdf)

### Bẫy tăng giá (bull trap)

**Thầy nhắc ở:** B1 00:25, B4 03:14 - lời tự thoại ở nhịp phục hồi, tay to giăng bẫy cuối sóng.

**Là gì:** Bẫy tăng giá là một lần giá bứt lên khỏi kháng cự hoặc đảo chiều lên trông như xu hướng giảm đã kết thúc, rồi giá quay đầu giảm lại, nhốt những người vừa mua theo tín hiệu đó.

**Giải thích:** Dấu hiệu thường được nêu: giá vượt kháng cự nhưng khối lượng mỏng, chỉ báo động lượng (ví dụ RSI) không xác nhận, nhịp tăng xuất hiện sau một đoạn tăng dài rồi chững lại tại kháng cự, hoặc thị trường chung và nhóm ngành đi ngược lại. Giá thường nhanh chóng đóng cửa trở lại dưới mức vừa phá. Không có dấu hiệu nào chắc chắn, người giao dịch thường kết hợp khối lượng, vùng giá và lệnh cắt lỗ để hạn chế thiệt hại. Hiện tượng đối xứng là bẫy giảm giá (bear trap). Trong lý thuyết Wyckoff, cú "upthrust" sau phân phối chính là một dạng bẫy tăng giá.

**Liên hệ với bài học:** Thầy dùng khái niệm này theo nghĩa hành vi: tay to cố ý tạo nhịp hồi để bên mua cuối cùng nhập cuộc trước khi xả tiếp. Hiểu biết phổ thông mô tả bẫy như một mẫu hình giá kết quả; thầy nhấn vào ý đồ của người tạo ra nó, điều mà bên ngoài không quan sát trực tiếp được.

**Đọc thêm:** [What is a bull trap - Cointelegraph](https://cointelegraph.com/explained/what-is-a-bull-trap-and-how-to-identify-it); [What is a sucker rally - Nasdaq](https://www.nasdaq.com/articles/what-is-a-sucker-rally); [Breakouts and fakeouts - IG](https://www.ig.com/en/ig-academy/the-basics-of-technical-analysis/breakouts-and-fakeouts)

### Độ rộng thị trường (market breadth)

**Thầy nhắc ở:** B2 01:29 - chỉ số tăng nhờ vài mã trụ.

**Là gì:** Độ rộng thị trường đo xem có bao nhiêu cổ phiếu thực sự tham gia nhịp tăng hay giảm của chỉ số, thay vì chỉ nhìn bản thân chỉ số.

**Giải thích:** Chỉ báo cơ bản nhất là đường Advance-Decline (AD Line): tích luỹ chênh lệch số mã tăng trừ số mã giảm mỗi phiên. Nếu chỉ số lập đỉnh mới mà AD Line không lập đỉnh mới thì sự tăng chỉ dựa vào số ít mã lớn, gọi là phân kỳ độ rộng. McClellan Oscillator áp dụng ý tưởng giống MACD lên dữ liệu tăng giảm (hiệu của hai đường EMA 19 và 39 ngày của tỷ lệ tăng giảm), còn McClellan Summation Index là bản tích luỹ cho khung dài hơn. Ngoài ra còn có đường số mã lập đỉnh mới trừ đáy mới. Với chỉ số có trọng số vốn hoá như VN-Index, vài cổ phiếu vốn hoá lớn có thể kéo chỉ số lên dù đa số cổ phiếu đứng yên hoặc giảm, nên độ rộng đặc biệt có ý nghĩa.

**Liên hệ với bài học:** Thầy nhắc để giải thích vì sao chỉ số tăng mà tài khoản nhà đầu tư nhỏ không tăng theo: tay to dùng mã trụ để giữ chỉ số trong khi xả ở các mã khác.

**Đọc thêm:** [Advance-Decline Line - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/market-indicators/advance-decline-line); [McClellan Oscillator - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/market-indicators/mcclellan-oscillator); [Advantages and disadvantages of using breadth - StockCharts](https://stockcharts.com/articles/dancing/2018/11/advantages-and-disadvantages-of-using-breadth.html)

### Phân tích liên thị trường (intermarket analysis)

**Thầy nhắc ở:** B11 02:26 - học viên hỏi, thầy không giảng lại.

**Là gì:** Phân tích liên thị trường nghiên cứu mối quan hệ giữa bốn nhóm thị trường: cổ phiếu, trái phiếu, tiền tệ và hàng hoá, để đọc xem thị trường này đang báo hiệu gì cho thị trường kia.

**Giải thích:** Khái niệm này gắn với John J. Murphy, tác giả "Intermarket Technical Analysis" (Wiley, 1991) và các sách sau như "Intermarket Analysis" (bản 2 khoảng năm 2013) và "Trading with Intermarket Analysis" (2015). Các quan hệ thường được tóm tắt: giá hàng hoá và giá trái phiếu thường đi ngược chiều (tức lợi suất trái phiếu đi cùng chiều hàng hoá); đồng đô la mạnh thường gây sức ép lên hàng hoá; trái phiếu thường dẫn trước cổ phiếu. Các quan hệ này thay đổi theo giai đoạn của chu kỳ kinh tế và không cố định.

**Liên hệ với bài học:** Thầy không giảng sâu, nên người học chỉ cần biết đây là hướng phân tích vĩ mô bằng biểu đồ, khác với việc đọc riêng một mã.

**Đọc thêm:** [Intermarket Analysis - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/market-analysis/intermarket-analysis); [Trading with Intermarket Analysis - Wiley](https://www.wiley-vch.de/de/fachgebiete/finanzen-wirtschaft-recht/trading-with-intermarket-analysis-978-1-119-21001-6)

## Cụm 2. Chỉ báo kỹ thuật

### Đường trung bình động (SMA, EMA), MA 50 và MA 200, giao cắt vàng, giao cắt tử thần

**Thầy nhắc ở:** B4 01:41, B7 03:47, B9 01:47, B9 03:08, B10 00:26, B10 00:27, B11 01:21 - học viên nêu MA là công cụ kiểm tra đầu tiên; thầy cho rằng tham số không có ý nghĩa tự thân và đặt câu tự kiểm tra về SMA20.

**Là gì:** Đường trung bình động là đường nối giá trị trung bình của N phiên gần nhất, được tính lại mỗi phiên để làm mượt giá. SMA là trung bình cộng đơn giản; EMA là trung bình luỹ thừa, đặt trọng số lớn hơn cho giá gần.

**Giải thích:** SMA(N) = tổng giá đóng cửa N phiên gần nhất chia N. Khi sang phiên mới, SMA đổi theo công thức: SMA mới = SMA cũ + (giá mới - giá cũ nhất vừa rời cửa sổ) / N. Nghĩa là SMA đổi không chỉ vì giá hôm nay mà còn vì giá cách đây N phiên bị loại ra; đó là lý do một đường SMA có thể rẽ hướng khi giá hôm nay không có gì đặc biệt. EMA: EMA hôm nay = alpha x giá hôm nay + (1 - alpha) x EMA hôm qua, với alpha = 2 / (N + 1). Mọi đường trung bình đều trễ: SMA trễ khoảng một nửa độ rộng cửa sổ so với giá mới nhất. Các số 50 và 200 phiên là quy ước phổ biến chứ không có cơ sở lý thuyết riêng. "Giao cắt vàng" (golden cross) là khi MA50 cắt lên trên MA200; "giao cắt tử thần" (death cross) là khi MA50 cắt xuống dưới MA200. Bằng chứng: CXO Advisory khảo sát Dow Jones và S&P 500 từ 1928 đến 2017 thấy lợi suất 126 phiên sau hai loại tín hiệu chênh nhau không rõ ràng (với Dow là 2,8% sau death cross và 2,3% sau golden cross; với S&P 500 là 3,8% và 6,4%). Kết luận chung của các nguồn: các tín hiệu này mô tả xu hướng hiện có hơn là dự báo lợi suất. Đây là kết quả từ tổng hợp của một trang nghiên cứu độc lập, chưa phải bài tạp chí bình duyệt.

**Liên hệ với bài học:** Thầy nói tham số 12, 50, 200 không mang ý nghĩa tự thân: đổi 20 thành 21 là ra tín hiệu khác. Hiểu biết phổ thông dùng chúng như tín hiệu mua bán; thầy coi đó là cách đọc quá khứ chứ không phải nguyên nhân của giá.

**Đọc thêm:** [Moving average - Wikipedia](https://en.wikipedia.org/wiki/Moving_average); [U.S. stock market death crosses and golden crosses - CXO Advisory](https://www.cxoadvisory.com/technical-trading/u-s-stock-market-death-crosses-and-golden-crosses/); [Are golden and death crosses a good bet - FactSet](https://insight.factset.com/are-golden-and-death-crosses-a-good-bet)

### MACD (Moving Average Convergence Divergence)

**Thầy nhắc ở:** B4 02:47, B4 02:48, B7 03:47, B9 03:08, B13 03:13, B15 00:01 - thầy nói MACD làm rối mắt; học viên từng đợi tín hiệu MACD mới mua.

**Là gì:** MACD là chỉ báo do Gerald Appel phát triển cuối thập niên 1970, đo sự hội tụ và phân kỳ giữa hai đường EMA, dùng để nhận ra thay đổi sức mạnh và hướng của xu hướng.

**Giải thích:** Công thức chuẩn: đường MACD = EMA12 của giá đóng cửa trừ EMA26. Đường tín hiệu = EMA9 của đường MACD. Biểu đồ cột (histogram) = đường MACD trừ đường tín hiệu. Cách đọc: MACD cắt lên đường tín hiệu thường được coi là tín hiệu tăng, cắt xuống là tín hiệu giảm; MACD cắt qua mức 0 xác nhận đổi hướng nhưng chậm hơn. Phân kỳ: giá lập đáy mới mà MACD không lập đáy mới là phân kỳ dương; giá lập đỉnh mới mà MACD không lập đỉnh mới là phân kỳ âm. Vì tính từ các đường trung bình nên MACD luôn trễ so với giá, hoạt động kém khi thị trường đi ngang, và các giao cắt có thể là tín hiệu sai. Đòi hỏi xác nhận thêm (ví dụ MACD nằm trên đường tín hiệu ba phiên) làm giảm tín hiệu sai nhưng cũng làm lỡ lợi nhuận.

**Liên hệ với bài học:** Cái "trễ" chính là lý do thầy cho rằng chờ MACD báo mua thì thường đã muộn so với người gom. Học viên coi MACD là bước kiểm tra đầu tiên; thầy coi nó chỉ là phép biến đổi của giá, không chứa thông tin mới.

**Đọc thêm:** [MACD - Wikipedia](https://en.wikipedia.org/wiki/MACD)

### Chỉ báo dao động và quá mua quá bán (RSI, Stochastic, CCI)

**Thầy nhắc ở:** B4 02:47, B7 03:47, B9 01:47, B10 02:00, B13 03:13, B15 00:01 - thầy chê tín hiệu quá mua xuất hiện sớm, RSI vùng 50 và 70 làm ví dụ đọc ngưỡng đơn lẻ.

**Là gì:** Chỉ báo dao động là các chỉ báo chạy lên xuống quanh một khoảng giới hạn, dùng để đánh giá giá đang "nóng" (quá mua) hay "nguội" (quá bán) so với các phiên gần đây.

**Giải thích:** RSI (Relative Strength Index) do J. Welles Wilder đưa ra năm 1978 trong sách "New Concepts in Technical Trading Systems". Với chu kỳ mặc định 14: tính mức tăng trung bình và mức giảm trung bình của giá đóng cửa theo kiểu làm mượt của Wilder, RS = mức tăng trung bình / mức giảm trung bình, RSI = 100 - 100 / (1 + RS). Quy ước: trên 70 là quá mua, dưới 30 là quá bán, 50 là đường giữa; một số người dùng 80 và 20 cho xu hướng mạnh. Stochastic của George Lane (cuối thập niên 1950): %K = (giá đóng cửa - đáy N phiên) / (đỉnh N phiên - đáy N phiên) x 100, thường N = 14; %D là trung bình 3 phiên của %K. CCI do Donald Lambert đưa ra năm 1980: lấy giá điển hình (cao + thấp + đóng cửa) / 3, trừ đi trung bình động của nó, chia cho độ lệch tuyệt đối trung bình, rồi nhân 1/0,015; các mức +100 và -100 là ngưỡng thường dùng. Điểm yếu: trong xu hướng mạnh, RSI có thể ở vùng "quá mua" rất lâu trong khi giá vẫn tăng, nên đọc ngưỡng đơn lẻ dễ cho tín hiệu sớm. Một nghiên cứu (Marek và Šedivá, 2017) thấy RSI với thiết lập chuẩn cho kết quả tốt trong thử nghiệm nhưng trong thời gian dài thường thua chiến lược mua và giữ.

**Liên hệ với bài học:** Thầy lấy RSI làm ví dụ cho việc gắn nhãn tín hiệu theo một con số: "RSI trên 70 là quá mua" là quy ước, không phải quy luật. Hiểu biết phổ thông dùng ngưỡng như tín hiệu bán; thầy chỉ ra tín hiệu thường đến sớm.

**Đọc thêm:** [Relative strength index - Wikipedia](https://en.wikipedia.org/wiki/Relative_strength_index); [Stochastic oscillator - Wikipedia](https://en.wikipedia.org/wiki/Stochastic_oscillator); [Commodity channel index - Wikipedia](https://en.wikipedia.org/wiki/Commodity_channel_index)

### Bollinger Bands, Parabolic SAR, ADX, Chaikin Money Flow và các nhóm chỉ báo xu hướng, động lượng, biến động

**Thầy nhắc ở:** B4 01:41, B7 03:51, B9 01:47, B10 02:01, B12 03:01 - tên trong báo cáo scan và trang mẫu; học viên dùng lọc mã, thầy nhắc để phê bình việc học công cụ rời rạc; thầy dùng "phương trình parabol" làm lớp xác nhận.

**Là gì:** Các chỉ báo thường được chia nhóm: xu hướng (đường trung bình động, Parabolic SAR, ADX), động lượng (RSI, Stochastic, MACD), biến động (Bollinger Bands, ATR), khối lượng (Chaikin Money Flow).

**Giải thích:**
- Bollinger Bands (John Bollinger, thập niên 1980): dải giữa là SMA 20 phiên, dải trên và dải dưới cách dải giữa 2 lần độ lệch chuẩn 20 phiên. Dải hẹp báo hiệu biến động thấp (thường gọi là "squeeze"), dải rộng báo hiệu biến động cao. Thực tế giá nằm trong dải ít hơn mức 95% kỳ vọng nếu phân phối chuẩn; các nghiên cứu báo cáo khoảng 85-90%.
- Parabolic SAR (Wilder, 1978): SAR kế tiếp = SAR + AF x (EP - SAR), với EP là điểm cực trị của xu hướng, AF bắt đầu 0,02, tăng 0,02 mỗi lần có cực trị mới, tối đa 0,20. Giá cắt SAR thì xu hướng đảo chiều và AF về 0,02. Dùng làm điểm dừng lỗ bám theo; nhiều tín hiệu sai khi thị trường đi ngang.
- ADX (Wilder, 1978): đo độ MẠNH của xu hướng, không đo hướng. Tính từ +DI và -DI (chu kỳ 14); dưới 20 coi là xu hướng yếu, trên 40 là mạnh.
- Chaikin Money Flow (Marc Chaikin): hệ số dòng tiền = [(đóng cửa - thấp nhất) - (cao nhất - đóng cửa)] / (cao nhất - thấp nhất); CMF 20 hoặc 21 phiên = tổng (hệ số x khối lượng) / tổng khối lượng. Dương nghiêng về lực mua, âm nghiêng về lực bán, thường dao động giữa -0,5 và +0,5.

**Liên hệ với bài học:** Thầy dùng các tên này như ví dụ về "học công cụ rời rạc": biết công thức từng chỉ báo không giúp hiểu ai đang gom hay xả. Các chỉ báo này đều là hàm của giá và khối lượng đã xảy ra.

**Đọc thêm:** [Bollinger Bands - Wikipedia](https://en.wikipedia.org/wiki/Bollinger_Bands); [Parabolic SAR - Wikipedia](https://en.wikipedia.org/wiki/Parabolic_SAR); [Average directional movement index - Wikipedia](https://en.wikipedia.org/wiki/Average_directional_movement_index); [Chaikin Money Flow - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/technical-indicators-and-overlays/technical-indicators/chaikin-money-flow-cmf)

### Ichimoku Kinko Hyo (vùng mây)

**Thầy nhắc ở:** B4 02:30, B9 01:47, B9 02:55, B10 01:00 - thầy nhắc tên như một trường phái; hình mã APS có vùng mây kéo sang phải.

**Là gì:** Ichimoku Kinko Hyo ("biểu đồ cân bằng một cái nhìn") là hệ thống chỉ báo từ Nhật Bản, do nhà báo Goichi Hosoda (bút danh Ichimoku Sanjin) phát triển, công bố cuối thập niên 1960 sau khoảng 30 năm hoàn thiện.

**Giải thích:** Gồm năm đường, đều tính từ trung điểm giữa đỉnh cao nhất và đáy thấp nhất: Tenkan-sen (đường chuyển đổi) trên 9 phiên; Kijun-sen (đường cơ sở) trên 26 phiên; Senkou Span A là trung bình của hai đường trên, vẽ lệch về phía trước 26 phiên; Senkou Span B là trung điểm 52 phiên, cũng vẽ lệch 26 phiên; Chikou Span là giá đóng cửa hôm nay vẽ lùi 26 phiên. Vùng giữa Span A và Span B là "mây" (kumo). Cách đọc phổ biến: giá nằm trên mây là thuận lợi, trong mây là trung tính, dưới mây là nghiêng giảm; Span A trên Span B là mây tăng; mây dày được coi là hỗ trợ kháng cự mạnh hơn. Vì mây vẽ lệch về tương lai nên hình ảnh có vẻ "dự báo", nhưng thực chất 26 phiên phía trước chỉ là phép tính từ dữ liệu quá khứ. Tài liệu tra cứu không đưa ra bằng chứng thống kê rằng hệ thống này có hiệu quả dự báo.

**Liên hệ với bài học:** Thầy xếp Ichimoku vào nhóm "trường phái" công cụ chồng lên giá. Phần mây kéo sang phải trong hình mã APS dễ khiến người học tưởng là dự báo, trong khi nó là phép dịch chuyển của dữ liệu đã có.

**Đọc thêm:** [Ichimoku Kinko Hyo - Wikipedia](https://en.wikipedia.org/wiki/Ichimoku_Kink%C5%8D_Hy%C5%8D)

### Momentum, giao dịch tần suất cao (HFT) và scalping

**Thầy nhắc ở:** B10 02:12 - thầy xếp là nhóm phương pháp tệ nhất (thầy gộp chung động lượng với giao dịch rất ngắn).

**Là gì:** Ba khái niệm khác nhau. Momentum (động lượng) trong tài chính là xu hướng quan sát được rằng cổ phiếu tăng mạnh gần đây có xu hướng tiếp tục tăng, giảm mạnh thì tiếp tục giảm. Giao dịch tần suất cao (HFT) là giao dịch thuật toán tốc độ rất cao, mở và đóng vị thế trong vài giây hoặc phần nghìn giây. Scalping là mở đóng vị thế trong vài phút hoặc vài giây để ăn chênh lệch giá rất nhỏ.

**Giải thích:** Momentum trong học thuật được xem là một "dị thường" thị trường: các nghiên cứu ghi nhận cổ phiếu thắng tiếp tục vượt trội, với mức vượt khoảng 1% mỗi tháng trong một số mẫu; giải thích hay gặp là nhà đầu tư phản ứng chậm với thông tin. Cần phân biệt: momentum kiểu học thuật đo trên khung vài tháng, còn momentum trong ngôn ngữ giao dịch hằng ngày thường là bắt nhịp ngắn hạn. HFT chủ yếu là việc của các công ty chuyên nghiệp có hạ tầng đặt máy gần sàn (co-location), từng chiếm khoảng 10-40% khối lượng cổ phiếu Mỹ theo ước tính năm 2016. Scalping bán lẻ thì chịu chi phí giao dịch và chênh lệch mua bán ăn mòn lợi nhuận nhỏ mỗi lệnh. Lưu ý: "scalping" cũng là tên của một hành vi gian lận khi nhà tư vấn mua cổ phiếu trước rồi khuyến nghị cho khách (nghĩa khác).

**Liên hệ với bài học:** Thầy gộp chung động lượng với giao dịch cực ngắn và coi là nhóm phương pháp tệ. Cách dùng này khác với văn liệu học thuật, nơi momentum là một chiến lược khung tháng có bằng chứng thực nghiệm nhưng cũng có rủi ro sụp đổ.

**Đọc thêm:** [Momentum (finance) - Wikipedia](https://en.wikipedia.org/wiki/Momentum_(finance)); [High-frequency trading - Wikipedia](https://en.wikipedia.org/wiki/High-frequency_trading); [Scalping (trading) - Wikipedia](https://en.wikipedia.org/wiki/Scalping_(trading))

## Cụm 3. Fibonacci, sóng Elliott, fractal

### Leonardo Fibonacci và dãy số Fibonacci (Liber Abaci, bài toán thỏ)

**Thầy nhắc ở:** B2 02:06, B3 00:48, B10 00:48, B10 00:50, B11 00:56 - thầy nói đây là quy luật tự nhiên có tính đệ quy, giới thiệu nhà toán học Ý.

**Là gì:** Dãy Fibonacci bắt đầu 0, 1 rồi mỗi số bằng tổng hai số liền trước: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144... Tên gọi lấy theo Leonardo xứ Pisa (khoảng 1170 đến khoảng 1240-1250), thường gọi là Fibonacci.

**Giải thích:** Fibonacci sinh ra khoảng năm 1170, cha là Guglielmo, một thương nhân kiêm quan chức hải quan phụ trách trạm buôn ở Bugia (nay là Béjaïa, Algeria), nên ông tiếp xúc với số học của người Ả Rập từ sớm. Năm 1202 ông xuất bản "Liber Abaci", cuốn sách đưa hệ số thập phân Ấn-Ả Rập (chữ số 0-9 với giá trị theo vị trí) vào châu Âu, thay dần chữ số La Mã. Trong sách có bài toán thỏ: một cặp thỏ mới sinh, mỗi cặp bắt đầu sinh sản khi một tháng tuổi và đẻ một cặp mới sau mỗi tháng tiếp theo, thỏ không chết; số cặp thỏ cuối mỗi tháng chính là các số của dãy trên. Cái tên "dãy Fibonacci" do nhà toán học Pháp Édouard Lucas đặt năm 1876. Tỷ số hai số liên tiếp tiến dần về tỷ lệ vàng khoảng 1,618 (nghịch đảo là 0,618); công thức đóng gọi là công thức Binet. Dãy xuất hiện ở một số hiện tượng sinh học (cách xếp lá, hạt thông, hoa cúc) nhưng không phải ở mọi loài; nhiều khẳng định "tỷ lệ vàng có ở khắp nơi" trong nghệ thuật và tự nhiên bị giới nghiên cứu coi là sai hoặc gán ghép. Liên quan tới hằng số e hay pi: các nguồn tra cứu chỉ nêu mối liên hệ với tỷ lệ vàng, không nêu liên hệ trực tiếp với e hay pi.

**Liên hệ với bài học:** Thầy nhắc dãy Fibonacci như bằng chứng của quy luật tự nhiên để dẫn sang tỷ lệ 0,618 và 1,618 trong thị trường. Phần toán thì chắc chắn; bước nhảy từ "dãy số có trong tự nhiên" sang "giá chứng khoán tôn trọng các tỷ lệ này" là giả thuyết, và các mục tiếp theo nêu bằng chứng.

**Đọc thêm:** [Fibonacci sequence - Wikipedia](https://en.wikipedia.org/wiki/Fibonacci_sequence); [Leonardo Pisano Fibonacci - MacTutor](https://mathshistory.st-andrews.ac.uk/Biographies/Fibonacci/); [Golden ratio - Wikipedia](https://en.wikipedia.org/wiki/Golden_ratio)

### Các mức Fibonacci thoái lui và mở rộng (0,236; 0,382; 0,5; 0,618; 1,618; 2,618)

**Thầy nhắc ở:** B2 02:06, B3 00:48, B10 02:09, B11 00:52, B11 02:21, B15 00:43 - thầy kéo Fibonacci từ đoạn gom ra các điểm mục tiêu, bác cách coi 38,2% là hỗ trợ, bác việc thời gian gom đẩy xả theo tỷ lệ phi, nhắc như ngưỡng người ta liều bắt đáy lần hai.

**Là gì:** Fibonacci thoái lui (retracement) là công cụ vẽ các mức phần trăm của một nhịp tăng hoặc giảm trước đó (23,6%; 38,2%; 50%; 61,8%; 78,6%) để dự đoán giá có thể hồi về đâu. Fibonacci mở rộng (extension) là các mức vượt quá nhịp ban đầu (161,8%; 261,8%) dùng làm mục tiêu giá.

**Giải thích:** Cách vẽ: chọn hai điểm là đáy swing và đỉnh swing của nhịp cần đo (xu hướng lên: từ đáy đến đỉnh; xu hướng xuống: từ đỉnh đến đáy). Mỗi mức = đỉnh trừ (tỷ lệ x độ dài nhịp). Ví dụ giá tăng từ 100 lên 150 (độ dài 50): mức 23,6% ở 138,2; 38,2% ở 130,9; 50% ở 125,0; 61,8% ở 119,1. Nguồn gốc các tỷ lệ: 61,8% là tỷ số một số Fibonacci với số kế tiếp (ví dụ 89/144); 38,2% là tỷ số với số cách hai bậc (89/233); 23,6% với số cách ba bậc (89/377). Mức 50% không thuộc dãy Fibonacci mà bắt nguồn từ quan sát của lý thuyết Dow rằng chỉ số hay hồi về một nửa nhịp trước. Điểm yếu: việc chọn hai điểm đầu cuối mang tính chủ quan, nên hai người vẽ ra hai bộ mức khác nhau; với nhiều mức gần nhau, giá chạm một mức nào đó gần như là điều chắc chắn. Về bằng chứng: tra cứu không tìm thấy nghiên cứu bình duyệt xác nhận các mức Fibonacci có sức dự báo; một nghiên cứu của Batchelor và Ramyar trên chỉ số Dow Jones (được trích trong Wikipedia) không thấy tần suất các tỷ lệ giá và thời gian khác với dữ liệu ngẫu nhiên. Bằng chứng tích cực hơn thuộc về hỗ trợ kháng cự nói chung (Osler), không riêng Fibonacci.

**Liên hệ với bài học:** Thầy dùng Fibonacci mở rộng để đặt mục tiêu từ đoạn gom, nhưng bác hai cách dùng phổ biến: coi 38,2% là hỗ trợ cứng và bắt tỷ lệ phi vào thời gian gom, đẩy, xả. Điều này khớp với bằng chứng: mức Fibonacci chỉ là điểm quy chiếu, không phải quy luật.

**Đọc thêm:** [Fibonacci retracements - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/chart-analysis/fibonacci-retracements); [Fibonacci retracement - BabyPips](https://www.babypips.com/school/fibonacci-retracement.html); [Elliott wave principle - Wikipedia](https://en.wikipedia.org/wiki/Elliott_wave_principle)

### Fibonacci Time Zone, đường chu kỳ, quạt Fibonacci và cung Gann

**Thầy nhắc ở:** B2 02:06, B3 00:48, B10 00:51, B10 01:07, B10 02:17, B10 02:20 - công cụ trong menu TradingView thầy mở, dùng chiếu chu kỳ từ đoạn tích luỹ; lưới hai trục thời gian và giá.

**Là gì:** Nhóm công cụ vẽ ra biểu đồ các đường hoặc cung theo tỷ lệ Fibonacci hay góc Gann để ước lượng thời điểm hoặc mức giá có thể đổi hướng.

**Giải thích:** Fibonacci Time Zones: các đường dọc cách điểm gốc theo khoảng cách 1, 2, 3, 5, 8, 13, 21, 34... đơn vị thời gian, gốc đặt tại một điểm swing quan trọng. Đường chu kỳ (Cycle Lines) khác ở chỗ khoảng cách giữa các đường bằng nhau, không theo dãy Fibonacci. Quạt Fibonacci: kẻ một đường xu hướng giữa hai điểm swing rồi từ điểm đầu kẻ các tia đi qua các mức 38,2%; 50%; 61,8% của đoạn thẳng đứng tại điểm cuối. Cung Fibonacci có bán kính bằng 38,2%; 50%; 61,8% khoảng cách giữa hai điểm, tâm đặt ở điểm đầu, và hình dạng cung phụ thuộc tỷ lệ trục của biểu đồ. Quạt Gann gồm các đường góc đi qua điểm gốc theo tỷ lệ thời gian trên giá (1x1, 2x1, 1x2...), trong đó đường 1x1 tương ứng 45 độ được coi là quan trọng nhất, nên phải cài tỷ lệ trục cho đúng. W. D. Gann có những khẳng định về chu kỳ hình học của thị trường; các nguồn phổ thông thừa nhận cả Gann lẫn Elliott đều dễ khớp với dữ liệu quá khứ và không có bằng chứng chặt chẽ về sức dự báo. Không tìm được số liệu tỷ lệ thành công đáng tin cho Fibonacci Time Zones.

**Liên hệ với bài học:** Thầy mở các công cụ này trong menu TradingView để cho người học thấy chúng làm được gì, rồi dùng chu kỳ chiếu từ đoạn tích luỹ như một cách tham khảo, không phải lịch hẹn của thị trường.

**Đọc thêm:** [Fib Time Tools - LuxAlgo](https://www.luxalgo.com/library/concept/fib-time-tools.md); [Fibonacci Time Zones - The Right Trader](https://therighttrader.com/learn/fibonacci-and-drawing-tools/fibonacci-time-zones); [Gann angles - Wikipedia](https://wikipedia.com/wiki/Gann_angles); [How can I draw Fibonacci fan lines - StockCharts](https://stockcharts.com/articles/mailbag/2012/10/how-can-i-draw-fibonacci-fan-lines.html)

### Lý thuyết sóng Elliott (Elliott Wave) và tiểu sử Ralph Nelson Elliott

**Thầy nhắc ở:** B2 02:05, B2 03:13, B3 00:48, B9 01:47, B10 00:21, B10 00:52, B11 01:19, B11 01:58, B11 02:36 - thầy chiếu sơ đồ 5 sóng đẩy 3 sóng điều chỉnh và các số 3, 5, 13, 21, 55, 89; cho rằng đếm sóng dễ mắc bẫy, chê dùng máy móc.

**Là gì:** Lý thuyết sóng Elliott cho rằng giá thị trường vận động theo chu kỳ lặp lại, mỗi chu kỳ gồm 5 sóng đẩy (đánh số 1-2-3-4-5) theo hướng xu hướng chính và 3 sóng điều chỉnh (A-B-C) ngược hướng, và các sóng này lồng vào nhau ở nhiều cấp độ.

**Giải thích:** Ralph Nelson Elliott (1871-1948), một kế toán người Mỹ, phát triển lý thuyết từ việc nghiên cứu dữ liệu thị trường chứng khoán. Ông trình bày với Charles J. Collins ở Detroit; hai người cùng viết cuốn sách "The Wave Principle", xuất bản ngày 31/8/1938; năm 1939 ông viết loạt 12 bài cho tạp chí Financial World. Robert Prechter sau này phổ biến lý thuyết qua sách "Elliott Wave Principle" viết cùng A. J. Frost. Ba quy tắc "bất khả xâm phạm" cho sóng đẩy: sóng 2 không hồi quá điểm bắt đầu của sóng 1; sóng 3 không bao giờ là sóng ngắn nhất trong ba sóng 1, 3, 5; sóng 4 không đi vào vùng giá của sóng 1. Các sóng điều chỉnh gồm nhiều dạng: zigzag (A-B-C sắc nét), flat (đi ngang, sóng B hồi ít nhất khoảng 90% sóng A), tam giác (năm sóng con A-E; sóng 4 có thể là tam giác, sóng 2 thì không). Các nguyên tắc hướng dẫn: sóng 2 thường hồi không quá 61,8% sóng 1; sóng 4 thường hồi dưới 38,2% sóng 3; sóng 3 thường dài khoảng 1,618 lần sóng 1; sóng C thường bằng hoặc dài hơn sóng A. Elliott coi dãy Fibonacci là nền tảng: 5 sóng đẩy, 8 sóng một chu kỳ, các cấp sóng con lên tới 55 và 89 sóng. Cấp độ sóng đi từ Grand Supercycle xuống Subminuette. Phê bình: tính chủ quan (hai người đếm cùng một biểu đồ ra hai kết quả khác nhau, sóng bị đếm lại khi dự báo sai), khó bác bỏ, và David Aronson gọi nó là "một câu chuyện" hơn là lý thuyết. Mandelbrot gọi dự báo bằng sóng là "một nghệ thuật" với thành tích "tốt nhất là hỗn hợp". Nghiên cứu của Batchelor và Ramyar trên Dow Jones không thấy các tỷ lệ Fibonacci xuất hiện khác ngẫu nhiên. Những người ủng hộ coi lý thuyết là khung mô tả cấu trúc và quản trị rủi ro hơn là công cụ dự báo chính xác.

**Liên hệ với bài học:** Các số 3, 5, 13, 21, 55, 89 thầy chiếu chính là dãy Fibonacci mà Elliott gắn với số sóng. Thầy cảnh báo đếm sóng dễ mắc bẫy, khớp với phê bình học thuật: cùng một chuyển động có thể đếm theo nhiều cách. Sơ đồ 5 sóng đẩy 3 sóng điều chỉnh cũng gần với chu trình đè, gom, đẩy, xả của thầy, nhưng thầy bàn nó theo hành vi người chơi chứ không theo tỷ lệ toán học.

**Đọc thêm:** [Elliott wave principle - Wikipedia](https://en.wikipedia.org/wiki/Elliott_wave_principle); [Ralph Nelson Elliott - Wikipedia](https://en.wikipedia.org/wiki/Ralph_Nelson_Elliott); [Corrective waves - BabyPips](https://www.babypips.com/learn/forex/corrective-waves); [Elliott Wave Theory - CMC Markets](https://cmcmarkets.com/en-sg/trading-guides/elliott-wave-theory)

### Fractal, tự đồng dạng và sóng lồng sóng (Mandelbrot, búp bê Nga)

**Thầy nhắc ở:** B2 02:11, B11 01:00, B11 01:20 - thầy gọi là nguyên lý nén để giảm nhiễu; dùng từ "đệ quy" và ẩn dụ búp bê Nga cho sóng lồng sóng.

**Là gì:** Fractal là hình hoặc quá trình có tính tự đồng dạng: nhìn ở thang nhỏ hay thang lớn đều thấy cấu trúc na ná nhau. Benoit Mandelbrot đưa ý tưởng này vào tài chính, cho rằng biến động giá có cấu trúc fractal.

**Giải thích:** Trong sách "The (Mis)behavior of Markets" (viết cùng Richard Hudson), Mandelbrot lập luận rằng mô hình phân phối chuẩn đánh giá thấp rủi ro cực đoan. Ông nêu hai hiệu ứng: "hiệu ứng Noah" (những cú nhảy giá đột ngột) và "hiệu ứng Joseph" (phụ thuộc dài hạn, xu hướng kéo dài), và đề xuất mô hình đa fractal (multifractal) có tính đến nhịp biến động thay đổi theo thời gian. Khi vẽ biến động giá trên trục logarit, người ta quan sát được độ dốc nhất quán gợi ý tự đồng dạng giữa các thang thời gian. Trong phân tích kỹ thuật, ý tưởng này được dùng theo hai hướng: nhìn đa khung thời gian (một nhịp tăng ở khung ngày gồm nhiều nhịp con ở khung giờ) và hình dung sóng lồng sóng như Elliott. Cần phân biệt: Mandelbrot dùng fractal để phê phán các mô hình rủi ro chuẩn, không phải để cung cấp quy tắc đếm sóng; chính ông cũng phê bình tính chủ quan của sóng Elliott.

**Liên hệ với bài học:** Thầy dùng ẩn dụ búp bê Nga để nói rằng trong một nhịp lớn có nhịp nhỏ cùng kiểu, nên cùng một logic đè, gom, đẩy, xả lặp lại ở mọi khung. Việc "nén" khung thời gian để bớt nhiễu là cách đọc đa khung, khác với chứng minh toán học về fractal.

**Đọc thêm:** [The Misbehavior of Markets - Hachette](https://www.hachettebookgroup.com/titles/benoit-mandelbrot/the-misbehavior-of-markets/9780465043576/); [The (Mis)behavior of Markets - Danny Yee](https://dannyreviews.com/h/Misbehavior_Markets.html); [Elliott wave principle - Wikipedia](https://en.wikipedia.org/wiki/Elliott_wave_principle)

## Cụm 4. Mẫu hình giá, nến Nhật, price action

### Mẫu hình giá đảo chiều (vai đầu vai, vai đầu vai ngược, cốc tay cầm) và sách "Encyclopedia of Chart Patterns"

**Thầy nhắc ở:** B4 01:30, B10 00:40, B10 00:45, B10 02:42, B11 01:55, B13 03:23, B15 00:01 - thầy nói vai đầu vai là hình do người đè gom vẽ cho thị trường, cùng một quá trình đè gom xả; nhắc hình dáng vai và đầu khi nói phân phối; học viên lấy cốc tay cầm làm ví dụ mẫu tay to "vẽ".

**Là gì:** Mẫu hình đảo chiều là hình dạng đường giá được cho là báo hiệu xu hướng sắp đổi chiều. Vai đầu vai (head and shoulders) gồm vai trái, đầu cao hơn, vai phải thấp hơn đầu, với đường viền cổ (neckline) nối các đáy. Vai đầu vai ngược là phiên bản lật ngược, báo hiệu đảo chiều từ giảm sang tăng. Cốc tay cầm (cup and handle) là hình cái cốc kèm quai nhỏ, thường được coi là mẫu hình tiếp diễn tăng.

**Giải thích:**
- Vai đầu vai: chỉ coi là hoàn thành khi giá phá thủng đường viền cổ; sau đó giá thường quay lại thử đường viền cổ trước khi đi tiếp. Mục tiêu giá tối thiểu thường đo bằng khoảng cách từ đỉnh đầu xuống đường viền cổ, chiếu xuống từ điểm phá vỡ. Khối lượng thường cao nhất ở vai trái và thấp dần ở vai phải. Hình thực tế hiếm khi cân đối; đường viền cổ có thể dốc. Mẫu hình đáy thường mất nhiều tháng, đỉnh thường vài tuần. Phiên bản "phân phối kiểu Wyckoff" có đầu và hai vai trái, vai phải yếu hơn.
- Cốc tay cầm: được William J. O'Neil, người sáng lập Investor's Business Daily, phổ biến trong sách "How to Make Money in Stocks" (1988). Điểm mua theo O'Neil là đỉnh của tay cầm cộng một biên nhỏ, không phải mép phải của cốc; khối lượng khi vượt thường cao hơn trung bình khoảng 40-50%; độ sâu tay cầm thường được nêu khoảng 8-12% hoặc khoảng một phần ba độ sâu cốc (các nguồn lệch nhau); cắt lỗ phổ biến 7-8% dưới điểm mua theo phương pháp của ông.
- Sách "Encyclopedia of Chart Patterns" của Thomas Bulkowski (Wiley, bản thứ ba năm 2021) thống kê hiệu suất và tỷ lệ thất bại của rất nhiều mẫu hình. Bảng xếp hạng trên thepatternsite.com (cập nhật ngày 24/08/2020) xếp cốc tay cầm ở nhóm tốt (hạng 3 và 2 trong hai cột; tôi không xác nhận được cột nào là hiệu suất, cột nào là tỷ lệ thất bại) và vai đầu vai đáy ở hạng 13 và 10. Số liệu của Bulkowski dựa trên quy tắc nhận diện của chính ông nên khó lặp lại một cách khách quan.

**Liên hệ với bài học:** Thầy nói các hình này không phải quy luật tự nhiên mà là kết quả của quá trình đè, gom, xả: hình vai đầu vai là dấu vết của phân phối. Hiểu biết phổ thông dạy "thấy vai đầu vai thì bán"; thầy đảo ngược nhân quả: hình sinh ra từ hành vi, nên cần hiểu hành vi thay vì thuộc hình.

**Đọc thêm:** [Head and shoulders (chart pattern) - Wikipedia](https://en.wikipedia.org/wiki/Head_and_shoulders_(chart_pattern)); [Cup With Handle - Fidelity](https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/cup-with-handle); [Chart pattern rank - Bulkowski, thepatternsite.com](https://www.thepatternsite.com/id73.html); [Encyclopedia of Chart Patterns - Wiley](https://www.wiley-vch.de/en/areas-interest/finance-economics-law/encyclopedia-of-chart-patterns-978-1-119-73968-5)

### Mẫu hình tiếp diễn (tam giác, nêm, cờ, cờ đuôi nheo, chữ nhật, ABCD)

**Thầy nhắc ở:** B10 00:51, B10 01:07, B11 01:50, B11 01:58 - slide nêu hình và nhãn bullish, bearish; có trong menu công cụ.

**Là gì:** Mẫu hình tiếp diễn là các giai đoạn giá đi ngang hoặc thu hẹp ngắn, sau đó được kỳ vọng tiếp tục theo hướng xu hướng trước đó.

**Giải thích:** Theo StockCharts ChartSchool: cờ (flag) và cờ đuôi nheo (pennant) thường kéo dài một đến bốn tuần; cờ quá 12 tuần thì xếp thành hình chữ nhật, cờ đuôi nheo quá 12 tuần thành tam giác cân. Cách đo mục tiêu giá: với cờ và cờ đuôi nheo, lấy độ dài "cán cờ" (nhịp đi mạnh trước đó) chiếu từ điểm phá vỡ; với chữ nhật, lấy chiều cao hình chữ nhật chiếu từ điểm phá vỡ; với tam giác, lấy bề rộng lớn nhất của tam giác. Vai trò khối lượng: thường co lại khi hình đang hình thành và tăng lên khi phá vỡ. ABCD là mẫu hình gồm bốn điểm, hai đoạn AB và CD thường bằng nhau về độ dài và thời gian; nó là nền của mẫu hình hài hoà Gartley (H. M. Gartley, "Profits in the Stock Market", 1935), sau này Scott Carney và Larry Pesavento gắn thêm các tỷ lệ Fibonacci. Mục tiêu đo từ hình học chỉ là mốc tham chiếu, không phải đích đến chắc chắn, và nên điều chỉnh nếu có vùng hỗ trợ kháng cự lớn nằm gần hơn. Muốn biết tỷ lệ thành công theo Bulkowski thì cần xem sách của ông, tra cứu này không tìm được bảng số liệu đáng tin cho từng mẫu hình.

**Liên hệ với bài học:** Các nhãn "bullish", "bearish" trên slide chỉ là cách phân loại hình theo giá; thầy dùng chúng để cho thấy phân tích kỹ thuật chia nhỏ một hiện tượng thành nhiều tên gọi.

**Đọc thêm:** [Flag and pennant - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/chart-analysis/chart-patterns/flag-pennant); [Rectangle - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/chart-analysis/chart-patterns/rectangle); [Harmonic patterns - StockCharts ChartSchool](https://chartschool.stockcharts.com/table-of-contents/trading-strategies-and-models/trading-strategies/harmonic-patterns); [The Gartley and the animals - BabyPips](https://www.babypips.com/learn/forex/the-gartley-and-the-animals)

### Mark Minervini, SEPA và VCP

**Thầy nhắc ở:** B4 01:30, B4 03:18 - học viên đọc sách Minervini để lọc mẫu nền giá, lấy cốc tay cầm làm ví dụ mẫu tay to "vẽ".

**Là gì:** Mark Minervini là nhà giao dịch cổ phiếu Mỹ, tác giả sách "Trade Like a Stock Market Wizard". Phương pháp của ông gọi là SEPA (Specific Entry Point Analysis, phân tích điểm vào lệnh cụ thể), trong đó VCP (Volatility Contraction Pattern, mẫu hình co hẹp biến động) là phần chọn điểm vào.

**Giải thích:** Theo các nguồn thứ cấp: SEPA bắt đầu bằng "Trend Template", danh sách tám điều kiện kỹ thuật để chọn cổ phiếu đang ở giai đoạn tăng (Stage 2), kết hợp lọc cơ bản và xếp hạng sức mạnh tương đối kiểu IBD. Với cổ phiếu qua được bộ lọc, VCP là nền giá mà biên độ dao động thu hẹp dần qua các nhịp, kèm khối lượng cạn dần, rồi mua khi giá vượt điểm pivot hẹp. Tôi chưa tìm được đoạn trích sách gốc nên chi tiết các điều kiện và con số nên đối chiếu với sách. Không nên coi lời quảng bá về thành tích của tác giả là bằng chứng độc lập.

**Liên hệ với bài học:** Học viên dùng sách này để lọc nền giá đẹp; thầy nhắc cốc tay cầm như ví dụ hình mà người ta cho là "đẹp" nhưng có thể do người điều khiển giá vẽ ra. Hai cách nhìn khác nhau về cùng một mẫu: một bên coi là cơ hội, một bên coi là kịch bản có thể bị dàn dựng.

**Đọc thêm:** [Mastering Mark Minervini's SEPA trading strategy - tổng hợp thứ cấp](https://grandavehousing.calpoly.edu/blog/mastering-mark-minervinis-sepa-trading-strategy-1764803681); [Minervini Trend Template - bộ lọc mô tả điều kiện](https://vcpscanner.com/screens/minervini-trend-template)

### Mẫu nến Nhật (Hanging Man, Hammer) và hiệu quả thực nghiệm

**Thầy nhắc ở:** B9 02:15, B10 01:37, B10 02:35, B11 01:21 - thầy bác bỏ hoàn toàn, nói đã kiểm định và thất bại.

**Là gì:** Nến Nhật là cách biểu diễn giá mỗi phiên bằng thân nến và bóng nến (giá mở cửa, cao nhất, thấp nhất, đóng cửa). Hammer (cây búa) là nến có thân nhỏ ở gần đỉnh, bóng dưới dài (thường từ hai lần thân trở lên), gần như không có bóng trên; xuất hiện sau đoạn giảm thì được coi là tín hiệu đảo chiều tăng. Hanging Man (người treo cổ) có hình dạng y hệt nhưng xuất hiện sau đoạn tăng và được coi là tín hiệu đảo chiều giảm. Hình dạng giống nhau, chỉ khác bối cảnh xu hướng trước đó.

**Giải thích:** Nguồn gốc thường được gắn với thương nhân gạo Munehisa Homma (1724-1803) ở Nhật Bản, người công bố tác phẩm năm 1755; Steve Nison lập luận biểu đồ nến thực ra xuất hiện muộn hơn, sau khoảng năm 1850. Về hiệu quả thực nghiệm: Marshall, Young và Rose (Journal of Banking & Finance, 2006) kiểm tra 28 tín hiệu nến trên các cổ phiếu Dow Jones giai đoạn 1992-2002, vào lệnh ở giá đóng cửa ngày sau tín hiệu và giữ 10 ngày, kết luận bằng kiểm định bootstrap rằng không có bằng chứng tín hiệu nến dự báo giá, và không thấy người theo phân tích nến vượt trội thị trường; bài nối tiếp năm 2007 cũng kết luận chỉ dựa vào chúng là không hợp lý. Có phản biện rằng các nghiên cứu bỏ qua yếu tố xu hướng ngắn hạn, và mẫu chỉ là cổ phiếu vốn hoá lớn Mỹ. Bulkowski kiểm tra Hanging Man và thấy 59% trường hợp lại là tiếp diễn xu hướng tăng, xếp hạng 87 trong các mẫu nến (trên trang của ông, cập nhật tháng 12/2025). Việc nhận diện mẫu nến còn mang tính chủ quan, phần mềm phải dùng quy tắc định sẵn.

**Liên hệ với bài học:** Thầy bác bỏ nến Nhật và nói đã kiểm định: điều này khớp với các nghiên cứu học thuật nêu trên về cổ phiếu Mỹ. Điểm cần nhớ là kết luận áp dụng cho các quy tắc được kiểm định (một mẫu, một thời gian giữ), không chứng minh mọi cách đọc nến đều vô ích.

**Đọc thêm:** [Candlestick pattern - Wikipedia](https://en.wikipedia.org/wiki/Candlestick_pattern); [Candlestick technical trading strategies: Can they create value for investors? - EconPapers](https://econpapers.repec.org/RePEc:eee:jbfina:v:30:y:2006:i:8:p:2303-2323); [Candlesticks, fiddlesticks - CXO Advisory](https://www.cxoadvisory.com/technical-trading/candlesticks-fiddlesticks/); [Hanging Man - thepatternsite.com (Bulkowski)](https://thepatternsite.com/HangingMan.html)

### Price action (PA)

**Thầy nhắc ở:** B13 02:57 - thầy chê "không đáng đọc".

**Là gì:** Price action là cách giao dịch chỉ dựa vào đọc hành vi giá thô (các thanh giá, nến, hỗ trợ kháng cự, xu hướng), ít hoặc không dùng chỉ báo.

**Giải thích:** Trường phái này gắn với nhiều tác giả; một tên tiêu biểu là Al Brooks với bộ ba sách của Wiley, mở đầu bằng "Trading Price Action Trends", đọc biểu đồ từng thanh một. Ủng hộ: chỉ báo chỉ là phép biến đổi của giá nên đọc thẳng giá là gọn hơn. Phản biện: cách đọc mang tính diễn giải chủ quan, khó kiểm định khách quan, và sách của Brooks bị nhiều độc giả nhận xét là dày đặc, khó đọc. Tra cứu không tìm được đánh giá học thuật chính thức về hiệu quả của phương pháp này.

**Liên hệ với bài học:** Thầy chê price action vì nó vẫn dừng ở việc đọc hình dạng giá mà không hỏi ai đang đè, gom, xả đằng sau; điều này cùng tinh thần với lời phê bình của thầy với nến Nhật và chỉ báo.

**Đọc thêm:** [Price action trading - Wikipedia](https://en.wikipedia.com/wiki/Price_action_trading); [Opinions on Al Brooks - BabyPips forum](https://forums.babypips.com/t/opinions-on-al-brooks/190776)

## Cụm 5. Wyckoff, giá - khối lượng, cấu trúc lệnh

### Phương pháp Wyckoff (tích luỹ, phân phối, spring, upthrust, shakeout, Phase D, back up)

**Thầy nhắc ở:** B9 03:00, B10 00:34, B10 00:39, B11 01:25, B12 02:37, B13 02:13, B13 02:16, B13 03:20, B13 03:32, B14 01:40, B15 02:14 - chu trình đè, gom, đẩy, xả của thầy rất gần Wyckoff nhưng thầy không nhắc tên; nhãn Phase D và Back Up trên biểu đồ HT1; thầy dùng "tích", "phân", "rũ"; học viên gắn Phase A, B, C lên VN-Index.

**Là gì:** Phương pháp Wyckoff là cách đọc thị trường qua giá và khối lượng, mô tả thị trường đi qua các chu kỳ tích luỹ (accumulation), tăng giá (markup), phân phối (distribution) và giảm giá (markdown), do dòng tiền lớn ("Composite Man") dẫn dắt. Đối chiếu thuật ngữ: "gom" tương ứng tích luỹ, "đẩy" là markup, "xả" là phân phối, "đè" là markdown và giai đoạn nén giá trước khi gom.

**Giải thích:** Richard D. Wyckoff (2/11/1873 - 7/3/1934) bắt đầu làm nhân viên môi giới năm 1888, sáng lập tạp chí The Ticker (1907, sau đổi tên The Magazine of Wall Street), viết "Studies in Tape Reading" (1910) và nhiều sách khác. Ba quy luật nền: cung và cầu, nhân và quả (cause and effect: vùng tích luỹ càng dài thì nhịp tăng sau đó càng lớn), nỗ lực và kết quả (effort versus result: khối lượng là nỗ lực, biến động giá là kết quả; khi lệch nhau là dấu hiệu đổi hướng).

Sơ đồ tích luỹ chuẩn theo các nguồn phổ thông (nhãn có thể lệch giữa các nguồn):
- Phase A: dừng đà giảm. Selling Climax (SC) là cú bán tháo khối lượng lớn, tiếp theo Automatic Rally (AR) rồi Secondary Test (ST) kiểm tra lại đáy.
- Phase B: giá đi ngang trong vùng, dòng tiền lớn hấp thụ nguồn cung.
- Phase C: phép thử cuối cùng, thường là Spring (giá chọc thủng đáy vùng rồi rút lên nhanh, rũ bỏ người cầm cổ phiếu yếu; "shakeout" là thuật ngữ gần nghĩa) hoặc Last Point of Support. Không phải sơ đồ nào cũng có spring.
- Phase D: Sign of Strength (SOS), giá đi lên kháng cự với biên độ và khối lượng tăng, thể hiện cầu chủ động; sau đó các nhịp lùi về trên khối lượng và biên độ hẹp được gọi là Last Point of Support (LPS) hoặc "Back Up to the Edge of the Creek" (BUEC), tức nhịp "back up" quay về mép vùng vừa phá.
- Phase E: giá rời hẳn vùng, bước vào markup.

Sơ đồ phân phối đối xứng: Preliminary Supply và Buying Climax ở Phase A; vùng đi ngang ở Phase B; Phase C có Upthrust (giá chọc lên trên kháng cự rồi thất bại, dạng bẫy tăng giá; upthrust sau phân phối gọi UTAD); Phase D có Sign of Weakness (SOW) phá hỗ trợ và Last Point of Supply (LPSY) là đỉnh thấp hơn; Phase E là markdown.

Đánh giá: bách khoa toàn thư mô tả phương pháp này là chủ quan, bản thân Wyckoff viết có chỗ mâu thuẫn, nhiều phiên bản hiện nay do học trò viết lại ("Wyckoff 2.0"), và việc kiểm định độc lập về hiệu quả rất hạn chế. Wyckoff còn bị một số người đương thời cáo buộc thao túng thị trường và từng bị toà xử thua một vụ kiện lừa đảo, theo Wikipedia.

**Liên hệ với bài học:** Chu trình đè, gom, đẩy, xả của thầy là cùng một khung với bốn pha Wyckoff; học viên gắn Phase A, B, C lên VN-Index là dùng đúng sơ đồ này. Chỗ khác: thầy bàn theo hành vi và ý đồ của người chơi lớn, và không gắn nhãn sự kiện bằng thuật ngữ Wyckoff.

**Đọc thêm:** [Richard Wyckoff - Wikipedia](https://en.wikipedia.org/wiki/Richard_Wyckoff); [How to determine the best trade entry points - StockCharts (Wyckoff)](https://my.stockcharts.com/articles/wyckoff/2016/04/how-to-determine-the-best-trade-entry-points.html); [Wyckoff Power Charting - StockCharts](https://my.stockcharts.com/articles/wyckoff/2015/07/wyckoff-power-charting-lets-review.html); [Wyckoff Method Explained - CMC Markets](https://www.cmcmarkets.com/en-gb/trading-strategy/what-is-wyckoff-method); [Wyckoff accumulation and distribution schematic - MarketCalls](https://www.marketcalls.in/price-action/understanding-wyckoff-accumulation-and-distribution-schematic-a-study-of-stock-market-behavior.html)

### Phân tích giá và khối lượng (VSA), phiên phân phối, churning, test cung cầu

**Thầy nhắc ở:** B11 01:38, B13 02:13, B13 02:16, B14 01:40 - dấu hiệu vùng đỉnh của thầy; học viên nhắc selling climax, test cung cầu.

**Là gì:** VSA (Volume Spread Analysis) là phương pháp đọc cùng lúc khối lượng, biên độ thanh giá (spread) và vị trí đóng cửa để suy ra cung cầu. Tom Williams, một cựu nhà giao dịch, hệ thống hoá phương pháp dựa trên ý tưởng của Wyckoff, xuất bản trong "The Undeclared Secrets That Drive the Stock Market" (1993), sau đổi tên "Master the Markets".

**Giải thích:** Một số khái niệm hay gặp: "no demand" là nến tăng biên độ hẹp khối lượng thấp, cho thấy thiếu lực mua; "no supply" là nến giảm biên độ hẹp khối lượng thấp, cho thấy thiếu lực bán; "stopping volume" là khối lượng tăng vọt chặn đà giảm, gần với Selling Climax của Wyckoff. Phiên phân phối là phiên có khối lượng lớn ở vùng giá cao mà giá không tiến thêm được, gợi ý hàng đang được bán ra cho bên mua. Khái niệm "churning" (khối lượng lớn nhưng giá đi rất ít) tôi chưa tìm được nguồn đáng tin trong lần tra cứu này; theo nguyên lý nỗ lực và kết quả của Wyckoff, nó là trường hợp nỗ lực lớn nhưng kết quả nhỏ, từ khoá gợi ý: "effort vs result Wyckoff", "churning volume". Test cung cầu là phiên thử lại vùng giá cũ với khối lượng thấp: nếu khối lượng cạn mà giá không giảm thêm thì được hiểu là cung đã yếu. Nguyên lý chung: khối lượng xác nhận xu hướng, tăng giá kèm khối lượng tăng được coi là khoẻ hơn tăng giá kèm khối lượng cạn. Các số liệu "tỷ lệ thắng" trên blog về VSA không có kiểm chứng độc lập.

**Liên hệ với bài học:** Các mô tả "tích", "phân", "rũ" của thầy và học viên là cách gọi tắt các tình huống VSA này trên VN-Index; thầy dùng chúng để nhận ra vùng đỉnh.

**Đọc thêm:** [Volume Spread Analysis - LuxAlgo](https://www.luxalgo.com/library/concept/volume-spread-analysis/); [No-demand and no-supply bars - LuxAlgo](https://www.luxalgo.com/library/concept/no-demand-no-supply-bars.md); [Stopping volume - Trading Setups Review](https://tradingsetupsreview.com/stopping-volume-volume-spread-analysis-vsa)

### Market Profile và Volume Profile (TPO, POC, value area)

**Thầy nhắc ở:** B17 02:29, B17 02:30 - thầy nhắc ở Mỹ có Market Profile thay cho bảng ba giá; AmiBroker có sẵn khối lượng theo vùng giá.

**Là gì:** Market Profile do J. Peter Steidlmayer phát triển ở Sở giao dịch Chicago Board of Trade vào thập niên 1980, vẽ phân bố THỜI GIAN giao dịch tại từng mức giá bằng các chữ cái TPO (Time Price Opportunity, mỗi chữ thường là một khung 30 phút). Volume Profile vẽ phân bố KHỐI LƯỢNG tại từng mức giá.

**Giải thích:** Điểm chung: cả hai có "point of control" (POC) là mức giá có nhiều hoạt động nhất, và "value area" là vùng chứa khoảng 70% hoạt động trong phiên. Điểm khác: với Market Profile, POC là mức có nhiều chữ TPO nhất; với Volume Profile, POC là mức có nhiều khối lượng nhất, nên hai POC có thể là hai mức giá khác nhau. Volume Profile không gắn với một tác giả duy nhất; nó mượn các từ "value" và "point of control" của Market Profile rồi thay thời gian bằng khối lượng. TradingView có công cụ TPO và Volume Profile; AmiBroker có chỉ báo khối lượng theo vùng giá.

**Liên hệ với bài học:** Thầy dùng chúng để so sánh với "bảng ba giá" của thị trường Việt Nam: bảng ba giá chỉ cho ba mức tốt nhất, còn các profile này cho cái nhìn phân bố khối lượng ở mọi mức giá trong phiên.

**Đọc thêm:** [Market profile - Wikipedia](https://en.wikipedia.com/wiki/Market_profile); [Time Price Opportunity charts explained - TradingView](https://in.tradingview.com/support/solutions/43000725590-time-price-opportunity-charts-explained); [Market profile vs volume profile - The Right Trader](https://therighttrader.com/learn/comparisons/market-profile-vs-volume-profile)

### Độ sâu thị trường (market depth, order book, Level 2) và danh sách lệnh khớp (time and sales)

**Thầy nhắc ở:** B17 02:17, B17 02:18, B17 02:28 - thầy so sánh với bảng ba giá Việt Nam.

**Là gì:** Độ sâu thị trường (Level 2, sổ lệnh) là danh sách các lệnh mua bán đang chờ khớp ở nhiều mức giá quanh giá hiện tại. Time and sales (băng giao dịch, "tape") là bản ghi các lệnh đã khớp: giá, khối lượng, thời điểm.

**Giải thích:** Có thể hình dung sổ lệnh là "ý định" (lệnh giới hạn đang chờ), còn danh sách lệnh khớp là "hành động" (giao dịch đã xảy ra). Lệnh lớn xuất hiện trong sổ lệnh nhưng không bao giờ khớp có thể chỉ là sự đánh lừa; hiện tượng đặt lệnh giả rồi huỷ gọi là spoofing. Vì vậy hai nguồn dữ liệu được dùng song song. Ở Việt Nam, bảng giá thông thường chỉ hiển thị ba mức giá mua và ba mức giá bán tốt nhất, thay vì toàn bộ sổ lệnh. Cần lưu ý Level 2 chỉ là bối cảnh, không phải tín hiệu độc lập.

**Liên hệ với bài học:** Thầy nhắc để người học thấy dữ liệu bảng giá Việt Nam hạn chế hơn các thị trường có sổ lệnh sâu, nên việc "đọc lệnh" kiểu nước ngoài khó áp dụng nguyên xi.

**Đọc thêm:** [Level 2 and time and sales - Day Trading Toolkit](https://daytradingtoolkit.com/beginners-guide/level-2-quotes-time-sales-order-book); [Level 1 vs Level 2 - LuxAlgo](https://www.luxalgo.com/blog/level-1-vs-level-2-what-traders-need-to-know/); [Tape reading - LuxAlgo](https://www.luxalgo.com/library/concept/tape-reading.md)

### Khối lượng mua chủ động, bán chủ động

**Thầy nhắc ở:** B15 00:50 - học viên hỏi khi bàn tự mua bán.

**Là gì:** Mỗi giao dịch khớp có một bên "chủ động" là bên đặt lệnh đánh vào lệnh chờ của bên kia: mua chủ động là mua khớp ngay tại giá chào bán, bán chủ động là bán khớp ngay tại giá chào mua. Khối lượng mua chủ động thường được hiểu là lực đẩy giá lên.

**Giải thích:** Trong tài chính định lượng, việc phân loại giao dịch thành mua chủ động hay bán chủ động thường dùng thuật toán Lee-Ready (kết hợp so sánh giá khớp với giá chào mua chào bán và so với giá khớp trước đó). Nghiên cứu cho thấy độ chính xác khoảng 85-93% tuỳ định nghĩa, giao dịch khớp đúng giữa giá mua và giá bán khó phân loại nhất, và sai số không ngẫu nhiên (thanh khoản cao và lệnh nhỏ bị phân loại sai nhiều hơn). Tra cứu không tìm được tài liệu tiếng Việt từ sở giao dịch giải thích cách bảng giá của các công ty chứng khoán phân loại mua và bán chủ động, nên cách mỗi nhà cung cấp thống kê có thể khác nhau; từ khoá gợi ý: "buyer-initiated seller-initiated volume", "tick rule". Giới hạn chung: thống kê này chỉ cho biết ai chủ động về mặt cơ chế, không cho biết ai là người có thông tin hay bên nào là "tay to".

**Liên hệ với bài học:** Học viên hỏi để xem có thể nhìn ra tay to tự mua tự bán qua khối lượng chủ động không. Cần thận trọng: mua chủ động nhiều không đồng nghĩa lực cầu bền vững, và một người có thể đặt cả hai phía.

**Đọc thêm:** [A test of the accuracy of the Lee/Ready trade classification algorithm - IDEAS](https://ideas.repec.org/a/eee/intfin/v11y2001i2p147-165.html); [Taker buy sell volume ratio - CryptoQuant](https://userguide.cryptoquant.com/vietnamese/cryptoquant-metrics/market/taker-buy-sell-volume-ratio)

## Cụm 6. Công cụ, sách, chứng chỉ, chiến lược nhắc đến

### Công cụ: AmiBroker (AFL), TradingView (Pine Script, Replay), FireAnt

**Thầy nhắc ở:** B4 04:11, B4 04:12, B17 01:29, B17 01:31, B18 00:19 - thầy chọn AmiBroker làm phần mềm thực hành; dạy tập đọc đồ thị bằng Replay; nói tự viết bộ lọc phải học AFL.

**Là gì:** AmiBroker là phần mềm phân tích kỹ thuật và kiểm thử chiến lược (backtest) cho máy tính cá nhân, do Tomasz Janeczko phát triển; AFL (AmiBroker Formula Language) là ngôn ngữ để viết chỉ báo, bộ lọc (scan) và hệ thống giao dịch. TradingView là nền tảng biểu đồ trên web; Pine Script là ngôn ngữ riêng của nó; Replay là chế độ phát lại giá quá khứ từng thanh. FireAnt là ứng dụng và trang dữ liệu chứng khoán Việt Nam.

**Giải thích:**
- AmiBroker: Janeczko có bằng thạc sĩ (1994) và tiến sĩ (1998) về khoa học máy tính và viễn thông tại Đại học Bách khoa Wrocław; AFL ra đời cùng AmiBroker 3.00 năm 1999 theo trang lịch sử của hãng. Phần mềm bán theo giấy phép mua một lần (một danh sách bên thứ ba ghi khoảng 279 đến 369 USD, có bản dùng thử 30 ngày; giá có thể đã thay đổi, cần xem amibroker.com). Trình backtest tính cả hoa hồng, lãi vay, lệnh dừng lỗ, quy mô vị thế. Ví dụ rất ngắn bằng AFL: Buy = Cross(Close, MA(Close, 50)); Sell = Cross(MA(Close, 50), Close); (mua khi giá cắt lên MA50, bán khi cắt xuống).
- Dữ liệu Việt Nam cho AmiBroker: FireAnt có sản phẩm MetaKit cung cấp dữ liệu giao dịch cổ phiếu và chỉ số ba sàn cho AmiBroker, MetaStock, MetaTrader (tài liệu không ghi rõ là realtime hay trễ). Các nguồn khác nêu trong kết quả tìm kiếm: Data24 của MBS cấu hình cập nhật theo phút, Ami X của DNSE có cập nhật realtime. Giá và điều kiện cần hỏi trực tiếp nhà cung cấp.
- TradingView: Replay cho phép bắt đầu từ một cây nến trong quá khứ, các nến sau đó được ẩn đi, rồi phát tiếp từng thanh để tự đưa ra quyết định như thời gian thực; giới hạn lịch sử phụ thuộc gói (gói miễn phí dùng được từ khung ngày). Pine Script có mô hình thực thi theo sự kiện, chạy tuần tự từng thanh; có hai loại script: chỉ báo (vẽ) và chiến lược (mô phỏng lệnh). Cẩn thận với việc tín hiệu dựa trên thanh chưa đóng có thể "vẽ lại" (repaint).
- So sánh: AmiBroker mạnh ở backtest danh mục và quét hàng loạt mã trên dữ liệu có sẵn trong máy; TradingView mạnh ở biểu đồ trên web, cộng đồng và Replay.
- Quy trình backtest thủ công bằng Replay: chọn mốc, ẩn tương lai, ghi lại lý do vào lệnh, điểm cắt lỗ, rồi phát tiếp và ghi kết quả.

**Liên hệ với bài học:** Thầy dạy dùng Replay để luyện đọc đồ thị mà không "nhìn trước" tương lai, và AmiBroker để tự viết bộ lọc. Đây là công cụ thực hành, phần thầy nhấn mạnh là hiểu logic trước khi viết lệnh.

**Đọc thêm:** [AmiBroker backtesting guide](https://amibroker.com/guide/h_backtest.html); [AmiBroker company history](https://lic.amibroker.com/about.html); [Bar Replay - TradingView Help](https://www.tradingview.com:443/support/solutions/43000712747-bar-replay-how-and-why-to-test-a-strategy-in-the-past/); [Pine Script execution model - TradingView](https://www.tradingview.com/pine-script-docs/language/execution-model); [FireAnt MetaKit Professional User Guide](https://corporate.fireant.vn/Download/FireAnt%20MetaKit%20Professional%20User%20Guide.pdf); [Amibroker là gì - DNSE](https://www.dnse.com.vn/hoc/amibroker-la-gi)

### Chứng chỉ CMT (Chartered Market Technician)

**Thầy nhắc ở:** B13 02:57 - học viên nói từng theo học.

**Là gì:** CMT là chứng chỉ quốc tế về phân tích kỹ thuật do CMT Association cấp.

**Giải thích:** Chương trình có ba cấp (Level I, II, III) phải thi theo thứ tự; Level I và II là trắc nghiệm, Level III có thêm câu trả lời ngắn. Kỳ thi tổ chức hai lần mỗi năm (tháng 6 và tháng 12) theo hình thức trên máy tại trung tâm Prometric hoặc giám sát từ xa, bằng tiếng Anh. Để được cấp danh hiệu cần đỗ cả ba cấp, là hội viên và có ba năm kinh nghiệm liên quan; thường mất khoảng ba năm chuẩn bị. Giáo trình chính thức do Wiley xuất bản. Phí đăng ký một lần khoảng 250 USD theo bảng phí tháng 6/2023 (số liệu cũ, cần kiểm tra lại).

**Liên hệ với bài học:** Học viên nhắc CMT trong cùng đoạn thầy chê price action (B13 02:57). Chương trình CMT bao quát nhiều trường phái phân tích kỹ thuật, trong đó có nhiều thứ thầy đánh giá thấp; chứng chỉ chứng minh người học đã nắm hệ thống kiến thức này, không chứng minh hiệu quả của các phương pháp.

**Đọc thêm:** [What is the CMT Program - CMT Association](https://cmtassociation.org/cmt-program); [About the CMT Exam - UWorld](https://finance.uworld.com/cmt/about-cmt-exam/)

### Sách của Alexander Elder (nguồn chưa chắc)

**Thầy nhắc ở:** B17 01:26 - thầy nhắc sách nói "khi xu thế rõ mới vào".

**Là gì:** Alexander Elder là tác giả "Trading for a Living" (xuất bản lần đầu 1993, có bản sửa "The New Trading for a Living"), nổi tiếng với "ba chữ M" (Mind, Method, Money: tâm lý, phương pháp, quản lý tiền) và hệ thống Triple Screen.

**Giải thích:** Triple Screen dùng ba lớp phân tích: màn hình thứ nhất ở khung thời gian dài xác định hướng xu hướng chính để không giao dịch ngược xu hướng lớn; màn hình thứ hai ở khung vừa dùng chỉ báo dao động ngược xu hướng để tìm điểm vào; màn hình thứ ba để canh lệnh. Elder ví ba lớp này như thuỷ triều, sóng và gợn sóng. Điều này gần với ý "chỉ vào khi xu thế rõ", nhưng tôi không xác nhận được thầy nhắc cuốn nào của Elder hay một tác giả khác. Từ khoá gợi ý: "Elder triple screen", "Trading for a Living trend".

**Liên hệ với bài học:** Nếu đúng là Elder thì "đợi xu thế rõ mới vào" là tinh thần cốt lõi của giao dịch theo xu hướng: vào muộn hơn để đổi lấy độ chắc chắn. Thầy dùng câu này như ví dụ về cách tiếp cận đi sau xu hướng; đối chiếu thêm mục "Giao dịch theo xu hướng".

**Đọc thêm:** [Trading for a Living - Wiley](https://www.wiley-vch.de/en/areas-interest/finance-economics-law/trading-for-a-living-978-0-471-59224-2); [Triple Screen Trading System - The Right Trader](https://therighttrader.com/learn/trend-analysis/triple-screen-trading-system)

### Chiến lược London breakout (forex)

> Mục này không liên quan đến đầu tư nên đã chuyển sang [PL05-phan-tich-ky-thuat.md](../../ngoai-dau-tu/phu-luc/PL05-phan-tich-ky-thuat.md).
