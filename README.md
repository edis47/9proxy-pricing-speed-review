# đánh giá 9proxy: giá từng gói, tốc độ thực tế và có đáng mua cho MMO, nuôi tài khoản?

Người tìm cụm "đánh giá 9proxy" thường đã đi qua vài diễn đàn MMO, thấy tiêu đề kiểu "$0.018/IP" rồi tự hỏi ba chuyện: dịch vụ này có thật không, giá thật là bao nhiêu, và lỡ mua rồi có xin lại được tiền không. Bài này trả lời đúng ba câu đó, cộng thêm phần giá từng gói và những phản hồi trái chiều đang có trên mạng.

## 9Proxy bán cái gì (và không bán cái gì)

9Proxy là nhà cung cấp proxy dân cư (residential proxy) — tức là IP lấy từ kết nối internet gia đình thật, không phải IP datacenter. Con số họ công bố là hơn 20 triệu IP dân cư trải trên 90+ quốc gia, hỗ trợ HTTP/HTTPS và SOCKS5, target được theo quốc gia, bang/tỉnh, thành phố, ZIP code và cả ISP.

Điểm dễ gây sốc nhất với người mới: **bạn không nhận được danh sách IP:port**. 9Proxy chạy qua phần mềm riêng và dashboard, không bán kiểu "đây là 100 dòng IP, tự nhập vào tool". Vài người dùng trên Trustpilot phàn nàn chính vì chuyện này — họ mua, mở ra không thấy file danh sách, đòi hoàn tiền và bị từ chối. Phía 9Proxy trả lời rằng cách làm này được nêu rõ trong FAQ và đem lại ổn định hơn danh sách tĩnh. Dù bạn đứng về phía nào, hãy biết trước: nếu quy trình của bạn bắt buộc phải có file IP:port, 9Proxy không phải lựa chọn phù hợp.

Các cách truy cập:

- **Proxy Program** — client Windows chạy ở tầng hệ điều hành, dùng cho phần mềm không hỗ trợ proxy.
- **Proxy2Web** — không cần cài, đăng nhập user:pass là dùng, hợp để kiểm tra nhanh trên trình duyệt.
- **ProxyHub / ProxyHub Lite / Pro** — quản lý proxy trên thiết bị di động.
- **API + SOCKS5** — dùng cho automation, kết nối với trình duyệt antidetect, proxychains hay script Python.

Ngoài ra có gói Enterprise với team mode (1 owner + tối đa 5 thành viên), chia sẻ lưu lượng không hết hạn trong nội bộ nhóm, và hệ thống sub-account/share code để nhiều người dùng chung một tài khoản.

## Ba kiểu tính tiền: chọn sai kiểu là tốn tiền vô ích

Đây là phần quan trọng nhất, và cũng là chỗ nhiều bài review nói lướt.

**Gói theo IP — băng thông không giới hạn.** Bạn mua một số lượng IP cố định, dùng bao nhiêu dữ liệu cũng được. Đổi lại, mỗi IP chỉ sống từ vài giờ đến tối đa khoảng 24 giờ. Nghĩa là mua 100 IP rồi để đó ba tuần là tiền bốc hơi. Kiểu gói này hợp với phiên làm việc dài, tải nặng, hoặc khi bạn không đoán được lưu lượng.

**Gói theo GB — trả tiền theo dung lượng.** Không giới hạn số lượng endpoint, muốn tạo bao nhiêu cũng được, xoay IP mỗi request hoặc giữ sticky theo phút. Hạn dùng 180 ngày cho các gói thường, và vô thời hạn với gói dung lượng lớn/Enterprise. Hợp với việc xoay liên tục nhưng mỗi request ít dữ liệu.

**Gói bundle — IP + GB trong một gói.** Dành cho ai vừa cần IP ổn định cho vài việc, vừa cần lưu lượng cho việc khác.

Nói cách khác: cùng một người, cùng một nhu cầu, chọn đúng kiểu gói có thể rẻ hơn đáng kể so với chọn sai. Trước khi trả tiền, bạn nên tự trả lời: công việc của tôi giữ một IP lâu hay xoay liên tục?

## Bảng giá gói theo IP

Giá bên dưới lấy từ các bài công bố gần đây (bài đánh giá năm 2026 của Geekflare và tài liệu đối tác cập nhật tháng 5/2026). 9Proxy đã điều chỉnh giá ít nhất một lần, nên các bài cũ hơn vẫn đang lan truyền mức $20/100 IP — thấp hơn giá hiện hành.

| Gói | Đơn giá | Tổng | Ghi chú |
| --- | --- | --- | --- |
| 100 IP | ~$0.24/IP | $24 | Mức thử nghiệm |
| 500 IP | ~$0.144/IP | $72 | Dùng cá nhân, việc nhẹ |
| 1.000 IP + tặng 500 IP | ~$0.084/IP | $126 | Nhóm nhỏ |
| 2.500 IP | ~$0.084/IP | $210 | Nhiều dự án song song |
| 5.000 IP | ~$0.072/IP | $360 | Agency quy mô vừa |
| 15.000 IP | ~$0.048/IP | $720 | Doanh nghiệp nhiều khu vực |
| 25.000 IP | ~$0.035/IP | $863 | Reseller, lab automation |
| 50.000 IP | ~$0.029/IP | $1.438 | Vận hành khối lượng lớn |
| 100.000 IP | — | ~$2.300 | Mức bán buôn |
| 500.000 IP | — | ~$8.625 | Mức bán buôn |

👉 [Xem giá gói IP hiện tại và tự chọn số lượng IP](https://bit.ly/9-Proxy)

Băng thông trong gói IP không giới hạn, nhưng đừng quên giới hạn thật sự nằm ở tuổi thọ IP và số phiên bạn cần tách riêng.

## Bảng giá gói theo GB

| Gói | Đơn giá | Tổng | Hạn dùng |
| --- | --- | --- | --- |
| 5 GB | $3.00/GB | $15 | 180 ngày |
| 50 GB + tặng 5 GB | $2.10/GB | $105 | 180 ngày |
| 100 GB | $1.50/GB | $150 | 180 ngày |
| 200 GB | $1.00/GB | $200 | 180 ngày |
| 1.000 GB | $0.80/GB | $800 | 180 ngày |
| 2.000 GB | $0.75/GB | $1.500 | 180 ngày |
| 6.000 GB | $0.70/GB | $4.200 | Không giới hạn |
| 10.000 GB | $0.68/GB | $6.800 | Không giới hạn |

👉 [Chọn gói GB theo đúng lưu lượng bạn tiêu mỗi tháng](https://bit.ly/9-Proxy)

Mức $0.68/GB ở đầu bảng giá này là con số mà nhiều nơi quảng cáo là "giá khởi điểm" — thực tế nó chỉ đạt được ở gói 10.000 GB. Gói nhỏ nhất tính ra $3.00/GB, gấp hơn bốn lần. Đó không phải chiêu trò riêng của 9Proxy, nhưng bạn nên biết mình đang so sánh cái gì khi thấy bảng so sánh giữa các nhà cung cấp.

## Bảng giá gói bundle

| Gói | Nội dung | Giá tham khảo | Hợp với |
| --- | --- | --- | --- |
| Starter | 100 IP + 5 GB | ~$30 | Dự án nhỏ, thử trước khi mở rộng |
| Growth | 1.500 IP + 50 GB | ~$180 | Agency vài khách hàng active |
| Pro | 5.000 IP + 500 GB | ~$720 | Vận hành khối lượng lớn, gói "all-in" |

👉 [Kiểm tra giá bundle và ưu đãi đang chạy trên trang chính thức](https://bit.ly/9-Proxy)

Lưu lượng trong bundle cũng có hạn 180 ngày. Con số bundle thay đổi giữa các nguồn (một số bài cũ ghi $25/$150/$600), nên hãy xác nhận trên trang giá trước khi thanh toán.

## Ba con số nên nhớ: 60 giây, Today List và 180 ngày

**60 giây** là chính sách thay IP: nếu một IP die sau khi cấp, bạn được đổi thủ công miễn phí trong vòng 60 giây đầu. Kèm theo đó là tính năng auto-refresh tự phát hiện và thay IP offline trong khoảng 60 giây.

**Today List** cho phép dùng lại miễn phí những IP đã dùng trong 24 giờ trước. Với công việc lặp lại theo ngày, tài liệu đối tác của 9Proxy ước tính cách này tiết kiệm 20–30% chi phí IP. Nghe hợp lý về mặt logic: IP cũ vẫn sạch thì không có lý do gì phải mua IP mới.

**180 ngày** là hạn dùng của gói GB thường và lưu lượng trong bundle. Đây là điểm đáng giá nếu bạn làm theo dự án không đều — mua 200 GB rồi dùng trong 5 tháng vẫn còn hiệu lực, thay vì bị reset theo tháng như nhiều dịch vụ khác.

## Tốc độ và tỷ lệ thành công: nên tin con số nào

Các bên đánh giá độc lập đưa ra kết quả không hoàn toàn giống nhau:

- Một bài test dài một tháng ghi nhận khoảng 12 triệu request, tỷ lệ thành công ~99,5% và thời gian phản hồi trung bình ~0,6 giây, đỉnh 600–700 request/phút trên một số target.
- Danh bạ ProxyLook lại ghi tỷ lệ thành công 97% và độ trễ khoảng 1.300 ms, kèm đánh giá tổng 3,9/5.
- Một bài so sánh phân khúc giá xếp 9Proxy vào nhóm ngân sách thấp, với tỷ lệ thành công 99%+ trên target "dễ" nhưng tụt xuống 70–85% trên target khó (các nền tảng chống bot gắt).

Chênh lệch này bình thường với proxy dân cư: kết quả phụ thuộc vào target và thời điểm test hơn là vào nhà cung cấp. Kết luận thực dụng: đừng mua gói 50.000 IP dựa trên bảng benchmark của người khác. Mua gói nhỏ nhất, test đúng website bạn cần, rồi mới mở rộng.

👉 [Tạo tài khoản và test với gói nhỏ trước](https://bit.ly/9-Proxy)

## Dùng 9Proxy cho việc gì ở Việt Nam

Nhóm dùng phổ biến vẫn là MMO và vận hành nhiều tài khoản: nuôi và quản lý nhiều profile Facebook/TikTok, mở nhiều shop trên các sàn, kiểm tra giá và tồn kho, theo dõi thứ hạng từ khóa, xác minh quảng cáo theo khu vực, và các công việc crawling dữ liệu.

Vài lưu ý thực tế:

- Trình duyệt antidetect như Dolphin Anty hay AdsPower được người dùng nhắc đến khi nói về 9Proxy — đây là combo phổ biến vì 9Proxy hỗ trợ SOCKS5 gốc, không cần ép protocol.
- Proxy dân cư không phải VPN. Nó không mã hóa toàn bộ traffic máy bạn và không phải công cụ để "ẩn danh tuyệt đối".
- Streaming không phải điểm mạnh. Một bài đánh giá trên iTWire ghi nhận 9Proxy vượt được kiểm tra của một số nền tảng thương mại điện tử nhưng có thể bị phát hiện trên Netflix. Nếu nhu cầu chính của bạn là xem nội dung chặn vùng, tiền đó nên tiêu ở chỗ khác.
- Chất lượng IP theo khu vực không đồng đều. Có người dùng phản ánh chọn IP New York nhưng công cụ check hiển thị một thành phố khác ở Texas — chênh lệch cơ sở dữ liệu geolocation là chuyện có thật, nhưng nếu bạn làm việc cần đúng thành phố thì phải test trước.

## Phản hồi người dùng: phần khó đọc nhưng cần đọc

Đây là chỗ nhiều bài "đánh giá" kiểu quảng cáo bỏ qua: **9Proxy có điểm rất thấp trên một số nền tảng đánh giá**.

Trên trang Trustpilot, 9Proxy bị chấm mức 2/5. Các phàn nàn lặp lại gồm: từ chối hoàn tiền khi khách đổi ý, hỗ trợ không đủ kiên nhẫn với người mới, IP bị block nhanh, tốc độ SOCKS chậm, và nghi ngờ về tính xác thực của các đánh giá tích cực. Về phía mình, 9Proxy đều trả lời công khai từng trường hợp, giải thích chính sách hoàn tiền và đề nghị hỗ trợ thêm qua kênh chính thức.

Chiều ngược lại, các đánh giá tích cực đến từ nhiều nguồn khác nhau: một review trên G2 (5.0, tuy chỉ có một đánh giá), phần thảo luận trên Product Hunt, một bài trên AlternativeTo, các trích dẫn trên Slashdot và SourceForge. Nội dung chung của nhóm này xoay quanh IP sạch, kết nối ổn định, giá hợp lý và hỗ trợ nhanh.

Không có mâu thuẫn kỳ lạ ở đây. Với proxy dân cư, người dùng target dễ sẽ thấy ổn, người dùng target khó hoặc kỳ vọng sai về cách dịch vụ vận hành sẽ thất vọng. Vấn đề đáng chú ý hơn là chính sách hoàn tiền chặt — nội dung đó nằm ở phần dưới.

## Chính sách hoàn tiền: đọc trước khi trả tiền

9Proxy hoàn tiền khi proxy hoàn toàn không hoạt động, và yêu cầu bằng chứng để xác minh. Trường hợp "tôi đổi ý", "tôi tưởng là proxy xoay", "tôi cần danh sách IP:port" không thuộc diện được hoàn. Trong các phản hồi trên Trustpilot, đại diện 9Proxy nhiều lần nhắc rằng chính sách này được hiển thị và phải chấp nhận ở bước thanh toán.

Hệ quả thực dụng rất đơn giản: coi như tiền mua gói nhỏ là tiền test. Chọn gói 100 IP hoặc 5 GB, chạy thử với chính target của bạn trong vài ngày, rồi mới quyết định nâng lên. Cách này rẻ hơn nhiều so với việc mua gói Pro rồi tranh cãi về hoàn tiền.

## Khuyến mãi và thanh toán

Ở thời điểm này, 9Proxy không có mã giảm giá vĩnh viễn công khai nào. Chương trình khuyến mãi chạy theo đợt và thay đổi liên tục:

- Dịp Tết, họ từng chạy giảm 8% cho các gói IP/GB thường với mã dạng theo mùa.
- Tháng 4, họ chạy chương trình hoàn 9% cho đơn GB tiếp theo: sau đơn GB đầu tiên trong tháng, một coupon cá nhân được cấp tự động vào mục My Coupons, tự áp ở bước thanh toán.
- Điều kiện chung của các coupon này: chỉ áp cho GB, không áp cho bundle và gói IP, dùng một lần, không cộng dồn với ưu đãi khác.

Thanh toán hỗ trợ thẻ tín dụng, crypto (USDT, BTC, ETH, LTC, DOGE…), thẻ ngân hàng, Alipay, Apple Pay, Google Pay. Khách thanh toán bằng crypto được cộng thêm 5% IP.

Về chương trình affiliate: hoa hồng trọn đời tối đa 15%, thanh toán crypto tức thì, người được giới thiệu nhận 5% giảm giá. Nếu bạn định vừa dùng vừa giới thiệu, đây là mức không hiếm trên thị trường nhưng điều kiện cụ thể nên xem lại trên trang đối tác.

## Nên chọn gói nào?

- **Mới thử lần đầu, chưa biết target có khó không:** gói 100 IP ($24) hoặc 5 GB ($15). Đây là mức "tiền test", không phải tiền đầu tư.
- **Nuôi vài chục profile ổn định, tải nhẹ:** gói GB. Xoay IP thoải mái, hạn 180 ngày, không lo IP hết hạn sau 24 giờ.
- **Chạy phiên dài, tải nặng, không đoán được lưu lượng:** gói theo IP. Băng thông không giới hạn nên chi phí không nhảy theo dung lượng.
- **Cần cả hai loại việc:** bundle Starter hoặc Growth rẻ hơn mua lẻ hai gói, nhưng nhớ hạn 180 ngày của phần lưu lượng.
- **Team từ 2 người trở lên:** cân nhắc gói Enterprise với team mode, nếu không sẽ phải vật lộn với share code và sub-account.

## Cảnh giác với hàng giả và kênh liên hệ giả

Trong các phản hồi trên Trustpilot, 9Proxy nhiều lần nói rằng người dùng đã liên hệ nhầm tài khoản Telegram không chính thức và bị lừa, hoặc mua qua kênh không phải website của họ. Có cả domain gần giống không liên quan đến dịch vụ này. Nguyên tắc an toàn: chỉ đăng ký và thanh toán trên trang chính thức, và chỉ nhắm liên hệ hỗ trợ theo thông tin niêm yết trên chính trang đó.

## Kết luận: 9Proxy có đáng dùng không?

**Đáng cân nhắc nếu** bạn cần proxy dân cư giá thấp, làm target ở mức dễ đến trung bình, thích mô hình băng thông không giới hạn theo IP, và muốn hạn dùng dài thay vì reset theo tháng.

**Không phù hợp nếu** bạn cần danh sách IP:port, cần streaming, cần SLA doanh nghiệp với cam kết hoàn tiền rộng, hoặc muốn dùng thử miễn phí mà không cần liên hệ hỗ trợ.

Điểm mấu chốt không nằm ở chuyện 9Proxy "tốt" hay "xấu". Nó nằm ở việc bạn có chấp nhận được cách dịch vụ này vận hành hay không: qua app, không hoàn tiền khi đổi ý, IP theo gói có hạn ngắn. Biết rõ ba điều đó trước khi thanh toán thì rủi ro gần như bằng không, vì gói nhỏ nhất chỉ $15.

👉 [Đăng ký tài khoản 9Proxy và kiểm tra giá cùng ưu đãi hiện hành](https://bit.ly/9-Proxy)

## Câu hỏi thường gặp

**9Proxy có phải lừa đảo không?**
Đây là dịch vụ đang hoạt động với khách hàng trả tiền, tài liệu công khai, hỗ trợ phản hồi công khai trên Trustpilot và nhiều bên thứ ba đánh giá. Điểm 2/5 trên Trustpilot đến từ chính sách hoàn tiền chặt và xung đột kỳ vọng, không phải từ việc không cung cấp dịch vụ. Vẫn nên bắt đầu bằng gói nhỏ nhất.

**9Proxy có dùng thử miễn phí không?**
Có nhưng không phải lúc nào cũng có sẵn. Trial dạng số lượng giới hạn, theo đợt, và phải hỏi qua hỗ trợ. Các gói trả tiền nhỏ nhất có giá $15.

**Proxy của 9Proxy dùng được bao lâu?**
Gói theo IP: mỗi IP sống từ vài giờ đến khoảng 24 giờ, băng thông không giới hạn. Gói theo GB: lưu lượng dùng trong 180 ngày với các gói thường, không giới hạn với gói dung lượng lớn.

**Có được chia sẻ tài khoản không?**
Được. 9Proxy hỗ trợ share code và sub-account, kèm hệ thống phân quyền cho các gói team.

**Có cần cài phần mềm không?**
Không bắt buộc. Bạn có thể dùng Proxy2Web ngay trên trình duyệt hoặc qua dashboard. Nhưng nếu cần chạy cho phần mềm không hỗ trợ proxy, bạn phải cài Proxy Program trên Windows.
