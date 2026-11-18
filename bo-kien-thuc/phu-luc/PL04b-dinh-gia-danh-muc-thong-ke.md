# Phụ lục PL04b - Định giá, lý thuyết danh mục và thống kê tài chính (phần 2)

> Phụ lục của Bộ kiến thức NKT. Giải thích những khái niệm thầy nhắc tới trong bài giảng mà chưa giảng đầy đủ. Nội dung được tra cứu từ các nguồn bên ngoài (thời điểm tra cứu: tháng 11/2026), không phải lời thầy.

Lưu ý chung: phụ lục giải thích khái niệm, không phải lời khuyên đầu tư. Các ví dụ số là số giả định để tự tính bằng tay hoặc Excel, không phải số liệu thị trường. Ký hiệu B3 01:15 nghĩa là buổi 3, phút 01:15 của buổi học.

## Danh sách mục

Cụm 1. Giá trị thời gian của tiền và tỷ lệ chiết khấu
1. NPV, IRR, thời gian thu hồi vốn và giá trị thời gian của tiền
2. WACC, chi phí vốn chủ sở hữu Ke, CAPM và các cách ước lượng tỷ lệ chiết khấu
3. Mô hình chiết khấu cổ tức (DDM, mô hình Gordon)

Cụm 2. Bội số, định giá và các cách ước lượng
4. P/E (trailing, forward), earnings yield, P/B, P/S, EV/EBITDA
5. Net-net, công thức Graham, biên an toàn
6. Unicorn và định giá startup (Alibaba mua Lazada)
7. Ước lượng EPS đồng thuận (consensus) và báo cáo chiến lược của công ty chứng khoán

Cụm 3. Lý thuyết danh mục và thống kê nền
8. Lý thuyết danh mục Markowitz: đa dạng hoá và đường biên hiệu quả
9. Hàm hữu dụng, đường phân bổ vốn (CAL), tỷ lệ Sharpe, rủi ro hệ thống và phi hệ thống
10. Alpha, beta và hồi quy (CAPM trong thực hành)
11. Phân bổ tài sản đa chân trời và chi phí rời thị trường sớm
12. Phân phối chuẩn, đường cong hình chuông và nguyên lý Pareto 80/20

Cụm 4. Quản trị vốn và cắt lỗ
13. Tỷ lệ lợi nhuận trên rủi ro (R/R), kỳ vọng toán, công thức Kelly và quy luật phục hồi sau lỗ
14. Quản trị vốn và tỷ trọng vào lệnh (position sizing)
15. Quy tắc cắt lỗ trong sách nổi tiếng (7-8% của William O'Neil, các ngưỡng 8%, 15%, 20%)

Cụm 5. Ngành, chu kỳ và dòng tiền
16. Phân ngành chuẩn (GICS, ICB), ngành phòng thủ và ngành chu kỳ
17. Luân chuyển ngành theo chu kỳ (sector rotation), Business Cycle Approach to Sectors, Sector Roadmap, GSCI
18. Luân chuyển dòng tiền từ vốn hoá lớn sang vừa và nhỏ trong chu kỳ tăng
19. Phân tích top-down và bottom-up, khung Thiên thời - Địa lợi - Nhân hoà, PEST
20. Phong cách đầu tư: tăng trưởng, giá trị, chất lượng, quy mô; growth stock
21. Sức mạnh tương đối (relative strength) và Relative Rotation Graph (RRG)

Cụm 6. Hành vi, kiểm nghiệm dữ liệu và các nhân vật mẫu
22. Lý thuyết trò chơi (game theory), cân bằng Nash, trò chơi tổng bằng không
23. Tài chính hành vi (behavioral finance), FOMO, ác cảm thua lỗ
24. Tài chính hành vi và các hiệu ứng mùa vụ
25. Phản ứng giá quanh ngày công bố kết quả kinh doanh
26. Tâm lý bầy đàn trong định giá: Seeking Alpha, quant
27. Thiên kiến nhìn trước (look-ahead bias)
28. Quant Trading của Hoàng Tùng
29. Warren Buffett và Bill Gates: triết lý đầu tư giá trị, kế hoạch thừa kế

## Cụm 1. Giá trị thời gian của tiền và tỷ lệ chiết khấu

### NPV, IRR, thời gian thu hồi vốn và giá trị thời gian của tiền (Net present value, Internal rate of return, Payback period, Time value of money)

**Thầy nhắc ở:** B7 00:23, B7 01:51, B7 01:53 - thầy nói giá trị thời gian của tiền là tư tưởng gốc của mọi phương pháp tài chính.

**Là gì:** Một đồng nhận hôm nay có giá trị hơn một đồng nhận sau này, vì đồng tiền hôm nay có thể đem đầu tư để sinh lời (chi phí cơ hội). NPV (giá trị hiện tại ròng) là tổng các dòng tiền tương lai quy về hiện tại, trừ vốn bỏ ra. IRR (suất sinh lời nội bộ) là mức chiết khấu làm NPV bằng 0.

**Giải thích:**
- Giá trị tương lai: FV = PV x (1 + r)^n. Hiện tại: PV = FV / (1 + r)^n.
- NPV = tổng của dòng tiền năm t chia (1 + r)^t, tính từ t = 0 (năm 0 là vốn bỏ ra, mang dấu âm).
- Ví dụ số: bỏ ra 100, nhận 40, 50, 60 trong 3 năm, r = 10%. Hiện giá: 40/1,1 = 36,36; 50/1,21 = 41,32; 60/1,331 = 45,08; tổng 122,76. NPV = 122,76 - 100 = 22,76 dương nên dự án tạo giá trị. Trong Excel: =NPV(10%, 40, 50, 60) - 100 (hàm NPV của Excel mặc định dòng đầu ở cuối kỳ 1, và giả định các kỳ cách đều nhau; dòng tiền lệch ngày dùng XNPV).
- IRR của ví dụ trên khoảng 21,6% (thử dần: ở 21,5% NPV xấp xỉ +0,24; ở 22% xấp xỉ -0,58). Excel: =IRR(...) với dòng -100, 40, 50, 60.
- Thời gian thu hồi vốn: cộng dồn 40, 90, 150 nên thu hồi sau 2 năm + 10/60 = khoảng 2,17 năm. Bản chiết khấu (discounted payback): cộng dồn hiện giá 36,36; 77,69; 122,76 nên khoảng 2 + 22,31/45,08 = 2,49 năm.
- Hạn chế: NPV phụ thuộc mạnh vào dự báo dòng tiền và mức chiết khấu, không cho biết tỷ suất; IRR có thể đánh lừa khi so dự án khác quy mô, giả định tái đầu tư ở chính IRR, và với dòng tiền đổi dấu nhiều lần có thể có nhiều nghiệm hoặc kết quả mâu thuẫn với NPV. Thời gian thu hồi vốn bỏ qua mọi dòng tiền sau điểm hoàn vốn.
- Ví dụ giá trị thời gian: 100 triệu gửi 5 năm ở 8%/năm thành 100 x 1,08^5 = 146,93 triệu; ngược lại 100 triệu nhận sau 5 năm hôm nay chỉ đáng 100 / 1,4693 = 68,06 triệu.

**Liên hệ với bài học:** mọi phương pháp định giá thầy nói ở các buổi sau (DCF, DDM, bội số) đều là biến thể của việc quy dòng tiền về hiện tại, nên chọn mức chiết khấu r là chỗ khó nhất (xem mục WACC). Ở Việt Nam, lãi suất và rủi ro thay đổi nhanh nên một mức r cố định cho nhiều năm dễ bị đánh giá thấp hoặc cao rủi ro; tôi chưa tìm được nguồn nghiên cứu riêng bàn chuyện này.

**Đọc thêm:** [Net present value (Wikipedia)](https://en.wikipedia.org/wiki/Net_present_value); [NPV vs IRR (FE Training)](https://www.fe.training/?p=10041779); [Hạn chế của IRR (Masterworks)](https://insights.masterworks.com/?p=5240)

### WACC, chi phí vốn chủ sở hữu Ke, CAPM và các cách ước lượng tỷ lệ chiết khấu (Weighted average cost of capital, Cost of equity, Build-up)

**Thầy nhắc ở:** B2 02:43, B4 03:55, B6 02:04, B7 02:03, B7 02:12, B7 03:21, B7 03:46, B8 03:09 - thầy phản biện việc dùng WACC cố định, so ROA với WACC và ROE với Ke, nói tỷ lệ chiết khấu r rất khó tính và "mỗi ông mỗi kiểu".

**Là gì:** WACC là chi phí vốn bình quân gia quyền của doanh nghiệp, gồm chi phí nợ sau thuế và chi phí vốn chủ sở hữu (Ke), mỗi loại nhân với tỷ trọng trong tổng vốn. Đây là mức chiết khấu thường dùng cho dòng tiền doanh nghiệp (FCFF). Ke là lợi suất tối thiểu cổ đông đòi hỏi, dùng chiết khấu dòng tiền cho chủ sở hữu.

**Giải thích:**
- WACC = E/V x Ke + D/V x Kd x (1 - T). E là vốn chủ, D là nợ, V = E + D, Kd là lãi vay trước thuế, T là thuế suất (lãi vay được khấu trừ thuế nên Kd nhân (1 - T)).
- CAPM: Ke = Rf + beta x (Rm - Rf). Rf lãi suất phi rủi ro (thường lấy lợi suất trái phiếu chính phủ 10 năm), beta đo độ nhạy với thị trường, (Rm - Rf) là phần bù rủi ro thị trường.
- Ví dụ số (lấy theo một tài liệu giảng dạy): Rf 4,5%, beta 1,25, phần bù 6% thì Ke = 4,5 + 1,25 x 6 = 12%. Kd trước thuế 5%, thuế 25% thì Kd sau thuế = 3,75%. Cơ cấu 60% vốn chủ, 40% nợ: WACC = 0,6 x 12 + 0,4 x 3,75 = 8,7%.
- Build-up (xây dựng cộng dồn): Ke = Rf + phần bù rủi ro cổ phiếu + phần bù quy mô nhỏ + phần bù rủi ro riêng của công ty. Dùng khi khó ước lượng beta đáng tin (công ty nhỏ, ít thanh khoản).
- Vì sao "mỗi ông mỗi kiểu": Rf, phần bù rủi ro, beta (chọn chỉ số, chu kỳ, số năm), tỷ trọng nợ (giá trị sổ sách hay thị trường) đều là lựa chọn của người làm; đổi một thông số là WACC đổi, kéo theo giá trị đổi lớn. Thầy nhắc tên vài hãng lớn (nghe như McKinsey, Goldman Sachs, Credit Suisse): chưa tìm được nguồn xác nhận mỗi hãng dùng cách nào, nên không khẳng định ở đây.
- Thay đổi theo lãi suất và cơ cấu vốn: lãi suất tăng thì Rf và Kd tăng; vay nhiều hơn thì Kd rẻ hơn nhưng rủi ro vốn chủ cao hơn nên Ke tăng. Vì vậy WACC không cố định, điều thầy phản biện.
- Ở Việt Nam: dữ liệu beta và lịch sử thị trường ngắn, thanh khoản thấp, nhà đầu tư cá nhân chiếm tỷ trọng lớn nên beta kém ổn định. Damodaran công bố phần bù rủi ro theo quốc gia (một trang tổng hợp ghi tổng phần bù rủi ro vốn chủ của Việt Nam là 11,13% tại 01/01/2023; đây là số lẻ từ trang thứ ba, cần đối chiếu bảng gốc của Damodaran). Trang valueinvesting.io (tính tự động) dùng phần bù thị trường 9,5-10,5% cho một cổ phiếu Việt Nam, cao hơn nhiều so với mức 4-7% hay gặp trong tài liệu phổ thông.

**Liên hệ với bài học:** khi thầy nói "r rất khó tính", đó là phê bình chính đáng với DCF/DDM: kết quả nhạy với r. Việc so ROE với Ke (hoặc ROA với WACC) là cách hỏi: doanh nghiệp có kiếm được hơn chi phí vốn không; nếu ROE bền vững thấp hơn Ke thì tăng trưởng huỷ giá trị.

**Đọc thêm:** [WACC formula (CFI)](https://corporatefinanceinstitute.com/resources/knowledge/valuation/wacc-formula/); [WACC explained (Ryan O'Connell)](https://ryanoconnellfinance.com/weighted-average-cost-of-capital/); [CAPM (Wikipedia)](https://en.wikipedia.org/wiki/Capital_asset_pricing_model); [Damodaran, trang chủ dữ liệu](https://pages.stern.nyu.edu/adamodar/New_Home_Page/home.htm); [Vietnam total equity risk premium (GuruFocus)](https://www.gurufocus.com/economic_indicators/6042/vietnam-total-equity-risk-premium?search=VIE); [WACC là gì (DSC)](https://dsc.com.vn/kien-thuc/wacc-la-gi)

### Mô hình chiết khấu cổ tức (Dividend discount model - DDM, mô hình Gordon)

**Thầy nhắc ở:** B2 02:45, B7 03:26, B7 03:46 - thầy phê phán DDM; báo cáo DPM có mục DDM; nhắc khi bàn chính sách cổ tức.

**Là gì:** Giá cổ phiếu bằng hiện giá của toàn bộ cổ tức tương lai. Dạng đơn giản nhất là mô hình tăng trưởng đều của Gordon: giá = D1 / (r - g).

**Giải thích:**
- D1 là cổ tức năm tới, r là chi phí vốn chủ (Ke), g là tốc độ tăng cổ tức đều mãi mãi. Nếu cho D0 (cổ tức vừa trả) thì D1 = D0 x (1 + g).
- Ví dụ số: D1 = 2.000 đồng, r = 12%, g = 4%: giá = 2.000 / 0,08 = 25.000 đồng. Chỉ đổi g lên 6%: 2.000 / 0,06 = 33.333 đồng, tăng 33% chỉ vì 2 điểm phần trăm. Đó là độ nhạy của mô hình.
- Điều kiện: cổ tức tăng đều, g nhỏ hơn r (nếu g gần r giá tiến tới vô cực), công ty trả cổ tức ổn định. Với công ty tăng trưởng nhanh thì dùng bản hai hoặc ba giai đoạn.
- Hạn chế thường nêu: bỏ qua dòng tiền ngoài cổ tức (mua lại cổ phiếu, giữ lại tiền tái đầu tư), không định giá được công ty không trả cổ tức, nhạy với g và r. Người bảo vệ DDM lập luận: cổ đông chỉ thật sự nhận tiền qua cổ tức (hoặc khi bán), nên dòng cổ tức là gốc của giá trị; John Burr Williams (1938) dựng ý tưởng này, Gordon và Shapiro (1956) đưa về dạng gọn.
- Khi nào dùng thay DCF: khi công ty trả cổ tức đều và có chính sách rõ (ngân hàng, tiện ích, một số doanh nghiệp bất động sản khu công nghiệp trả cổ tức tiền mặt). Khi công ty đang tái đầu tư mạnh, DCF phù hợp hơn.
- Lưu ý cho Việt Nam (suy luận thêm, chưa tìm được nguồn riêng): nhiều công ty chia cổ tức bằng cổ phiếu, không phải dòng tiền ra khỏi công ty, nên không đưa thẳng vào DDM như cổ tức tiền mặt được.

**Liên hệ với bài học:** thầy phê phán DDM vì giá phụ thuộc g và r, hai con số khó biết; phụ lục này cho thấy phê phán đó có cơ sở toán học (độ nhạy). Cũng nên biết DDM vẫn là khung gốc để hiểu vì sao chính sách cổ tức liên quan đến giá.

**Đọc thêm:** [Dividend discount model (Wikipedia)](https://en.wikipedia.org/wiki/Dividend_discount_model); [Gordon growth model (CFI)](https://corporatefinanceinstitute.com/resources/valuation/gordon-growth-model); [A review of the Dividend Discount Model (arXiv)](https://arxiv.org/pdf/2001.00465)

## Cụm 2. Bội số, định giá và các cách ước lượng

### P/E (trailing, forward), earnings yield, P/B, P/S, EV/EBITDA

**Thầy nhắc ở:** B2 00:45, B2 02:35, B4 02:11, B4 03:55 - thầy giảng P/E như số năm hoàn vốn, lấy ví dụ P/E của Tesla "trên mây".

**Là gì:** Bội số định giá là tỷ lệ giữa giá (hoặc giá trị doanh nghiệp) và một chỉ tiêu tài chính. P/E = giá / lợi nhuận mỗi cổ phiếu (EPS); trailing P/E dùng EPS 12 tháng đã qua, forward P/E dùng EPS dự báo. Earnings yield = EPS / giá, tức nghịch đảo của P/E.

**Giải thích:**
- Ví dụ số: giá 50.000 đồng, EPS 5.000 đồng: P/E = 10; earnings yield = 10%. Nếu lợi nhuận đứng yên và chia hết, "10 năm hoàn vốn": đây là cách hiểu trực quan thầy dùng.
- Hạn chế của cách hiểu số năm hoàn vốn: lợi nhuận không đứng yên (tăng thì hoàn vốn nhanh hơn, giảm thì chậm hơn); lợi nhuận kế toán không phải tiền mặt về túi cổ đông; công ty giữ lại lợi nhuận hoặc chia cổ tức làm thay đổi bức tranh; P/E thấp có thể là bẫy giá trị khi lợi nhuận sắp giảm; lợi nhuận bất thường làm P/E méo. Earnings yield tiện so với lãi suất trái phiếu (P/E 14 tương ứng khoảng 7,1%).
- P/B = giá / giá trị sổ sách mỗi cổ phiếu (BVPS): giá 30.000, BVPS 20.000 thì P/B = 1,5; hợp với ngân hàng, bảo hiểm, tài sản nặng. P/S = giá / doanh thu mỗi cổ phiếu: dùng khi chưa có lãi (công ty tăng trưởng) nhưng bỏ qua biên lợi nhuận.
- EV/EBITDA: EV = vốn hoá + nợ vay - tiền mặt (cộng cổ đông thiểu số, cổ phiếu ưu đãi nếu có). Ví dụ: vốn hoá 1.000 tỷ, nợ 400 tỷ, tiền 100 tỷ thì EV = 1.300 tỷ; EBITDA 200 tỷ thì EV/EBITDA = 6,5 lần. Dùng để so các công ty khác cơ cấu vốn, hoặc khi lợi nhuận ròng âm; nhược điểm: EBITDA không phải dòng tiền, bỏ qua vốn đầu tư (capex) và vốn lưu động.
- Chọn bội số: P/E cho công ty có lãi ổn định; P/B cho tổ chức tài chính; P/S cho công ty chưa có lãi; EV/EBITDA cho ngành nhiều nợ, vốn nặng hoặc khi so xuyên biên giới.
- P/E Tesla 2021: không có con số duy nhất. Marketscreener ghi P/E năm tài chính 2021 khoảng 216 lần; một bài Motley Fool ngày 08/12/2021 nêu forward P/E 124 lần; InvestorPlace (không rõ ngày) nêu trailing P/E 411 lần. Các số lệch vì khác thời điểm giá và loại EPS. Số chuẩn: giá đóng cửa 31/12/2021 chia EPS pha loãng năm 2021 trong báo cáo 10-K của Tesla.

**Liên hệ với bài học:** thầy dùng P/E như thước đo "bao lâu thu hồi", rất trực quan nhưng chỉ đúng trong giả định lợi nhuận phẳng; P/E của Tesla "trên mây" minh hoạ giá phản ánh kỳ vọng tăng trưởng, không phải lợi nhuận hiện tại. Ở Việt Nam, dùng EPS theo báo cáo hợp nhất và lưu ý EPS bị pha loãng bởi cổ phiếu thưởng, phát hành thêm.

**Đọc thêm:** [Earnings yield (Wikipedia)](https://en.wikipedia.org/wiki/Earnings_yield); [EV/EBITDA (GuruFocus)](https://gurufocus.com/term/enterprise-value-to-ebitda); [EV/EBITDA, lựa chọn thay cho P/E (Investing.com)](https://www.investing.com/analysis/ev-ebitda:-an-alternative-to-price-earnings-240352); [Tesla valuation (MarketScreener)](https://uk.marketscreener.com/quote/stock/TESLA-INC-6344549/valuation/); [Tesla, Motley Fool 08/12/2021](https://www.fool.com/investing/2021/12/08/up-1305-since-march-2020-low-is-tesla-still-a-buy)

### Net-net, công thức Graham, biên an toàn (Margin of safety)

**Thầy nhắc ở:** B2 02:33, B2 02:55, B3 03:24, B4 01:35 - "cách định giá 1"; học viên áp công thức Graham với EPS và P/E.

**Là gì:** Benjamin Graham (thầy của Warren Buffett) đề ra vài cách ước lượng giá trị. Net-net: mua cổ phiếu có giá thấp hơn giá trị tài sản lưu động ròng (NCAV). Biên an toàn: chênh lệch giữa giá trị ước lượng và giá mua, làm vùng đệm cho sai số.

**Giải thích:**
- NCAV = tài sản ngắn hạn - tổng nợ phải trả; chia cho số cổ phiếu ra NCAV mỗi cổ phiếu. Graham chỉ mua khi giá nhỏ hơn 2/3 NCAV. Ví dụ: tài sản ngắn hạn 500, nợ 300, 10 cổ phiếu thì NCAV = 20 mỗi cổ phiếu; ngưỡng mua = 20 x 2/3 = 13,3.
- Số Graham: căn bậc hai của (22,5 x EPS x BVPS), coi là giá tối đa nhà đầu tư thận trọng nên trả. Ví dụ EPS 2, BVPS 20: căn (22,5 x 2 x 20) = căn 900 = 30.
- Công thức V = EPS x (8,5 + 2g): 8,5 là P/E của công ty không tăng trưởng, g là tăng trưởng lợi nhuận kỳ vọng (đơn vị phần trăm, thường 5 đến 10 năm). Ví dụ EPS 2.000 đồng, g = 5: V = 2.000 x 18,5 = 37.000 đồng. Bản sau thêm hệ số 4,4/Y (4,4 là lãi suất trái phiếu AAA năm 1962, Y là lãi suất AAA hiện hành). Một bài trên Nasdaq cho rằng công thức này không nằm trong khung chính của Graham (ông nêu ba cách: số Graham, giá doanh nghiệp tăng cấp, NCAV), nguồn khác thì ghi nó xuất hiện ở ấn bản 1962 của Security Analysis. Hai nguồn lệch nhau, nên coi đây là phép ước lượng nhanh, không phải công thức "chuẩn".
- Biên an toàn = (V - giá) / V. V = 37.000, giá mua 25.000 thì biên an toàn = 32,4%. Biên càng lớn thì càng chịu được sai số ước lượng.
- Hạn chế: công thức dùng lãi suất và P/E của những năm 1960, nên hệ số cứng; net-net hiếm gặp ở thị trường tăng giá, thường gặp ở công ty rất yếu, rủi ro "bẫy giá trị"; tôi chưa tìm được nguồn nghiên cứu net-net trên thị trường Việt Nam.

**Liên hệ với bài học:** thầy dùng Graham làm ví dụ cho nhóm phương pháp "định giá bằng tài sản và lợi nhuận hiện tại" và học viên đã thử nhập EPS và P/E. Nên nhớ công thức chỉ cho một con số tham chiếu; thứ thật sự quan trọng của Graham là tư tưởng biên an toàn.

**Đọc thêm:** [Understanding the Benjamin Graham formula (Nasdaq)](https://www.nasdaq.com/articles/understanding-benjamin-graham-formula-correctly-2015-04-28); [Testing Graham's NCAV strategy (Nasdaq)](https://www.nasdaq.com/articles/testing-grahams-net-current-asset-value-strategy-part-1-2017-03-02); [Benjamin Graham formula (Cavacopedia)](https://cavac.at/cavacopedia/Benjamin%20Graham%20formula); [Benjamin Graham formula (Investing.com)](https://www.investing.com/academy/analysis/benjamin-graham-formula-definition); [Deep value (Stockopedia)](https://www.stockopedia.com/academy/articles/deep-value/)

### Unicorn và định giá startup (Alibaba mua Lazada)

**Thầy nhắc ở:** B2 00:49, B4 00:24 - ví dụ chấp nhận lỗ để thống lĩnh thị trường.

**Là gì:** Unicorn là startup chưa niêm yết có định giá trên 1 tỷ USD; thuật ngữ do nhà đầu tư mạo hiểm Aileen Lee đặt năm 2013. Trên 10 tỷ USD gọi là decacorn.

**Giải thích:**
- Định giá startup dựa vào cơ hội tăng trưởng và kỳ vọng dài hạn, thường theo vòng gọi vốn; ba phương pháp phổ biến: DCF, so bội số công ty tương đương, so giao dịch tương đương. Một nghiên cứu Stanford 2018 cho rằng định giá báo cáo của unicorn cao hơn giá trị hợp lý trung bình 48%.
- Lazada: tháng 4/2016 Alibaba nắm quyền kiểm soát (khoảng 1 tỷ USD gồm phát hành mới khoảng 500 triệu USD và mua cổ phiếu từ cổ đông hiện hữu; một số nguồn ghi 51%). Năm 2017 Alibaba tăng lên 83% với 1 tỷ USD nữa (định giá khoảng 3,1 tỷ USD theo báo chí). Tháng 3/2018 Alibaba rót thêm 2 tỷ USD, nâng tổng vốn đầu tư vào Lazada lên 4 tỷ USD; bà Lucy Peng thay ông Max Bittner làm CEO. Tôi chưa kiểm tra diễn biến của Lazada sau 2018.
- Ý nghĩa với định giá: với công ty đốt tiền để giành thị phần, lợi nhuận hiện tại không nói lên gì, nên P/E vô nghĩa; nhà đầu tư trả cho thị phần và kỳ vọng độc quyền sau này.

**Liên hệ với bài học:** thầy dùng ví dụ này để nói rằng chấp nhận lỗ có thể là chiến lược hợp lý khi mục tiêu là thống lĩnh, và vì thế các bội số dựa vào lợi nhuận không áp dụng được cho nhóm này.

**Đọc thêm:** [Unicorn (Wikipedia)](https://en.wikipedia.org/wiki/Unicorn_(finance)); [Alibaba invests additional USD2 billion in Lazada (Alibaba Group)](https://www.alibabagroup.com/en-US/document-1491488162294267904); [Alibaba doubles down on Lazada (TechCrunch, 18/03/2018)](https://techcrunch.com/2018/03/18/alibaba-doubles-down-on-lazada); [Alibaba raises stake in Lazada (Caixin, 19/03/2018)](https://www.caixinglobal.com/2018-03-19/alibaba-raises-stake-in-southeast-asias-lazada-101223338.html)

### Ước lượng EPS đồng thuận (consensus) và báo cáo chiến lược của công ty chứng khoán

**Thầy nhắc ở:** B2 01:24, B4 01:22 - thầy nói nước ngoài có consensus, Việt Nam không.

**Là gì:** Consensus là con số trung bình hoặc trung vị các dự báo của nhiều nhà phân tích bán bên (sell-side) cho một chỉ tiêu (EPS, doanh thu, EBITDA). Các nhà cung cấp dữ liệu như Bloomberg, FactSet, LSEG (trước là Refinitiv, sở hữu I/B/E/S) thu thập mô hình của từng nhà phân tích rồi gộp lại.

**Giải thích:**
- Các nhà cung cấp công bố consensus hơi khác nhau vì cách lọc ước tính cũ và cách tính; một nghiên cứu đăng trên Columbia Law School Blue Sky Blog (2021) cho rằng I/B/E/S đưa ra những lựa chọn chủ quan khi loại bỏ ước tính, và có xu hướng loại bớt ước tính lạc quan sau khi trao đổi với doanh nghiệp, giúp công ty dễ "vượt kỳ vọng". Nghiên cứu khác (Springer, 2020) cho thấy độ chính xác và độ lệch của I/B/E/S khác nhau giữa các phiên bản tệp dữ liệu.
- Nhìn chung các nghiên cứu lâu năm cho rằng dự báo sell-side thường lệch lạc quan. Ở Việt Nam số công ty chứng khoán theo dõi một mã ít, không có cơ sở dữ liệu consensus công khai tương đương; cách thực tế là tự lấy trung bình các báo cáo của vài công ty, kèm lưu ý trên.
- Cách đọc và phản biện báo cáo chiến lược: xem giả định vĩ mô (GDP, lãi suất, tỷ giá), P/E mục tiêu được chọn dựa trên gì, EPS dự phóng tăng bao nhiêu so với lịch sử, có kiểm định lại dự báo kỳ trước không, và công ty chứng khoán có quan hệ kinh doanh với doanh nghiệp được khuyến nghị không.

**Liên hệ với bài học:** thầy phê phán định giá dựa vào dự báo người khác; nên coi consensus như một dữ liệu về kỳ vọng thị trường (giá đã phản ánh gì), không phải sự thật.

**Đọc thêm:** [How optimistic earnings forecasts are kept in check (CLS Blue Sky Blog)](https://clsbluesky.law.columbia.edu/2021/12/21/how-optimistic-earnings-forecasts-are-kept-in-check/?amp=1); [Accuracy and bias of I/B/E/S detail files (Review of Accounting Studies)](https://link.springer.com/article/10.1007/s11142-020-09560-x); [Companies publish their own consensus estimates (IR Impact)](https://www.ir-impact.com/2012/07/companies-publish-their-own-consensus-estimates/)

## Cụm 3. Lý thuyết danh mục và thống kê nền

### Lý thuyết danh mục Markowitz: đa dạng hoá và đường biên hiệu quả (Modern portfolio theory)

**Thầy nhắc ở:** B2 02:27, B2 03:30, B5 02:42, B16 00:21 - thầy phê phán mô hình trung bình - phương sai, cho là sai lầm với nhà đầu tư cá nhân.

**Là gì:** Harry Markowitz (bài báo "Portfolio Selection", 1952) chỉ ra rằng rủi ro của danh mục không phải trung bình rủi ro từng tài sản, mà phụ thuộc vào tương quan giữa các tài sản. Giữ các tài sản không tương quan hoàn toàn giúp giảm rủi ro mà không nhất thiết giảm lợi suất kỳ vọng. Rủi ro được đo bằng độ lệch chuẩn (hoặc phương sai) của lợi suất.

**Giải thích:**
- Lợi suất kỳ vọng danh mục = tổng (tỷ trọng x lợi suất kỳ vọng từng tài sản). Hai tài sản: phương sai = wA bình phương x sA bình phương + wB bình phương x sB bình phương + 2 x wA x wB x sA x sB x tương quan AB.
- Ví dụ số: A có độ lệch chuẩn 20%, B có 10%, tỷ trọng 50/50. Nếu tương quan 1: độ lệch chuẩn danh mục = 15% (chỉ là trung bình). Nếu tương quan 0,5: phương sai = 0,25 x 0,04 + 0,25 x 0,01 + 2 x 0,25 x 0,2 x 0,1 x 0,5 = 0,01 + 0,0025 + 0,005 = 0,0175 nên độ lệch chuẩn = 13,2%. Nếu tương quan -1: 5%. Tương quan càng thấp, rủi ro danh mục càng giảm. Trong Excel: =CORREL(), =STDEV.S(), =SUMPRODUCT/MMULT cho dạng ma trận.
- Đường biên hiệu quả (efficient frontier): với mỗi mức lợi suất kỳ vọng, danh mục có phương sai thấp nhất; các điểm đó nối thành đường cong (hình "viên đạn Markowitz"). Danh mục nằm phía dưới đường là không hiệu quả.
- Giả định: nhà đầu tư ghét rủi ro và hợp lý, lợi suất xấp xỉ phân phối chuẩn, quá khứ (phương sai, tương quan) dùng làm đại diện cho tương lai, không có chi phí giao dịch.
- Phê bình: rất nhạy với sai số ước lượng đầu vào (lợi suất kỳ vọng thay đổi chút thì tỷ trọng tối ưu thay đổi mạnh); phương sai coi lãi và lỗ lớn như nhau trong khi nhà đầu tư sợ lỗ hơn; đuôi dày (biến cố cực đoan) bị đánh giá thấp (Taleb phê phán gay gắt); một giai đoạn duy nhất; có nghiên cứu cho rằng chia đều tỷ trọng đôi khi ngang hoặc hơn tối ưu hoá Markowitz. Một bài trên AAII ghi rằng đa số nhà đầu tư, kể cả tổ chức, không thật sự tối ưu hoá theo đường biên, và Markowitz cũng không làm vậy.
- Với nhà đầu tư cá nhân ở Việt Nam: danh mục thường 3 đến 10 mã, tương quan giữa các mã cùng ngành và cùng chu kỳ cao, dữ liệu lịch sử ngắn nên ma trận tương quan ước lượng kém. Tôi chưa tìm được nguồn học thuật riêng về chủ đề này cho thị trường Việt Nam.

**Liên hệ với bài học:** thầy cho Markowitz là sai lầm với nhà đầu tư cá nhân vì (1) cá nhân không có số liệu kỳ vọng đáng tin, (2) đa dạng hoá quá mức làm loãng lợi nhuận khi bạn thật sự có lợi thế thông tin ở vài mã. Ý chính của Markowitz (đừng đặt hết vào các tài sản cùng chiều) vẫn được nhiều người coi là đúng; cái bị chỉ trích là việc ép thành bài toán tối ưu bằng số.

**Đọc thêm:** [Modern portfolio theory (Wikipedia)](https://en.wikipedia.org/wiki/Modern_portfolio_theory); [Harry Markowitz and modern portfolio theory (Britannica)](https://eb.com/money/modern-portfolio-theory-explained); [Harry Markowitz's lasting influence (AAII)](https://www.aaii.com/investor-update/article/68554-harry-markowitzs-lasting-influence-on-investing); [The birth of portfolio theory (JLEM, 2024)](https://jlem.com/p/Editors_Introduction-The_Birth_of_Portfolio_Theory_-_July_2024.pdf); [Is MPT obsolete? (GARP)](https://www.garp.org/risk-intelligence/market/is-modern-portfolio-theory-obsolete?hs_amp=true)

### Hàm hữu dụng, đường phân bổ vốn (CAL), tỷ lệ Sharpe, rủi ro hệ thống và phi hệ thống

**Thầy nhắc ở:** B9 00:00, B9 01:05, B9 01:06 - slide chiếu mà thầy không giảng.

**Là gì:** Đây là phần tiếp theo của lý thuyết danh mục trong giáo trình đầu tư kinh điển. Hàm hữu dụng cho điểm mức hài lòng của nhà đầu tư với một danh mục: U = E(r) - 1/2 x A x sigma bình phương, trong đó A là hệ số ngại rủi ro (A càng lớn càng ngại). CAL là đường các kết hợp giữa tài sản phi rủi ro và danh mục rủi ro; độ dốc của nó là tỷ lệ Sharpe.

**Giải thích:**
- Ví dụ số: danh mục rủi ro có E(r) = 12%, độ lệch chuẩn 20%, lãi suất phi rủi ro 3%, A = 3. Hữu dụng U = 0,12 - 0,5 x 3 x 0,04 = 0,06 (6%), hơn 3% khi gửi phi rủi ro, nên nhà đầu tư này thích nắm danh mục rủi ro hơn.
- Tỷ lệ phân bổ tối ưu vào danh mục rủi ro: y = (E(r) - rf) / (A x sigma bình phương) = 0,09 / (3 x 0,04) = 0,75: 75% vào danh mục rủi ro, 25% phi rủi ro (công thức này tôi suy từ điều kiện bậc nhất, giáo trình Bodie, Kane, Marcus trình bày tương tự). A = 6 thì y = 0,375.
- Tỷ lệ Sharpe = (E(r) - rf) / sigma = 0,09 / 0,20 = 0,45; đây là độ dốc của CAL. Danh mục tiếp tuyến (tangency) là danh mục rủi ro có Sharpe cao nhất; mọi nhà đầu tư hiệu quả chỉ pha trộn danh mục đó với tài sản phi rủi ro (định lý một quỹ). Sharpe gốc (1966) gọi là "reward-to-variability"; bản sửa 1994 dùng chênh lệch so với chuẩn so sánh.
- Hạn chế của Sharpe: giả định lợi suất xấp xỉ chuẩn, nên bỏ sót rủi ro đuôi (chiến lược bán quyền chọn có thể có Sharpe cao đến khi xảy ra lỗ lớn); có thể bị làm đẹp nếu tài sản kém thanh khoản được định giá "mượt".
- Rủi ro phi hệ thống (đặc thù từng công ty) giảm được bằng đa dạng hoá; rủi ro hệ thống (cả thị trường) thì không, và chỉ phần này được thị trường "trả công" theo CAPM.
- Bảng câu hỏi khẩu vị rủi ro 9-27 điểm: chưa tìm được nguồn đáng tin cho bảng cụ thể 9 câu, mỗi câu 1 đến 3 điểm; từ khoá gợi ý: "risk tolerance questionnaire", "Grable Lytton risk tolerance scale", và giáo trình "Investments" của Bodie, Kane, Marcus chương 6.

**Liên hệ với bài học:** các slide này là phần lý thuyết gốc của việc "mỗi người có khẩu vị rủi ro khác nhau nên tỷ trọng cổ phiếu khác nhau". Điểm cốt lõi: đừng chọn "danh mục tốt nhất" chung cho mọi người, mà chọn danh mục rủi ro hiệu quả rồi chỉnh tỷ trọng theo A.

**Đọc thêm:** [Risk aversion, CAL, market portfolio (AnalystPrep)](https://analystprep.com/cfa-level-1-exam/uncategorized/optimal-portfolio-selection-risk-aversion-capital-allocation-line-market-portfolio-and-capital-market-line/); [Sharpe ratio (Wikipedia)](https://en.wikipedia.org/wiki/Sharpe_ratio); [Modern portfolio theory (Wikipedia)](https://en.wikipedia.org/wiki/Modern_portfolio_theory)

### Alpha, beta và hồi quy (CAPM trong thực hành)

**Thầy nhắc ở:** B2 03:30, B3 03:24, B5 02:42 - thầy giải thích giản lược alpha, beta.

**Là gì:** Beta đo độ nhạy của cổ phiếu với thị trường: beta = hiệp phương sai (cổ phiếu, thị trường) / phương sai thị trường; thị trường có beta 1. Alpha là phần lợi suất vượt mức CAPM dự đoán (lợi suất "vượt trội" do kỹ năng, may mắn hoặc yếu tố chưa mô hình hoá).

**Giải thích:**
- Hồi quy: (lợi suất cổ phiếu - rf) = alpha + beta x (lợi suất thị trường - rf) + sai số. Hệ số góc là beta, hệ số chặn là alpha.
- Ví dụ số (giả định, 3 kỳ, đã trừ rf): thị trường +10%, 0%, -10%; cổ phiếu +14%, +2%, -10%. Trung bình cổ phiếu 2%. Hiệp phương sai (tổng độ lệch nhân nhau) = 10 x 12 + 0 + (-10) x (-12) = 240; tổng bình phương độ lệch thị trường = 200; beta = 1,2; alpha = 2 - 1,2 x 0 = 2%. Trong Excel: =SLOPE(lợi suất CP, lợi suất TT) và =INTERCEPT(...). Ví dụ này chỉ minh hoạ phép tính; thực tế cần hàng chục kỳ và nên kiểm tra R bình phương.
- Beta lớn hơn 1 là biến động hơn thị trường; ví dụ thị trường +1% thì cổ phiếu beta 1,2 kỳ vọng +1,2%.
- Phê bình CAPM: beta không ổn định theo thời gian; "danh mục thị trường" thực không quan sát được (phê bình Roll); hiệu ứng quy mô và giá trị không giải thích được bằng beta (dẫn tới mô hình Fama-French); cổ phiếu beta thấp thường sinh lời cao hơn dự đoán (bất thường biến động thấp). Fama và French (2004) nhận xét thất bại thực nghiệm của CAPM khiến nhiều ứng dụng không còn hiệu lực.
- Tương quan rủi ro giữa các tài sản: hệ số tương quan nằm trong -1 đến +1; hai tài sản lên xuống cùng nhau (gần +1) không giảm rủi ro cho nhau, ví dụ nhiều mã ngân hàng trong một danh mục.
- Ở Việt Nam: chọn VN-Index làm thị trường thì beta của cổ phiếu vốn hoá lớn bị chi phối bởi chính các cổ phiếu đó (vì tỷ trọng lớn trong chỉ số), và dữ liệu lịch sử ngắn nên beta nhiều mã kém tin cậy; chưa tìm được nguồn học thuật riêng.

**Liên hệ với bài học:** khi thầy nói "alpha là cái mình làm giỏi hơn thị trường, beta là cái thị trường cho", đó là cách nói giản lược của hồi quy ở trên. Chỗ khác với hiểu biết phổ thông: trong học thuật alpha phải được đo sau khi đã trừ rủi ro (beta), nên "lãi hơn VN-Index" chưa chắc là alpha.

**Đọc thêm:** [Capital asset pricing model (Wikipedia)](https://en.wikipedia.org/wiki/Capital_asset_pricing_model); [Modern portfolio theory (Wikipedia)](https://en.wikipedia.org/wiki/Modern_portfolio_theory)

### Phân bổ tài sản đa chân trời (secular trend, business cycle, tactical, Dynamic Asset Allocation) và chi phí rời thị trường sớm

**Thầy nhắc ở:** B2 01:20, B2 02:57, B3 03:19 - slide ba khung thời gian và "Keep your balance" (41%, 23%).

**Là gì:** Cách xây dựng danh mục theo ba lớp thời gian: xu hướng dài hạn nhiều năm (secular), chu kỳ kinh doanh vài năm (business cycle), và điều chỉnh chiến thuật ngắn hạn (tactical). "Dynamic asset allocation" là điều chỉnh tỷ trọng giữa các loại tài sản theo thay đổi của điều kiện thị trường. Phần "rời thị trường sớm" là lập luận rằng bỏ lỡ vài phiên tăng mạnh nhất làm lợi suất dài hạn giảm nhiều.

**Giải thích:**
- Con số 41% và 23% trên slide: chưa tìm được tài liệu gốc ("Keep your balance" cùng hai số này) trong lần tra cứu; các tổ chức như T. Rowe Price, Vanguard và Questrade có các minh hoạ tương tự với số liệu riêng, ví dụ Questrade: lợi suất bình quân năm 11,1% nếu luôn đầu tư, 8,9% nếu bỏ lỡ 10 ngày tốt nhất, 7,3% nếu bỏ lỡ 20 ngày, 6,0% nếu bỏ lỡ 30 ngày (số liệu và thị trường của họ, không phải của slide thầy).
- Phản biện: Kiplinger chỉ ra rằng ngày tốt nhất và ngày tệ nhất thường nằm sát nhau (từ 1988, hơn 70% số lần một ngày tốt nhất hoặc tệ nhất xảy ra trong vòng 21 phiên so với một ngày cực đoan khác), nên người rời thị trường vì sợ cũng thường tránh luôn những ngày tệ nhất; câu hỏi đáng hỏi hơn là danh mục có chịu được giai đoạn biến động hay không.
- Ví dụ số tự tính: nếu 20 năm lợi suất 10%/năm, 100 triệu thành 100 x 1,1^20 = 672,7 triệu; nếu thiếu vài ngày tốt khiến lợi suất còn 8%, thành 100 x 1,08^20 = 466,1 triệu, thấp hơn khoảng 31%. Đây là phép tính minh hoạ, không phải số thực.
- Ở Việt Nam: tôi chưa tìm được nghiên cứu "missed best days" cho VN-Index; biên độ giá và cơ cấu nhà đầu tư cá nhân khiến phân bố ngày tăng mạnh khác thị trường Mỹ.

**Liên hệ với bài học:** thầy dùng slide để nói về việc đừng quá thường xuyên ra vào thị trường và cần tách quyết định theo ba khung thời gian. Hiểu rõ: các minh hoạ "bỏ lỡ ngày tốt nhất" mang tính khuyến khích ở lại thị trường, người phản biện chỉ ra chúng bỏ qua việc tránh được các ngày xấu nhất.

**Đọc thêm:** [Stay invested (T. Rowe Price)](https://troweprice.com/en/us/insights/staying-invested-the-cost-of-cashing-out-during-a-market-sell-off); [Why staying invested matters (Questrade)](https://www.questrade.com/learning/markets-economy/why-staying-invested-matters); [Is buy and hold really the best strategy? (Kiplinger)](https://www.kiplinger.com/investing/is-buy-and-hold-really-the-best-investing-strategy); [Staying the course (Vanguard)](https://advisors.vanguard.com/insights/article/staying-the-course-does-not-mean-set-it-and-forget-it.html)

### Phân phối chuẩn, đường cong hình chuông và nguyên lý Pareto 80/20

**Thầy nhắc ở:** B1 02:50, B2 00:14, B4 01:07 (phân phối chuẩn); B16 01:27, B19 01:16 (Pareto) - thầy vẽ đa số ở giữa, tinh hoa khoảng 0,5%, tỷ lệ 20/80; dùng Pareto để lọc tin, phân bổ tài sản và tập trung đầu mối.

**Là gì:** Phân phối chuẩn là phân phối đối xứng hình chuông, được xác định bởi trung bình và độ lệch chuẩn. Nguyên lý Pareto (80/20) là quy tắc kinh nghiệm: một thiểu số nguyên nhân (khoảng 20%) tạo ra đa số kết quả (khoảng 80%).

**Giải thích:**
- Quy tắc 68-95-99,7: khoảng 68,27% quan sát nằm trong 1 độ lệch chuẩn quanh trung bình, 95,45% trong 2, 99,73% trong 3. Ngoài 3 độ lệch chuẩn khoảng 0,27% (xấp xỉ 1 trên 370), mỗi bên đuôi khoảng 0,135%. Nếu dữ liệu có đuôi dày thì các tỷ lệ này không còn đúng; bất đẳng thức Chebyshev chỉ đảm bảo khoảng 88,9% trong 3 độ lệch chuẩn.
- Ví dụ số: lợi suất ngày trung bình 0,1%, độ lệch chuẩn 1,5%. Nếu chuẩn, 95% số phiên nằm trong khoảng -2,9% đến +3,1%. Một phiên giảm 7% là hơn 4 độ lệch chuẩn, theo phân phối chuẩn gần như không xảy ra, nhưng thị trường thật có những phiên như vậy: đó là lý do giới học thuật cảnh báo về đuôi dày.
- Độ lệch chuẩn bằng tay: lợi suất 10%, -5%, 15%, 0%: trung bình 5%; độ lệch 5, -10, 10, -5; bình phương 25, 100, 100, 25 = 250; phương sai mẫu = 250/3 = 83,3; độ lệch chuẩn mẫu = 9,13% (Excel =STDEV.S). Dùng chia cho n thì 62,5 và 7,91% (=STDEV.P).
- Pareto: nhà kinh tế người Ý Vilfredo Pareto quan sát khoảng 1896 đến 1906 rằng khoảng 80% đất ở Ý thuộc 20% dân; Joseph Juran đưa vào quản lý chất lượng năm 1941 với cách gọi "số ít quan trọng, số nhiều hữu ích". Toán học tương ứng là phân phối luỹ thừa (Pareto) với tham số khoảng 1,16 cho tỷ lệ 80:20. 80/20 chỉ là quy tắc thô: thực tế có thể là 90/10 hay 70/30, hai con số không nhất thiết cộng thành 100.
- Phạm vi áp dụng: phân bổ doanh thu theo khách hàng, lỗi phần mềm, thu nhập, chi phí y tế. Cảnh báo: phân tích Pareto có thể bỏ qua vấn đề nhỏ nhưng lớn dần, và nhiều con số dẫn trong các nguồn mô tả cần kiểm chứng.
- Tinh hoa 0,5% trên hình của thầy: đó là cách vẽ minh hoạ; đuôi phân phối chuẩn vượt 2,5 độ lệch chuẩn xấp xỉ 0,6% mỗi bên. Tôi chưa xác minh trùng khớp chủ ý của thầy.

**Liên hệ với bài học:** thầy dùng đường cong chuông để nói đa số nhà đầu tư nằm giữa và chỉ rất ít người vượt trội, còn Pareto để nhắc tập trung vào ít nguồn tin, ít mã, ít việc quan trọng nhất. Lưu ý: lợi suất cổ phiếu và thu nhập không thật sự chuẩn, nên đừng dùng quy tắc 68-95-99,7 như đảm bảo.

**Đọc thêm:** [68-95-99.7 rule (Wikipedia)](https://en.wikipedia.org/wiki/68%E2%80%9395%E2%80%9399.7_rule); [Pareto principle (Wikipedia)](https://en.wikipedia.org/wiki/Pareto_principle)

## Cụm 4. Quản trị vốn và cắt lỗ

### Tỷ lệ lợi nhuận trên rủi ro (R/R), kỳ vọng toán (expectancy), công thức Kelly và quy luật phục hồi sau lỗ

**Thầy nhắc ở:** B9 03:08, B10 02:12, B10 02:15, B13 02:11, B14 00:27 - thầy viết A/B = 2, nhắc sách toán về tỷ lệ cá cược, câu tự kiểm tra "lỗ 50% cần lãi 100%".

**Là gì:** R/R là tỷ lệ giữa mức lãi kỳ vọng (A) và mức lỗ chấp nhận (B) của một lệnh. Kỳ vọng toán (expectancy) là lãi lỗ trung bình mỗi lệnh khi kết hợp R/R với xác suất thắng. Công thức Kelly cho tỷ lệ vốn tối ưu đặt vào mỗi lệnh để tối đa hoá tốc độ tăng trưởng vốn dài hạn (theo logarit).

**Giải thích:**
- Kỳ vọng mỗi lệnh = p x lãi - (1 - p) x lỗ. Đơn vị R (1R = mức lỗ chấp nhận). Ví dụ A/B = 2 (lãi 2R, lỗ 1R), xác suất thắng 40%: kỳ vọng = 0,4 x 2 - 0,6 x 1 = +0,2R mỗi lệnh. Tỷ lệ thắng hoà vốn = 1 / (1 + A/B) = 33,3%. Nếu R/R = 1 thì cần thắng trên 50%.
- Kelly cho cược thắng nhận b lần tiền cược, thua mất hết: f = p - (1 - p) / b. Ví dụ đồng xu thắng 60%, chẵn lẻ b = 1: f = 0,6 - 0,4 = 20% vốn mỗi ván. Với p = 40%, b = 2: f = 0,4 - 0,6/2 = 10% vốn. Tốc độ tăng trưởng vốn hình học ở ví dụ đồng xu khoảng 2,03% mỗi ván (so với kỳ vọng số học 4%).
- Kelly một phần (nửa Kelly, một phần tư Kelly) thường dùng để giảm biến động và sai số: nếu bạn ước lượng p quá cao thì cược vượt Kelly, làm tăng nguy cơ phá sản. Phê bình: cần biết chính xác xác suất (thực tế hiếm khi biết), Paul Samuelson cho rằng tối đa hoá tăng trưởng logarit bỏ qua mức chịu rủi ro của từng người, và có tranh luận về việc dùng trung bình tập hợp hay theo thời gian.
- Quy luật phục hồi sau lỗ: lỗ x% cần lãi x / (1 - x) để hoà vốn. Lỗ 10% cần lãi 11,1%; lỗ 20% cần 25%; lỗ 33% cần 50%; lỗ 50% cần 100%; lỗ 70% cần 233%. Lỗ càng sâu, đường về càng dốc, nên kiểm soát mức lỗ quan trọng hơn so với kiếm thêm lãi.
- Với cổ phiếu, p và R/R không cố định, đặc biệt khi giá nhảy cóc qua mức cắt lỗ; chưa tìm được nguồn bàn riêng về Kelly ở thị trường Việt Nam.

**Liên hệ với bài học:** A/B = 2 của thầy chính là R/R; sách toán về cá cược thầy nhắc rất có thể là các tài liệu về tiêu chí Kelly. Điều thầy muốn nhấn là: không chỉ thắng nhiều lần mà phải xét cả độ lớn lãi lỗ.

**Đọc thêm:** [Kelly criterion (Wikipedia)](https://en.wikipedia.org/wiki/Kelly_criterion); [Position sizing guide (TradingSim)](https://www.tradingsim.com/blog/position-sizing-guide)

### Quản trị vốn và tỷ trọng vào lệnh (position sizing)

**Thầy nhắc ở:** B14 00:16, B17 03:21 - thầy nhắc lời khuyên vào lệnh 20-30% và các mức vốn 500 triệu, 5 tỷ, 50 tỷ.

**Là gì:** Position sizing là quyết định mua bao nhiêu cổ phiếu cho mỗi lệnh, dựa trên tổng vốn, mức rủi ro chấp nhận mất và khoảng cách tới điểm cắt lỗ.

**Giải thích:**
- Công thức cố định phần trăm rủi ro (fixed fractional): số cổ phiếu = (vốn x % rủi ro mỗi lệnh) / (giá vào - giá cắt lỗ). Ví dụ vốn 500 triệu, chấp nhận mất 1% = 5 triệu, giá vào 50.000, cắt lỗ cách 7% (46.500, lỗ 3.500 mỗi cổ phiếu): số cổ phiếu = 5.000.000 / 3.500 = 1.428, làm tròn 1.400 (HOSE có lô chẵn 100 cổ phiếu từ 04/01/2021) tức vốn vào lệnh 70 triệu = 14% vốn. Nếu cắt lỗ rộng hơn (15%) thì số cổ phiếu giảm xuống còn khoảng 666, vốn vào lệnh khoảng 6,7%, mức mất tối đa vẫn 5 triệu.
- Do đó tỷ trọng vào lệnh là kết quả của rủi ro chấp nhận và cắt lỗ, không phải con số cố định. Mức 20-30% vốn mỗi lệnh thầy nhắc tương ứng với chiến lược ít mã, tập trung; người dùng quy tắc 1% có thể vào lệnh 10 đến 15% vốn nếu cắt lỗ 7 đến 10%.
- Hạn chế: công thức giả định lệnh cắt lỗ khớp đúng giá; khi giá nhảy cóc hoặc kém thanh khoản, lỗ thực có thể vượt 1%. Biên độ giá ở Việt Nam hạn chế khả năng thoát lệnh trong phiên (nguồn lệch nhau: HOSE ±7% hoặc ±7,5%, HNX ±10%, UPCoM ±15%); chưa có văn bản gốc trong kết quả tra cứu.
- Vốn lớn và thanh khoản: khi vốn lên hàng chục tỷ, khối lượng mỗi lệnh có thể chiếm tỷ lệ đáng kể trong thanh khoản của cổ phiếu, nên việc vào ra làm giá dịch chuyển và chi phí trượt giá tăng; nhiều tổ chức giới hạn tỷ trọng theo khối lượng giao dịch bình quân. Phần này là nguyên tắc chung tôi chưa tìm được nguồn định lượng cho thị trường Việt Nam; chưa tìm được nguồn nào bàn về các mốc 500 triệu, 5 tỷ, 50 tỷ do thầy nêu.

**Liên hệ với bài học:** thầy gắn số vốn với cách vào lệnh vì vốn nhỏ có thể tập trung vài mã, vốn lớn thì bị thanh khoản chi phối; đây là lập luận hợp lý về nguyên tắc, nhưng các mốc cụ thể là kinh nghiệm cá nhân của thầy.

**Đọc thêm:** [Position sizing guide (TradingSim)](https://www.tradingsim.com/blog/position-sizing-guide); [The one percent rule (TheRightTrader)](https://therighttrader.com/learn/risk-management/one-percent-rule); [HOSE tăng lô giao dịch lên 100 cổ phiếu (Báo Đầu tư)](https://baodautu.vn/hose-tang-lo-giao-dich-tu-10-len-100-co-phieu-tu-dau-nam-2021-d135847.html)

### Quy tắc cắt lỗ trong sách nổi tiếng (7-8% của William O'Neil, các ngưỡng 8%, 15%, 20%)

**Thầy nhắc ở:** B13 02:14, B14 00:27 - thầy phê phán áp dụng máy móc.

**Là gì:** William O'Neil (nhà sáng lập Investor's Business Daily, tác giả "How to Make Money in Stocks" và phương pháp CAN SLIM) khuyên bán khi cổ phiếu giảm 7 đến 8% so với giá mua, "không có ngoại lệ", để giữ khoản lỗ nhỏ.

**Giải thích:**
- Lập luận ủng hộ: lỗ nhỏ dễ phục hồi (xem bảng phục hồi ở mục Kelly: lỗ 7,5% cần lãi 8,1%); lợi nhuận của CAN SLIM đến từ vài cổ phiếu thắng lớn, nên phải cắt nhanh các lệnh sai; O'Neil nêu tỷ lệ lãi/lỗ khoảng 3:1 (chốt lãi 20 đến 25%, cắt lỗ 7 đến 8%). Trong thị trường giá xuống, một số người khuyên thoát sớm hơn (giảm 3 đến 4% so với điểm mua).
- Phản biện: ngưỡng cố định không tính đến biến động riêng từng cổ phiếu (cổ phiếu biến động mạnh có thể chạm 7% chỉ do nhiễu rồi quay lại); thị trường có biên độ giá và nhảy cóc nên mức thoát thực tế khác; ngưỡng 8%, 15%, 20% ở các sách khác nhau phản ánh phong cách giao dịch khác nhau, không có ngưỡng đúng chung; nhiều trader dùng mức dừng theo biến động (ví dụ bội số ATR) hoặc theo cấu trúc giá thay vì phần trăm cố định.
- Kết hợp với position sizing: điểm cắt lỗ chọn trước, rồi mới tính số cổ phiếu (xem mục trên), thay vì chọn phần trăm rồi mua kích cỡ tuỳ ý.
- Thị trường Việt Nam: tôi chưa tìm được nghiên cứu kiểm định quy tắc 7-8% trên cổ phiếu Việt Nam; phần ghi chú trên là lập luận chung.

**Liên hệ với bài học:** thầy phê phán việc áp dụng máy móc: một ngưỡng phần trăm cố định chỉ có nghĩa khi gắn với lý do vào lệnh và độ biến động của mã. Điểm chung của cả người ủng hộ lẫn người phản biện là phải có điểm thoát định trước, chỉ khác nhau ở cách đặt ngưỡng.

**Đọc thêm:** [William O'Neil's CAN SLIM approach (AAII)](https://www.aaii.com/files/journal/pdf/9874_william-oneil-can-slim-approach-to-selecting-growth-stocks.pdf); [Interview with Bill O'Neil (Motley Fool, 2002)](https://www.fool.com/specials/2002/06/20/foolcom-tmf-interview-bill-oneil-special.aspx); [When to sell stocks, CAN SLIM perspective (Stockopedia)](https://www.stockopedia.com/content/when-to-sell-stocks-a-can-slim-growthmomentum-perspective-63746/)

## Cụm 5. Ngành, chu kỳ và dòng tiền

### Phân ngành chuẩn (GICS, ICB), ngành phòng thủ và ngành chu kỳ

**Thầy nhắc ở:** B1 00:46, B1 01:17, B1 02:52 - thầy liệt kê 8 nhóm ngành chính, gọi y tế và điện là phòng thủ.

**Là gì:** GICS (Global Industry Classification Standard) do MSCI và S&P xây dựng năm 1999; ICB (Industry Classification Benchmark) do FTSE Russell duy trì. Cả hai xếp mọi công ty niêm yết vào các nhóm ngành chuẩn để so sánh quốc tế.

**Giải thích:**
- GICS có 4 cấp: 11 khu vực (sector), 25 nhóm ngành (industry group), 74 ngành, 163 phân ngành. 11 khu vực: Năng lượng (Energy); Vật liệu (Materials); Công nghiệp (Industrials); Tiêu dùng không thiết yếu (Consumer Discretionary); Tiêu dùng thiết yếu (Consumer Staples); Y tế (Health Care); Tài chính (Financials); Công nghệ thông tin (Information Technology); Dịch vụ truyền thông (Communication Services); Tiện ích như điện, nước, khí (Utilities); Bất động sản (Real Estate).
- ICB có 11 ngành lớn (Technology, Telecommunications, Health Care, Financials, Real Estate, Consumer Discretionary, Consumer Staples, Industrials, Basic Materials, Energy, Utilities), 20 siêu nhóm, 45 nhóm, 173 phân nhóm.
- Phòng thủ (defensive) là ngành ít nhạy với chu kỳ kinh tế vì nhu cầu ổn định: thường gồm hàng tiêu dùng thiết yếu, y tế, tiện ích. Chu kỳ (cyclical) là ngành doanh thu và lợi nhuận dao động mạnh theo kinh tế: thường gồm tiêu dùng không thiết yếu, công nghiệp, vật liệu, năng lượng, tài chính. Đây là cách phân loại phổ biến trong giới đầu tư, không phải một phần của chuẩn GICS hay ICB (trang Wikipedia về GICS cũng không phân loại).
- Ở Việt Nam: một nguồn báo chí cho biết HOSE từng công bố phân ngành công ty niêm yết thành 10 ngành và ra mắt 10 chỉ số ngành dựa trên GICS; các nguồn khác nhắc ICB cho các chỉ số ngành VN. Các nguồn tra cứu chưa thống nhất nên cần đối chiếu tài liệu của HOSE. Vietstock cũng công bố một bảng phân ngành riêng (2025) có nhắc lịch sử ICB. Thị trường Việt Nam nghiêng nhiều về tài chính, bất động sản và vật liệu; một factsheet của HOSE (03/2025) ghi tài chính chiếm khoảng 48% vốn hoá tự do chuyển nhượng của nhóm chỉ số đó.
- Tôi không đối chiếu được "8 nhóm" thầy liệt kê với một chuẩn cụ thể; có thể đó là cách gộp riêng của thầy.

**Liên hệ với bài học:** phân ngành chuẩn giúp thầy nói về "luân chuyển ngành" bằng ngôn ngữ chung; nhưng phòng thủ hay chu kỳ chỉ là nhãn tương đối (ví dụ điện ở Việt Nam phụ thuộc thuỷ văn và giá nhiên liệu, y tế dược phẩm có khác biệt giữa các công ty).

**Đọc thêm:** [Global Industry Classification Standard (Wikipedia)](https://en.wikipedia.org/wiki/Global_Industry_Classification_Standard); [Industry Classification Benchmark (Wikipedia)](https://en.wikipedia.org/wiki/Industry_Classification_Benchmark); [ICB (FTSE Russell)](https://www.lseg.com/en/ftse-russell/industry-classification-benchmark-icb); [Vietstock sector classification 2025](https://static1.vietstock.vn/vietstock/2025/VS-SECTOR_2.0_2025.pdf)

### Luân chuyển ngành theo chu kỳ (sector rotation), Business Cycle Approach to Sectors, Sector Roadmap, GSCI

**Thầy nhắc ở:** B1 01:10, B2 01:07, B2 02:50, B2 03:00 - thầy hẹn giảng; bảng từ tài liệu các tổ chức phương Tây.

**Là gì:** Sector rotation là quan điểm rằng các ngành sinh lời vượt trội ở những pha khác nhau của chu kỳ kinh tế, nên có thể xoay vòng tỷ trọng ngành. "Business Cycle Approach to Sectors" là tài liệu của nhóm nghiên cứu phân bổ tài sản của Fidelity, chia chu kỳ thành 4 pha: hồi phục sớm, giữa chu kỳ, cuối chu kỳ, suy thoái.

**Giải thích:**
- Theo Fidelity (phân tích theo xác suất, không phải quy luật chắc chắn): pha sớm thường nghiêng về tiêu dùng không thiết yếu và công nghiệp; giữa chu kỳ là pha dài nhất, công nghiệp thường khá nhưng không ổn định; cuối chu kỳ năng lượng thường tốt. Trong bảng minh hoạ trên Wikipedia: tiêu dùng chu kỳ và tài chính dẫn trước ở đáy; công nghệ và viễn thông ở giữa thị trường tăng; năng lượng muộn gần đỉnh; tiêu dùng thiết yếu "ít tệ nhất" khi thị trường giảm. Phần mô tả pha suy thoái trong tài liệu Fidelity tôi chưa đọc đầy đủ; đọc file PDF gốc.
- Cơ chế vĩ mô được nêu: kinh tế mở rộng làm tăng cầu nguyên liệu, kéo lạm phát và lãi suất lên, rồi làm chậm kinh tế; nên giá hàng hoá, trái phiếu, tiền tệ và cổ phiếu dịch chuyển theo thứ tự tương đối.
- GSCI: S&P GSCI (trước đây là Goldman Sachs Commodity Index) là chỉ số hàng hoá gia quyền theo sản lượng sản xuất toàn cầu trung bình 5 năm gần nhất của từng hàng hoá. Năng lượng là nhóm lớn nhất: khoảng 57,4% theo trọng số hợp đồng sản xuất cho năm 2025 (58,4% cho năm 2024), nên chỉ số này chủ yếu phản ánh giá dầu. Có phiên bản giảm trọng số năng lượng.
- Quan hệ giá hàng hoá với chu kỳ: hàng hoá thường tăng khi kinh tế mở rộng, cầu nguyên liệu tăng và nguồn cung chặt; lúc này ngành năng lượng và vật liệu thường hưởng lợi. Quan hệ này không một chiều, vì giá hàng hoá tăng mạnh cũng có thể làm chậm tăng trưởng (chưa tìm được nguồn định lượng).
- "Sector Roadmap": chưa xác định được tài liệu cụ thể thầy nói; từ khoá gợi ý: "Sector Roadmap" cùng "investment clock", "business cycle sector performance".
- Bằng chứng và giới hạn: Wikipedia ghi bài này thiếu nguồn dẫn; tài liệu Fidelity nêu rõ hiệu quả có thể tăng khi kết hợp phân tích ngành và lạm phát, và ngành đơn lẻ biến động hơn danh mục đa dạng. Ở Việt Nam, chu kỳ kinh tế và chính sách (tín dụng, tỷ giá, đầu tư công) khác thị trường Mỹ; chưa tìm được nguồn xác nhận các bảng phương Tây áp dụng được cho Việt Nam.

**Liên hệ với bài học:** thầy dùng bảng phương Tây để minh hoạ ý "mỗi ngành có lúc"; hãy xem đó là khung tham khảo và kiểm tra bằng số liệu Việt Nam.

**Đọc thêm:** [Business cycle approach to equity sector investing (Fidelity)](https://institutional.fidelity.com/app/literature/item/943044.html); [Business cycle sector approach (Fidelity, PDF)](https://fidelity.com/bin-public/060_www_fidelity_com/documents/fixed-income/Business_Cycle_Sector_Approach.pdf); [The business cycle and its investing implications (Fidelity)](https://www.fidelity.com/learning-center/trading-investing/markets-sectors/business-cycle); [Sector rotation (Wikipedia)](https://en.wikipedia.org/wiki/Sector_rotation); [S&P GSCI (Wikipedia)](https://en.wikipedia.org/wiki/S%26P_GSCI); [Goldman Sachs, GSCI approach](https://www.goldmansachs.com/what-we-do/FICC-and-equities/business-groups/sts-folder/gsci/approach.html); [S&P GSCI methodology](https://spglobal.com/spdji/kr/documents/methodologies/methodology-sp-gsci.pdf)

### Luân chuyển dòng tiền từ vốn hoá lớn sang vừa và nhỏ trong chu kỳ tăng

**Thầy nhắc ở:** B6 03:15, B10 01:23, B11 03:32 - thầy giải thích blue chip tăng trước rồi lan sang nhóm nhỏ, bằng tỷ trọng trong chỉ số.

**Là gì:** Quan niệm cho rằng trong một pha tăng, dòng tiền vào nhóm vốn hoá lớn (blue chip) trước, rồi lan dần sang vốn hoá vừa và nhỏ.

**Giải thích:**
- Tỷ trọng trong chỉ số: chỉ số tính theo vốn hoá (có thể điều chỉnh free float) thì cổ phiếu lớn có sức nặng lớn. Ví dụ tổng vốn hoá 1.000, cổ phiếu A vốn hoá 100 (tỷ trọng 10%): A tăng 5% kéo chỉ số tăng khoảng 0,5%. Cổ phiếu nhỏ có tỷ trọng 0,1% tăng 10% chỉ đóng góp 0,01%. Vì vậy chỉ số có thể tăng mạnh chủ yếu nhờ vài cổ phiếu lớn trong khi đa số cổ phiếu nhỏ không tăng.
- Ở Việt Nam: các chỉ số của HOSE (VN30, VNMidcap, VNSmallcap, VNAllshare) tính theo vốn hoá điều chỉnh free float, có trần tỷ trọng 10% (không áp dụng cho các chỉ số ngành VNAllshare), rà soát định kỳ tháng 1 và tháng 7. Các bản factsheet của HOSE công bố hai con số vốn hoá (tổng vốn hoá và vốn hoá điều chỉnh free float); một bản cập nhật ghi 5.497.838 tỷ đồng so với 2.298.122 tỷ đồng. Cách tính của riêng VN-Index (có điều chỉnh free float hay không) tôi chưa xác minh được từ các nguồn tra cứu; hãy xem tài liệu phương pháp của HOSE.
- Bằng chứng thực nghiệm: nguồn tra cứu chủ yếu là bình luận của các hãng quản lý quỹ, không phải nghiên cứu học thuật. Fisher Investments cho rằng vốn hoá nhỏ vượt trội thường tập trung ở nhịp bật đầu của thị trường tăng sau đáy, rồi nhường chỗ cho vốn hoá lớn khi chu kỳ trưởng thành; Schwab (2024) ghi rằng lần dẫn dắt của vốn hoá lớn trong chu kỳ đó là khác thường so với lịch sử, vì trước đây vốn hoá nhỏ thường theo kịp hoặc vượt trội ở giai đoạn đầu. Nghĩa là thứ tự "lớn trước, nhỏ sau" không phải quy luật bền; các nguồn này còn mâu thuẫn nhau.
- Một nghiên cứu năm 2003 của tạp chí Journal of Investing mô tả "con lắc" quy mô, chu kỳ vốn hoá nhỏ gắn với chênh lệch giữa chỉ số bình quân đều và gia quyền vốn hoá (tôi chỉ đọc được tóm tắt).

**Liên hệ với bài học:** thầy giải thích bằng tỷ trọng: chỉ số tăng khi cổ phiếu nặng tăng, rồi nhà đầu tư tìm cổ phiếu "chưa tăng". Nên kiểm tra ý đó bằng dữ liệu nhiều giai đoạn thay vì coi là quy luật.

**Đọc thêm:** [The myth of small caps' superiority (Fisher Investments)](https://www.fisherinvestments.com/en-us/marketminder/the-myth-of-small-caps-superiority); [Market leadership shifts (Schwab Asset Management)](https://schwabassetmanagement.com/story/breadth-life-market-leadership-shifts); [HOSE factsheet, chỉ số vốn hoá (03/2025)](https://static2.vietstock.vn/vietstock/2025/3/13/20250312_form_factsheet_mcindices_eng_t03_2025.pdf); [HOSE factsheet VN (09/2021)](https://static2.vietstock.vn/vietstock/2021/9/21/20210921_Form_Factsheet_MCIndices_VN_T09.2021.pdf)

### Phân tích top-down và bottom-up, khung Thiên thời - Địa lợi - Nhân hoà, PEST

**Thầy nhắc ở:** B1 00:35, B1 02:46, B4 02:00 - slide doanh nghiệp, ngành, quốc gia, vĩ mô; thầy đề xuất kết hợp hai cách.

**Là gì:** Top-down bắt đầu từ vĩ mô và ngành rồi thu hẹp về doanh nghiệp; bottom-up bắt đầu từ doanh nghiệp bất kể bối cảnh. PEST là khung phân tích môi trường bên ngoài: Political (chính trị, pháp lý), Economic (kinh tế), Social (xã hội), Technological (công nghệ).

**Giải thích:**
- Top-down: đánh giá vĩ mô (tăng trưởng, lãi suất, tỷ giá), chọn ngành thuận lợi, rồi chọn cổ phiếu tốt trong ngành. Bottom-up: đọc báo cáo tài chính, lợi thế cạnh tranh, ban lãnh đạo, định giá từng công ty. Nhiều quỹ kết hợp: top-down để chọn ngành, bottom-up để chọn mã.
- PEST do Francis Aguilar đề xuất năm 1967 (còn gọi ETPS); biến thể PESTLE thêm pháp lý, môi trường. Phê bình: giúp giải thích quá khứ nhưng ít khi dự báo được tương lai vì môi trường vĩ mô biến động; liệt kê các yếu tố thì dễ, hiểu quan hệ nhân quả với kết quả kinh doanh mới khó.
- "Thiên thời, Địa lợi, Nhân hoà" là thành ngữ cổ Trung Hoa (thường dẫn từ sách Mạnh Tử: thiên thời không bằng địa lợi, địa lợi không bằng nhân hoà). Thầy mượn để xếp: thiên thời là vĩ mô và chu kỳ, địa lợi là ngành và vị thế cạnh tranh, nhân hoà là con người và quản trị; đây là cách ánh xạ theo ý thầy, tôi chưa kiểm chứng ngoài tra cứu này.
- Ví dụ áp dụng nhanh: một công ty xi măng: Political (đầu tư công, quy định môi trường), Economic (lãi suất, giá than, tín dụng bất động sản), Social (đô thị hoá), Technological (công nghệ lò nung, xi măng xanh). Từng gạch đầu dòng có thể gắn một giả định định lượng cho mô hình.

**Liên hệ với bài học:** hai cách top-down và bottom-up không loại trừ nhau; điều quan trọng thầy nhấn là thứ tự các lớp phân tích (quốc gia, ngành, doanh nghiệp) và việc mỗi lớp phải gắn với con số cụ thể.

**Đọc thêm:** [Top-down investment (AnalystPrep)](https://analystprep.com/study-notes/cfa-level-iii/top-down-investment); [Top down vs bottom up approach (Strike)](https://www.strike.money/stock-market/top-down-vs-bottom-up-investing); [PEST analysis (Wikipedia)](https://en.wikipedia.org/wiki/PEST_analysis)

### Phong cách đầu tư: tăng trưởng, giá trị, chất lượng, quy mô; growth stock

**Thầy nhắc ở:** B2 01:28, B2 03:23, B4 01:55 - slide "Growth is over-rated", bộ lọc tăng trưởng doanh thu.

**Là gì:** Phong cách đầu tư là cách phân nhóm cổ phiếu theo đặc tính: giá trị (value: P/B, P/E thấp), tăng trưởng (growth: doanh thu, lợi nhuận tăng nhanh, định giá cao), chất lượng (quality: lợi nhuận cao, ít nợ, lợi nhuận ổn định), quy mô (size: vốn hoá nhỏ hay lớn). Growth stock là cổ phiếu công ty tăng trưởng nhanh hơn thị trường.

**Giải thích:**
- Fama và French (1993) xây mô hình ba yếu tố (thị trường, quy mô, giá trị), mở rộng năm 2014 thành năm yếu tố (thêm lợi nhuận và đầu tư); Fama nhận Nobel năm 2013 một phần nhờ công trình về hiệu quả thị trường. Về sau thêm các yếu tố động lượng, chất lượng, biến động thấp.
- Bằng chứng: tại Mỹ, cổ phiếu giá trị (book-to-market cao) trung bình sinh lời hơn cổ phiếu tăng trưởng trong dài hạn, cả với vốn hoá lớn lẫn nhỏ, nhỏ hơn ở nhóm vốn hoá lớn (CFA Institute tóm tắt Fama và French 2006); nhưng giá trị kém trong thập niên 2010. Nguyên nhân phần thưởng giá trị vẫn tranh cãi: Fama và French cho rằng là phần bù rủi ro, người khác cho rằng là định giá sai do hành vi.
- Hiệu suất trong pha giảm: chưa tìm được nguồn đáng tin cho khẳng định "tăng trưởng giảm sâu hơn trong pha giảm" ở thị trường Việt Nam; hiểu biết chung là cổ phiếu định giá cao nhạy với lãi suất tăng, nhưng đây là lập luận chung.
- Bộ lọc tăng trưởng doanh thu: chọn công ty có doanh thu tăng, ví dụ trên 15% mỗi năm; hạn chế là doanh thu tăng bằng giảm giá hoặc đốt tiền không tạo giá trị (xem mục Unicorn).

**Liên hệ với bài học:** slide "Growth is over-rated" ngụ ý đừng trả giá quá cao cho tăng trưởng; học thuật không kết luận một phong cách thắng mãi mãi, thắng thua thay đổi theo chu kỳ.

**Đọc thêm:** [CFA Digest, value premium (Fama và French 2006)](https://rpc.cfainstitute.org/-/media/documents/article/cfa-digest/2007/dig-v37-n2-4606-pdf.pdf); [Can value factor investing be saved? (FTSE Russell)](https://www.lseg.com/en/insights/ftse-russell/can-value-factor-investing-be-saved); [Fama-French five-factor model (IFA)](https://www.ifa.com/videos/ifa-charts-fama-french-five-factor-model)

### Sức mạnh tương đối (relative strength) và Relative Rotation Graph (RRG)

**Thầy nhắc ở:** B2 01:09, B2 01:15 - chuẩn hoá chỉ số về 100, học viên so sánh với phần mềm Optuma.

**Là gì:** Sức mạnh tương đối so sánh hai chuỗi giá: tỷ số giá tài sản / giá chuẩn so sánh (chỉ số). RRG (Relative Rotation Graph) là biểu đồ do Julius de Kempenaer sáng lập, vẽ nhiều chứng khoán hoặc ngành lên mặt phẳng hai trục: JdK RS-Ratio (xu hướng tương đối) ngang và JdK RS-Momentum (động lượng của RS-Ratio) dọc, cắt nhau ở 100.

**Giải thích:**
- Chuẩn hoá về 100 tại một ngày gốc cho phép so các chuỗi có mức giá khác nhau. Ví dụ cổ phiếu 50.000 lên 55.000 (+10%), chỉ số 1.000 lên 1.050 (+5%). Đường sức mạnh tương đối = 1,10 / 1,05 x 100 = 104,8: cổ phiếu mạnh hơn chỉ số khoảng 4,8% kể từ ngày gốc.
- RS-Ratio trên 100: xu hướng tương đối đi lên; RS-Momentum trên 100: động lượng tăng. Bốn góc phần tư (theo quy ước phổ biến): Leading, Weakening, Lagging, Improving; điểm thường xoay theo chiều kim đồng hồ. Công thức chính xác của JdK là sở hữu riêng; tôi chưa tìm được công thức công bố, nên kết quả trên phần mềm khác nhau là bình thường (Optuma và StockCharts đều có bản của họ).
- Khác RSI: RSI (Relative Strength Index) đo động lượng riêng của một chuỗi giá (tỷ lệ phiên tăng so với giảm trong 14 phiên, thang 0 đến 100), không so với chuẩn; sức mạnh tương đối và RRG thì luôn so sánh với một chuẩn. Tên gọi dễ gây nhầm.
- Ở Việt Nam: chọn VN-Index làm chuẩn, các chỉ số ngành làm đối tượng; thanh khoản mỏng làm đường RS nhiễu hơn ở mã nhỏ.

**Liên hệ với bài học:** thầy dùng việc chuẩn hoá về 100 để so ngành với thị trường; học viên đối chiếu với Optuma, công cụ hiển thị RRG.

**Đọc thêm:** [Relative Rotation Graphs (Optuma)](https://www.optuma.com/kb/charts/relative-rotation-graphs-rrg); [Relative Rotation Graphs (StockCharts ChartSchool)](https://chartschool.stockcharts.com/table-of-contents/chart-analysis/chart-types/relative-rotation-graphs-rrg-charts); [RRG scripting guide (Optuma)](https://www.optuma.com/blog/scripting-for-rrgs)

## Cụm 6. Hành vi, kiểm nghiệm dữ liệu và các nhân vật mẫu

### Lý thuyết trò chơi (Game theory), cân bằng Nash, trò chơi tổng bằng không (Zero-sum)

**Thầy nhắc ở:** B15 01:30, B15 01:46, B15 01:49, B16 00:40, B16 01:40 - thầy vẽ ma trận bốn ô, phê bình là xa thực tiễn, nói tiền chỉ dịch từ người này sang người khác.

**Là gì:** Lý thuyết trò chơi nghiên cứu cách nhiều bên ra quyết định khi kết quả của mỗi bên phụ thuộc vào lựa chọn của bên kia. Cân bằng Nash là tình huống mà không ai có thể cải thiện kết quả của mình bằng cách tự đổi chiến lược khi các bên còn lại giữ nguyên. Trò chơi tổng bằng không là trò chơi trong đó phần được của người này đúng bằng phần mất của người kia.

**Giải thích:**
- Ma trận bốn ô là bảng kết quả cho hai người chơi, mỗi người có hai lựa chọn. Ví dụ kinh điển là thế lưỡng nan của người tù. Theo cách đặt điểm trong một tài liệu tra cứu: cả hai im lặng thì mỗi người được 2; cả hai khai thì mỗi người được 1; một người khai còn người kia im lặng thì người khai được 3 và người im lặng được 0. Kiểm tra: nếu bạn tôi khai, tôi khai được 1, im lặng được 0, nên tôi khai; nếu bạn tôi im lặng, tôi khai được 3, im lặng được 2, nên tôi vẫn khai. Cả hai cùng khai là cân bằng Nash (1, 1), dù cả hai im lặng sẽ tốt hơn cho cả hai (2, 2). Nghĩa là cân bằng Nash chưa chắc là kết quả tốt nhất chung.
- Trò chơi tổng bằng không: ví dụ tung đồng xu "ngửa khớp, sấp lệch": người thắng nhận 1, người thua mất 1, tổng luôn bằng 0. Ở trò chơi hai người tổng bằng không, cân bằng Nash có thể tìm bằng quy hoạch tuyến tính.
- Áp vào cổ phiếu: nếu A bán cho B ở giá 10.000 và sau đó giá lên 12.000, thì phần lãi 2.000 của B là phần A không có; xét riêng cặp giao dịch này, chênh lệch cộng lại bằng 0 trước phí. Nếu hai bên đều trả phí 0,2% trên 100 triệu, tổng thể thành âm 0,4 triệu. Đây là cách hiểu "tiền chỉ dịch từ người này sang người khác" của thầy, đúng cho giao dịch ngắn hạn thuần tuý.
- Giới hạn: thị trường không phải tổng bằng không khi nhìn dài hạn, vì doanh nghiệp tạo lợi nhuận, trả cổ tức và tăng giá trị cho người nắm giữ; ngoài ra thị trường có rất nhiều người chơi, quyết định không đồng thời, thông tin không đầy đủ, điểm thưởng không biết trước, và một trò chơi có thể có nhiều cân bằng. Vì vậy ma trận bốn ô là mô hình minh hoạ, không dự đoán được giá. Chưa tìm được nguồn bàn riêng về việc áp dụng ở thị trường Việt Nam; từ khoá gợi ý: "Keynes beauty contest", "game theory in financial markets".

**Liên hệ với bài học:** thầy vẽ ma trận để nói về đối thủ và đối ứng trong giao dịch, rồi phê bình rằng mô hình này xa thực tiễn: đúng ở điểm giả định người chơi hợp lý và biết điểm thưởng. Phân biệt ngắn hạn (gần với tổng bằng không) và dài hạn (có phần giá trị tạo ra) là chỗ thầy nhấn.

**Đọc thêm:** [Zero-sum game (Wikipedia)](https://en.wikipedia.org/wiki/Zero-sum_game); [Prisoner's Dilemma (Stanford Encyclopedia of Philosophy)](https://plato.stanford.edu/archives/spr2008/entries/prisoner-dilemma/); [Ghi chú giảng về cân bằng Nash và trò chơi tổng bằng không (QMUL)](https://webspace.maths.qmul.ac.uk/felix.fischer/teaching/opt/notes/notes9.pdf)

### Tài chính hành vi (Behavioral finance), FOMO, ác cảm thua lỗ (Loss aversion)

**Thầy nhắc ở:** B13 01:35, B15 00:05, B15 01:30 - học viên đề xuất học kèm kỹ thuật, thầy cho là chưa đủ, và gọi tên nỗi sợ bỏ lỡ.

**Là gì:** Tài chính hành vi nghiên cứu cách tâm lý và thiên kiến làm quyết định đầu tư lệch khỏi mô hình "con người hoàn toàn hợp lý". Ác cảm thua lỗ là xu hướng cảm nhận khoản lỗ nặng hơn khoản lãi cùng độ lớn. FOMO (fear of missing out) là nỗi sợ bỏ lỡ cơ hội khi thấy người khác kiếm được tiền, thúc đẩy mua đuổi.

**Giải thích:**
- Tác giả tiêu biểu: Daniel Kahneman và Amos Tversky, bài "Prospect Theory: An Analysis of Decision under Risk" đăng trên Econometrica năm 1979. Hàm giá trị của họ có ba đặc điểm: lõm với phần lãi, lồi với phần lỗ, và dốc hơn với phần lỗ so với phần lãi; xác suất thấp bị đánh giá quá cao, còn kết quả chắc chắn được ưu ái. Kahneman nhận Nobel Kinh tế năm 2002 (thông tin này tôi nêu từ hiểu biết chung, chưa kiểm trong lần tra cứu này). Robert Shiller với "Irrational Exuberance" thường được dẫn khi nói tâm lý đám đông có thể là nguyên nhân lớn của biến động giá.
- Hệ số ác cảm thua lỗ: con số 2,25 hay được trích từ bài của Tversky và Kahneman năm 1992 (mẫu 25 sinh viên cao học, chọn tình huống giả định, tiền nhỏ); nguồn khác chỉ ra bài 1979 chưa ước lượng hệ số cụ thể. Một phân tích tổng hợp (Brown, Imai, Vieider, Camerer) cho trung bình khoảng 1,955, khoảng tin cậy 95% từ 1,820 đến 2,102. Nhìn chung nên hiểu là "lỗ nặng gấp đôi lãi" tuỳ người, tuỳ bối cảnh, không phải hằng số.
- Ví dụ số: tung đồng xu, thua mất 100 hoặc thắng X, xác suất mỗi bên 50%. Người có hệ số 2 chỉ chấp nhận khi X lớn hơn 200; hệ số 2,25 thì cần X lớn hơn 225. Vì thế nhiều người từ chối cược "thắng 150, thua 100" dù kỳ vọng toán dương (+25).
- FOMO và bầy đàn: Morningstar mô tả FOMO là một dạng hành vi bầy đàn có thể đẩy giá và tạo bong bóng; một nghiên cứu năm 2022 trên tạp chí International Journal of Emerging Markets xét vai trò trung gian của FOMO giữa bầy đàn, ác cảm thua lỗ và quyết định của nhà đầu tư cá nhân. Bằng chứng ở đây mang tính khảo sát, không phải bằng chứng nhân quả.
- Ở Việt Nam, tỷ trọng nhà đầu tư cá nhân lớn thường được dẫn như lý do tâm lý đám đông quan trọng; tôi chưa tìm được nguồn định lượng đáng tin trong lần tra cứu này.

**Liên hệ với bài học:** khi học viên đề xuất học thêm kỹ thuật, thầy cho rằng chưa đủ vì lỗ hổng nằm ở kỷ luật và cảm xúc: biết điểm cắt lỗ mà không dám cắt (ác cảm thua lỗ), biết giá đã cao mà vẫn mua (FOMO). Khác với nghĩa phổ thông: trong học thuật, đây là các thiên kiến có đo lường được, không phải lời trách "thiếu bản lĩnh".

**Đọc thêm:** [Prospect Theory (Econometrica, 1979)](https://www.econometricsociety.org/publications/econometrica/1979/03/01/prospect-theory-analysis-decision-under-risk); [Bản PDF bài 1979 (Princeton)](https://kahneman.scholar.princeton.edu/document/11); [Loss aversion và cuộc tranh luận về mức độ (Atticus Li)](https://atticusli.com/replication-crisis/loss-aversion/); [Hệ số loss aversion (Munich)](https://epub.ub.uni-muenchen.de/75121/1/275.pdf); [How herding leads to market bubbles (Morningstar)](https://www.morningstar.com/financial-advisors/how-herding-leads-market-bubbles); [Herding, loss aversion và FOMO ở nhà đầu tư cá nhân (Emerald)](https://emerald.com/insight/content/doi/10.1108/IJOEM-08-2020-0933/full/html)

### Tài chính hành vi và các hiệu ứng mùa vụ (Calendar effect, Sell in May, Tax-loss selling, hiệu ứng tháng Giêng, mua tin đồn bán sự thật, Contrarian)

**Thầy nhắc ở:** B7 03:13, B7 03:52, B9 01:40, B11 00:25 - khẩu quyết "giá cả là tâm lý, giá trị là nền tảng", "thứ Hai mua, thứ Sáu bán".

**Là gì:** Hiệu ứng mùa vụ (calendar effect) là các khuôn mẫu lặp lại của lợi suất theo thời điểm: tháng trong năm, ngày trong tuần, quanh kỳ nghỉ lễ. Tên hay gặp: hiệu ứng tháng Giêng (cổ phiếu nhỏ tăng đầu năm, một phần được giải thích bằng bán cắt lỗ thuế cuối năm rồi mua lại), Sell in May (nắm cổ phiếu từ tháng 11 đến tháng 4, tránh mùa hè), hiệu ứng ngày trong tuần. "Mua tin đồn, bán sự thật" là câu nói giá thường tăng trước tin tốt và giảm khi tin chính thức ra. Contrarian là đầu tư ngược số đông.

**Giải thích:**
- Bằng chứng thống kê và rủi ro đào dữ liệu: Sullivan, Timmermann và White (Journal of Econometrics, 2001) dùng 100 năm dữ liệu ngày và thấy rằng dù từng quy tắc lịch riêng lẻ có ý nghĩa thống kê rất cao, chúng không còn đáng kể khi so với toàn bộ tập quy tắc mà người ta có thể đã thử. Lý do: thử càng nhiều quy tắc, càng dễ gặp quy tắc "đẹp" do ngẫu nhiên. Ví dụ số: thử 100 quy tắc độc lập ở mức ý nghĩa 5% thì kỳ vọng khoảng 5 quy tắc có ý nghĩa thuần do may rủi; xác suất có ít nhất một quy tắc như vậy là 1 - 0,95^100, khoảng 99,4%.
- Nhưng kết luận không thống nhất: một nghiên cứu khác cho rằng lập luận đào dữ liệu không áp dụng cho Sell in May vì đây không phải một quy tắc lấy ngẫu nhiên từ nhiều quy tắc lịch, và hiệu ứng mạnh ở các nước châu Âu; khảo sát của CXO Advisory ghi hiệu ứng tháng Giêng của cổ phiếu nhỏ còn nhưng đã dịch sang tháng 12, và hiệu ứng đầu cuối tháng còn với một chút "đi trước". Cả hai bên đều cảnh báo thiên kiến đào dữ liệu.
- Ở Việt Nam: bài của VnBusiness ghi từ năm 2000 VN-Index tháng 12 tăng trung bình cao nhất (3,45%), tháng 1 đứng thứ hai (2,82%); nhưng tháng 1 các năm 2020 đến 2022 đều giảm 1 đến 4% và tháng 1/2023 tăng 10,3%; tháng 1/2002 và 1/2008 là hai tháng giảm mạnh nhất. Một chuyên gia được dẫn cho rằng số liệu quá ngắn. Học thuật Việt Nam có các nghiên cứu về hiệu ứng ngày trong tuần, Halloween (Friday và Hoang, 2015) và trước Tết âm lịch; tôi chưa tìm được kết luận chung của chúng, nên không khẳng định.
- "Thứ Hai mua, thứ Sáu bán" là cách nói của thầy về hiệu ứng ngày trong tuần; tôi chưa tìm được nguồn xác nhận quy tắc này đúng ở Việt Nam.

**Liên hệ với bài học:** câu "giá cả là tâm lý, giá trị là nền tảng" ghép với hiệu ứng mùa vụ: thầy dùng chúng như gợi ý về nhịp, không như công thức. Cách an toàn là coi chúng là giả thuyết cần kiểm nghiệm trên dữ liệu ngoài mẫu (xem mục thiên kiến nhìn trước) chứ không phải quy luật.

**Đọc thêm:** [The dangers of data-driven inference: calendar effects (LSE Research Online)](https://researchonline.lse.ac.uk/id/eprint/119142); [Bản thảo thảo luận 304 (FMG)](https://www.fmg.ac.uk/sites/default/files/2020-11/dp304.pdf); [Khảo sát các hiệu ứng lịch (CXO Advisory)](https://www.cxoadvisory.com/?p=11987); [Có hay không hiệu ứng tháng Giêng năm 2024 (VnBusiness)](https://vnbusiness.vn/co-hay-khong-hieu-ung-thang-gieng-nam-2024.html)

### Phản ứng giá quanh ngày công bố kết quả kinh doanh (Earnings reaction, giá đi trước tin)

**Thầy nhắc ở:** B9 02:40 - thầy nói thị trường Mỹ hay xả trước ba ngày.

**Là gì:** Giá cổ phiếu thường di chuyển quanh ngày công bố lợi nhuận, và có thể đã dịch chuyển trước ngày đó (do kỳ vọng, rò rỉ, hoặc người nắm thông tin giao dịch trước). Hiện tượng ngược là giá còn tiếp tục trôi cùng hướng với bất ngờ sau ngày công bố (post-earnings-announcement drift, PEAD), do Ball và Brown ghi nhận năm 1968.

**Giải thích:**
- Đo bất ngờ lợi nhuận: bất ngờ = (EPS thực - EPS kỳ vọng) / |EPS kỳ vọng|. Ví dụ EPS thực 1,10 so với kỳ vọng 1,00 là bất ngờ +10%. Phản ứng giá thường đo bằng lợi suất vượt trội: cổ phiếu +6% khi chỉ số +1% thì lợi suất vượt trội +5%.
- Giá đi trước tin: một bài nghiên cứu (SBFC 2025) lập luận phần đáng kể của "bất ngờ" đã được phản ánh trước khi công bố (pre-PEAD), và một nghiên cứu khác của Martineau ("Rest in Peace Post-Earnings Announcement Drift") cho rằng cả trôi trước và trôi sau công bố đã yếu đi nhiều theo thời gian ở thị trường Mỹ.
- Câu "xả trước ba ngày" của thầy: tôi chưa tìm được nguồn đo đúng con số ba ngày; các nghiên cứu trên chỉ cho thấy giá di chuyển trước công bố là có thật nhưng độ lớn và thời gian thay đổi theo mẫu và thời kỳ.
- Ở Việt Nam, chưa tìm được nghiên cứu cụ thể về phản ứng giá quanh công bố kết quả; lưu ý chung là thông tin kết quả sơ bộ, hội nghị nhà đầu tư và tin đồn thường lan trước báo cáo chính thức, nên "giá đi trước" khó tách khỏi nhiễu.

**Liên hệ với bài học:** điều thầy muốn nói là đừng chờ tin ra mới hành động vì giá có thể đã phản ánh; kết hợp với câu "mua tin đồn, bán sự thật". Đây là quan sát kinh nghiệm cần kiểm nghiệm, không phải quy luật.

**Đọc thêm:** [Post-earnings-announcement drift (Wikipedia)](https://EN.wikipedia.com/wiki/Post-earnings-announcement_drift); [Rest in Peace Post-Earnings Announcement Drift (Martineau)](https://cfr.ivo-welch.info/published/papers/martineau2021rest.pdf); [Bài thảo luận về trôi giá trước công bố (SBFC 2025)](https://sbfc.sydney.edu.au/2025/papers/SBFC2025_2E2_P113.pdf); [Bài thảo luận (Univ. Graz, 2020)](https://static.uni-graz.at/fileadmin/sowi/Working_Paper/2020-04_Fink.pdf)

### Tâm lý bầy đàn trong định giá: Seeking Alpha, quant

**Thầy nhắc ở:** B2 03:30 - thầy giải thích giản lược.

**Là gì:** Bầy đàn (herding) là hành vi làm theo số đông thay vì phân tích độc lập. Seeking Alpha là trang đầu tư có "Quant Rating", một hệ thống xếp hạng cổ phiếu bằng mô hình định lượng.

**Giải thích:**
- Theo trang trợ giúp của Seeking Alpha: mỗi cổ phiếu được chấm theo năm yếu tố: giá trị, tăng trưởng, lợi nhuận, động lượng và điều chỉnh dự báo EPS; hơn 100 chỉ tiêu được chấm so với các cổ phiếu cùng ngành, gộp thành năm điểm A+ đến F, rồi thành điểm Quant (Strong Buy đến Strong Sell). Cập nhật mỗi ngày trước giờ mở cửa, phủ khoảng 5.600 mã. Công thức đầy đủ không công khai.
- Liên hệ với bầy đàn: đây là cách thầy giản lược việc nhiều nhà đầu tư và nhiều mô hình cùng dùng bộ yếu tố giống nhau (giá trị, tăng trưởng, động lượng, điều chỉnh dự báo) nên có thể cùng mua, cùng bán một nhóm mã; khi mọi người dùng cùng tín hiệu, tín hiệu dễ bị "đông đúc". Đây là cách hiểu của tôi từ ngữ cảnh ngắn, tôi chưa tìm được lời thầy cụ thể hơn.
- Hạn chế: nguồn tra cứu chủ yếu là trang giới thiệu của chính Seeking Alpha, chưa có đánh giá độc lập mạnh trong kết quả.

**Liên hệ với bài học:** thầy dùng ví dụ để cảnh báo rằng định giá bằng mô hình số cũng có thể phản ánh tâm lý chung của thị trường. Hãy coi điểm quant như một lát cắt dữ liệu, không phải đáp án.

**Đọc thêm:** [What are Quant Ratings (Seeking Alpha Help)](https://help.seekingalpha.com/premium/what-are-quant-ratings-and-how-do-i-use-them); [How herding leads to market bubbles (Morningstar)](https://www.morningstar.com/financial-advisors/how-herding-leads-market-bubbles)

### Thiên kiến nhìn trước (Look-ahead bias)

**Thầy nhắc ở:** B3 03:18 - thầy giải thích bằng ví dụ dùng dữ liệu cuối năm để đánh giá quyết định đầu năm.

**Là gì:** Thiên kiến nhìn trước là lỗi khi kiểm nghiệm lại (backtest) hoặc phân tích mà dùng thông tin chưa thể biết tại thời điểm ra quyết định.

**Giải thích:**
- Ví dụ kinh điển: giả định lợi nhuận quý được biết ngay ngày cuối quý, trong khi báo cáo thực ra công bố vài tuần sau. Ví dụ ở Việt Nam: backtest "mua ngày 02/01/2020 những mã có EPS năm 2020 cao nhất" là sai, vì EPS cả năm 2020 chỉ biết sau khi báo cáo được công bố vào đầu năm 2021. Ví dụ thầy dùng (dữ liệu cuối năm đánh giá quyết định đầu năm) cùng loại.
- Cách tránh: chỉ dùng dữ liệu có sẵn tại từng thời điểm (point-in-time) và dùng đúng ngày công bố, không dùng ngày kết thúc kỳ; tránh dùng giá đóng cửa hôm nay để vừa tạo tín hiệu vừa khớp lệnh ngay giá đóng cửa đó; cẩn thận với chỉ báo tự "vẽ lại" quá khứ; kiểm tra trên dữ liệu chưa thấy (out of sample); coi kết quả đẹp bất thường là dấu hiệu cảnh báo.
- Ở Việt Nam, hạn công bố báo cáo và số liệu bị điều chỉnh sau kiểm toán là chỗ dễ gây lỗi; cần dữ liệu có ngày công bố thật. Tôi chưa tìm được nguồn chuyên về chủ đề này cho thị trường Việt Nam.

**Liên hệ với bài học:** lỗi này giải thích vì sao nhiều "chiến lược" nghe hiệu quả trên giấy lại thất bại khi dùng thật; thầy đưa ví dụ để nhắc người học đặt mình vào thời điểm ra quyết định, không phải thời điểm đã biết kết quả.

**Đọc thêm:** [Look-ahead bias (Corporate Finance Institute)](https://corporatefinanceinstitute.com/resources/capital_markets/look-ahead-bias/); [Backtesting biases and how to avoid them (Auquan)](https://medium.com/auquan/backtesting-biases-and-how-to-avoid-them-776180378335)

### Quant Trading của Hoàng Tùng

**Thầy nhắc ở:** B17 03:20 - học viên giơ bìa sách, thầy thấy giống bài giảng.

**Là gì:** Cuốn "Quant Trading - Đầu tư Chứng khoán dưới Góc nhìn Khoa học" của tác giả Hoàng Tùng, giới thiệu đầu tư định lượng cho người đọc Việt Nam.

**Giải thích:** Theo tóm tắt đánh giá trong kết quả tìm kiếm, đây là sách mỏng, mang tính dẫn nhập, dễ đọc, dùng như sổ tay hơn là giáo trình mô hình toán. Chưa tìm được thông tin chắc chắn về nhà xuất bản, năm phát hành và nội dung từng chương: nên kiểm tra trên trang sách hoặc nhà xuất bản trước khi mua. Muốn hiểu sâu hơn về giao dịch định lượng bằng tiếng Anh, cuốn "Quantitative Trading" của Ernest Chan thường được giới thiệu.

**Liên hệ với bài học:** thầy thấy sách giống bài giảng nghĩa là cùng cách tiếp cận khoa học, có kiểm nghiệm; các mục về look-ahead bias và hiệu ứng mùa vụ ở phụ lục này là các lỗi phổ biến của cách tiếp cận đó.

**Đọc thêm:** [Quant Trading, Hoàng Tùng (Goodreads)](https://www.goodreads.com/book/show/54203069-quant-trading-u-t-ch-ng-kho-n-d-i-g-c-nh-n-khoa-h-c); [Quantitative trading là gì (DSC)](https://www.dsc.com.vn/kien-thuc/quantitative-trading-la-gi)

### Warren Buffett và Bill Gates: triết lý đầu tư giá trị, kế hoạch thừa kế

**Thầy nhắc ở:** B1 00:32, B4 00:10 - thầy kể Buffett không dùng máy tính, nắm giữ 5-10-20 năm, các tỷ phú để lại cho con rất ít.

**Là gì:** Warren Buffett là chủ tịch kiêm CEO của Berkshire Hathaway, nhà đầu tư giá trị nổi tiếng. Bill Gates là đồng sáng lập Microsoft, nhà từ thiện. Hai người đồng khởi xướng Giving Pledge năm 2010.

**Giải thích:**
- Tiểu sử và triết lý: Buffett học khoá của Benjamin Graham tại Columbia năm 1951 (trang của Columbia Business School), sau đó làm việc ở công ty của Graham; một nguồn ghi Graham từ chối lần đầu rồi nhận ông năm 1954. Cốt lõi của Graham là mua chứng khoán rẻ hơn giá trị thật có biên an toàn (xem mục Net-net). Buffett khuyên chỉ đầu tư vào việc mình hiểu, gọi là vòng tròn năng lực (circle of competence), và ông tránh phần lớn cổ phiếu công nghệ.
- Chuyện "không dùng máy tính": Business Insider (2013) viết ông không có máy tính ở bàn làm việc; một bài năm 2011 cho biết ông dùng máy tính ở nhà để nghiên cứu, viết và chơi bridge trực tuyến; Fortune ghi ông không dùng điện thoại thông minh và tính nhẩm nhiều. Các nguồn từ 2006 đến 2017, thói quen hiện tại có thể đã khác. Ý đúng là ông không dựa vào mô hình bảng tính phức tạp; không nên hiểu là ông không dùng công nghệ.
- Nắm giữ "5-10-20 năm": hợp với triết lý nắm giữ dài hạn doanh nghiệp tốt; tôi chưa tìm được nguồn xác nhận một câu cụ thể thầy trích.
- Giving Pledge: ra mắt năm 2010, cam kết tặng phần lớn tài sản trong lúc sống hoặc theo di chúc. Theo Fortune, thư cam kết của Buffett nêu trên 99% tài sản sẽ được tặng; cũng theo Fortune, năm 1986 ông nói sẽ để lại cho con "đủ tiền để cảm thấy có thể làm mọi thứ, nhưng không nhiều tới mức không làm gì" (các nguồn ghi câu này hơi khác nhau về chữ). Wikipedia ghi ông chuyển 500 triệu USD vào quỹ của mỗi người trong ba người con. Số người ký lệch giữa các nguồn: trang Giving Pledge ghi 183 cá nhân từ 22 quốc gia, Wikipedia (tháng 8/2025) ghi 256; chênh lệch do ngày cập nhật.
- Gates: nhiều nguồn dẫn ông nói mỗi người con sẽ nhận khoảng 10 triệu USD, dưới 1% tài sản, vì "không phải một triều đại" và để không làm hại con; ly hôn năm 2021, một số bài cho rằng kế hoạch vẫn nhất quán. Số tài sản thay đổi theo từng năm.

**Liên hệ với bài học:** thầy dùng Buffett để minh hoạ đầu tư giá trị dài hạn và việc tự hiểu doanh nghiệp, còn các tỷ phú để lại ít cho con để nói về cách nhìn tiền và thừa kế. Lưu ý: các chi tiết thầy kể là giai thoại chung; phụ lục này chỉ xác nhận phần có nguồn.

**Đọc thêm:** [History of Value Investing (Columbia Business School)](https://business.columbia.edu/heilbrunn/about/valueinvestinghistory); [Warren Buffet made value investing sexy (Quartz)](https://qz.com/warren-buffet-value-investing-benjamin-graham); [Buffett's office tour (Business Insider)](https://businessinsider.in/take-a-tour-of-warren-buffetts-office-at-berkshire-hathaway/articleshow/22165648.cms); [Timeless wisdom from Warren Buffett (Value Research)](https://www.valueresearchonline.com/stories/49632/timeless-wisdom-from-warren-buffett/); [Giving Pledge, thư của Warren Buffett](https://givingpledge.org/pledge/warren-buffett/); [The $600 billion challenge (Fortune, 2010)](https://fortune.com/2010/06/16/the-600-billion-challenge/); [Con của Buffett sẽ nhận gì (Fortune, 2022)](https://dc.fortune.com/2022/07/09/warren-buffett-pledged-to-give-away-his-96-billion-fortune-what-will-his-three-children-get); [Vì sao con của Gates không thừa kế nhiều (IBTimes)](https://ibtimes.com/heres-why-bill-gates-kids-wont-inherit-much-his-multibillion-dollar-fortune-3145670); [Gates, thừa kế và từ thiện (Fortune, 2025)](https://dc.fortune.com/2025/03/31/bill-gates-children-inheritence-microsoft-fortune-philanthropy/)

## Lời kết

Các mục trong phụ lục này nối với nhau theo một chuỗi: giá trị thời gian của tiền và tỷ lệ chiết khấu dẫn tới các mô hình định giá (DDM, bội số, Graham); lý thuyết danh mục và thống kê cho thấy cách đo rủi ro và đa dạng hoá; quản trị vốn biến các con số đó thành quy tắc vào lệnh và cắt lỗ; ngành, chu kỳ và dòng tiền là bối cảnh; cuối cùng, hành vi và kiểm nghiệm dữ liệu nhắc rằng mọi công thức đều chạy qua con người và dữ liệu có thể sai lệch. Điểm chung nên mang theo là: mỗi công thức có giả định, ví dụ số trong phụ lục là số giả định để tự kiểm lại, và các giới hạn ở thị trường Việt Nam được ghi rõ ở từng mục là chỗ cần tự kiểm chứng bằng dữ liệu địa phương. Phụ lục không phải lời khuyên đầu tư.
