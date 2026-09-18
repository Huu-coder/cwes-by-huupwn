# Review CWES

Chào mọi người :>, dạo này thế nào? Mình là huupwn — đó là biệt danh hacker của mình, còn tên thật là Hữu. Mình vẫn đang học cấp 3, và CWES thực ra là chứng chỉ đầu tiên mình từng đạt được.

Năm sau mình đặt mục tiêu tham gia một giải CTF, và mình quyết định cách chuẩn bị tốt nhất là học và thi lấy chứng chỉ **CWES (Web Exploitation Specialist)** của Hack The Box (HTB). Đây là một chứng chỉ khá mới nhưng đang được chú ý ngày càng nhiều, và người ta thường so sánh nó với eWPTX hay BSCP. Dưới đây là toàn bộ trải nghiệm của mình: khóa học, kỳ thi, và bài báo cáo.

## Giới thiệu

Mình đến với an ninh mạng gần như tình cờ — nghịch các module miễn phí của HTB Academy vì tò mò (một phần cũng hẻm có n.yêu :> ), rồi bị cuốn vào cảm giác khá là thích thú khi tìm ra được một exploit hoạt động. Mình không có chứng chỉ nào trước đó, không có kinh nghiệm làm việc chuyên nghiệp, cũng chẳng có mối quan hệ nào trong ngành. Thứ mình có là rất nhiều thời gian rảnh vì còn là học sinh, và một niềm đam mê thật sự với web exploitation (và hacking nói chung).

Mình thích chứng chỉ vì chúng là bằng chứng cụ thể cho kiến thức — một cách để chứng minh với chính mình (và sau này là với người khác) rằng kỹ năng là thật, kể cả khi chưa có một bản CV dày kinh nghiệm làm việc.

Sau một hồi tìm hiểu, mình thu hẹp lựa chọn xuống còn hai: **Certified Web Exploitation Specialist (CWES)** của HTB và **Burp Suite Certified Practitioner (BSCP)** của PortSwigger. Mình đã từng thử vài module miễn phí của HTB Academy cho vui và thích cách họ giảng dạy, nên CWES có vẻ là bước tiếp theo tự nhiên — và cũng là một cột mốc vững chắc trên đường đến giải CTF năm sau.

Để lấy được chứng chỉ, bạn cần:

1. Hoàn thành toàn bộ tài liệu học trong lộ trình **Web Penetration Tester**.
2. Vượt qua kỳ thi với số điểm tối thiểu 80/100.
3. Nộp một bản báo cáo chuyên nghiệp.

## Khóa học chuẩn bị

Bạn phải hoàn thành 100% tài liệu khóa học và vượt qua bài đánh giá kỹ năng ở cuối mỗi module trước khi kỳ thi được mở khóa.

Lộ trình này có khoảng 20 module, độ khó từ dễ đến trung bình. Mọi thứ đều ở dạng văn bản — không có video, không có slide. Mình bị kẹt ở vài bài, nhưng những gợi ý từ cộng đồng (trên mạng và trong Discord của HTB) đã cứu mình nhiều lần.

Không có gì để phàn nàn về nội dung — nó rõ ràng, súc tích, đi thẳng vào vấn đề. Có thể nhận ra vài module được viết bởi những người có kinh nghiệm pentest thực tế; thỉnh thoảng họ chèn vào những câu chuyện thực tế, khá thú vị.

Danh sách đầy đủ các module có trên trang HTB Academy, trong lộ trình Web Penetration Tester.

### Nhược điểm của phần chuẩn bị

Khoảng trống lớn nhất là *thực hành*. Đúng là mỗi module đều kết thúc bằng các bài tập, nhưng bạn đã biết trước chính xác đang tìm loại lỗ hổng nào — điều đó khiến mọi thứ dễ hơn nhiều so với thực tế.

Kỳ thi thật thì đưa cho bạn một ứng dụng và chẳng có gì khác cả; việc tìm ra cần kiểm tra cái gì là do bạn tự lo. Một phòng lab lớn tích hợp nhiều ứng dụng — thứ thật sự mô phỏng điều kiện thi — sẽ giúp ích rất nhiều. Một danh sách máy thực hành bổ sung riêng biệt cũng không thừa. Nhìn chung, mình cảm thấy khóa học chưa chuẩn bị đủ cho bạn về mặt thực hành.

## Kỳ thi

Một điểm cộng lớn: không cần đặt lịch. Bạn chỉ cần đăng nhập và bấm bắt đầu bất cứ khi nào sẵn sàng. Bạn có **7 ngày tổng cộng**, bao gồm cả quyền truy cập lab lẫn viết báo cáo — không có thêm thời gian riêng cho báo cáo, vì vậy hãy lên kế hoạch cho phù hợp.

Bạn sẽ đối mặt với nhiều ứng dụng, mỗi ứng dụng yêu cầu một user flag và một root flag. Thường thì điều đó có nghĩa là khai thác một lỗ hổng, hoặc kết hợp hai lỗ hổng. Thường sẽ có thêm một mẹo nào đó bạn phải tự nghĩ ra, dù một vài flag khá đơn giản — tương đương với các bài đánh giá kỹ năng.

Thành thật mà nói, một số phần của kỳ thi *khó hơn nhiều* so với bất cứ điều gì trong các module — vài thử thách đẩy mình vượt xa những gì các bài đánh giá kỹ năng đã chuẩn bị. Các flag khác thì gần với độ khó của module hơn, nhưng mình không dám nói kỳ thi "ngang tầm" xuyên suốt; hãy chuẩn bị tinh thần cho những đợt tăng độ khó thực sự. Mình lấy được hết các flag vào ngày thứ 4 và dành thời gian còn lại để viết báo cáo.

### Nhược điểm của kỳ thi

Bảy ngày là một khoảng thời gian dài. Mình đã sắp xếp thi vào kỳ nghỉ hè để khỏi phải xin nghỉ làm — không hẳn là cách nghỉ ngơi thoải mái, và khá mệt mỏi về tinh thần khi mọi người xung quanh đang thư giãn. Mình cho rằng khung thời gian (và có thể cả số lượng nhiệm vụ) nên được rút ngắn lại.

Cũng cần nói thẳng: nếu không có kinh nghiệm với các máy ngoài các module chính thức, kỳ thi thực sự khó. Chỉ riêng lý thuyết của khóa học là chưa đủ.

### Ưu điểm của kỳ thi

Môi trường thi rất ổn định — không lag, không crash, điều này rất quan trọng trong suốt cả tuần thi. Mình cũng thật sự thích thiết kế của một vài thử thách.

## Khóa học có đủ để vượt qua kỳ thi không?

Trả lời ngắn gọn: chỉ một phần. Các kỹ thuật khai thác được dạy khá tốt, nhưng như đã nói, kỳ thi dựa vào những "mẹo" không được đề cập rõ ràng trong các module. Hãy chuẩn bị tinh thần tự mày mò một số phần — mà thành thật thì, đó cũng là luyện tập tốt cho môi trường CTF, nơi bạn hiếm khi được cầm tay chỉ việc.

## Viết báo cáo

Chỉ lấy được flag thôi là chưa đủ — một bản báo cáo chuyên nghiệp là bắt buộc, và có người trượt vì nộp báo cáo yếu. Đây không phải là một bài walkthrough; nó cần có phân tích đầy đủ cho từng lỗ hổng: mức độ ảnh hưởng, điểm CWE/CVSS, biện pháp khắc phục, và các bước tái hiện chi tiết. HTB cung cấp một mẫu (template) nêu rõ chính xác những gì họ mong đợi.

Mình dùng **Sysreptor** để viết báo cáo, và nó giúp quá trình dễ dàng hơn nhiều. Nó tự động định dạng mọi thứ theo phong cách của HTB, tạo mục lục, và cung cấp sẵn cấu trúc cho từng phát hiện. Tìm được một lỗi SQL injection? Bấm "add new finding," chọn SQLi từ danh sách, và nó sẽ tạo ra một chương với phần mô tả và biện pháp khắc phục đã điền sẵn — bạn chỉ cần bổ sung các bước cụ thể của mình vào.

**Mẹo:** phiên bản cloud của Sysreptor có phí, nhưng bạn có thể tự host miễn phí trên VM của riêng mình và truy cập qua giao diện web từ Kali hoặc máy chủ của bạn. Mình khuyên bạn nên thiết lập cái này *trước khi* kỳ thi bắt đầu. Nó không chịu chạy trên máy Kali của mình, nên mình phải dựng Ubuntu thay thế — mất khoảng 90 phút mà mình không muốn mất giữa kỳ thi.

Viết báo cáo mất của mình 5–6 tiếng. Mình để qua đêm rồi xem lại mọi thứ với một cái đầu tỉnh táo vào sáng hôm sau. SLA chấm điểm của HTB là tối đa 20 ngày làm việc.

**Cập nhật:** Mình nộp báo cáo và chỉ hơn hai ngày để xét duyệt và có kết quả.

## Chi phí

Tính đến đầu năm 2026, có hai cách chính để thanh toán:

- **Gói Silver Annual Subscription — 490 USD.** Toàn quyền truy cập lộ trình Web Penetration Tester cộng một voucher thi. Lựa chọn đơn giản nhất, thiết lập một lần rồi khỏi lo.
- **Cubes (đơn vị tiền tệ nội bộ của HTB).** Toàn bộ lộ trình Web Penetration Tester tốn 1.410 cubes (~150 USD với giá ~100 USD cho mỗi 1.000 cubes), cộng thêm voucher thi riêng 210 USD — tổng cộng khoảng **360 USD**. Tiết kiệm hơn nếu CWES là mục tiêu duy nhất của bạn trên nền tảng này.

Hãy kiểm tra trang thanh toán của HTB để biết giá hiện tại.

## Lời khuyên của mình

1. **Ghi chú chi tiết.** Không thể bỏ qua. Các module thường giấu những chi tiết nhỏ hoặc đoạn code trở thành gợi ý trực tiếp trong kỳ thi — hãy ghi lại mọi thứ để có thể tìm kiếm sau này.
2. **Làm lại các bài đánh giá kỹ năng trước kỳ thi.** Quay lại giải lại các bài tập cuối module, và lướt qua tài liệu học một lần nữa để bạn có thể tra cứu nhanh khi áp lực thời gian. Bạn *sẽ* phải lật lại nội dung khóa học trong kỳ thi để tìm ý tưởng.
3. **Tìm thêm cơ hội thực hành bên ngoài.** Chỉ riêng các module là chưa đủ — thời gian dành cho các máy trên nền tảng chính của HTB là vô giá. Bản thân mình chưa hoàn thành lộ trình Bug Bounty Hunter, nhưng nó có vẻ là một nơi thực hành khai thác thủ công rất tốt, và khai thác thủ công chính là kỹ năng mà một giải CTF sẽ kiểm tra.
4. **Chọn lọc kỹ tài nguyên bổ sung.** Mình đã học qua một phần lộ trình CPTS của IppSec, và dù nó khá hay, nó không thực sự liên quan lắm đến đây. Hãy tìm những máy đòi hỏi khai thác web thủ công, chứ không phải các exploit công khai cho phần mềm lỗi thời — đó mới chính là bộ kỹ năng mà cả CWES lẫn giải CTF năm sau đều đánh giá cao.

*Date: 19-09-26*

***Lưu ý về việc sử dụng AI:*** *Mình tự viết bài này. Mình đã dùng Claude (Anthropic) để chỉnh sửa đáng kể về ngữ pháp, cách dùng từ và cấu trúc câu; nội dung kỹ thuật và mọi nhận định đều là của mình.*

***Lưu ý:*** *Nếu bạn muốn xem một phần bài viết CWES của mình, hãy liên hệ mình [tại đây](https://www.facebook.com/profile.php?id=61553341873402)*
