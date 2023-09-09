
## Một kỹ sư phần mềm cần phải có một loạt kỹ năng kỹ thuật và không kỹ thuật để thành công trong lĩnh vực này. Dưới đây là một danh sách các kỹ năng quan trọng mà một kỹ sư phần mềm cần phải phát triển:

### Kỹ năng Kỹ thuật:

- Lập trình: Nắm vững ít nhất một ngôn ngữ lập trình và có khả năng nắm bắt nhanh chóng ngôn ngữ mới.

- Kiến thức về Cơ sở dữ liệu: Hiểu về cơ sở dữ liệu, SQL, và kiến thức về quản lý cơ sở dữ liệu.

- Web Development: Kiến thức về phát triển web, bao gồm HTML, CSS, JavaScript, và các framework web như React, Angular, hoặc Vue.js.

- Kiến thức về Hệ thống: Hiểu về hệ điều hành, mạng, và cơ bản về quản lý hệ thống.

- Tích hợp: Kỹ năng tích hợp các dịch vụ và ứng dụng khác nhau bằng cách sử dụng API hoặc giao tiếp giữa các thành phần khác nhau.

- Kiểm tra và Kiểm tra tự động: Hiểu biết về quy trình kiểm tra phần mềm và việc tạo và chạy các kiểm tra tự động.

- Quản lý Phiên bản: Sử dụng hệ thống quản lý phiên bản như Git để theo dõi mã nguồn và quản lý phiên bản.

- Kiến thức về Bảo mật: Hiểu về các lỗ hổng bảo mật phổ biến và biện pháp bảo mật.

### Kỹ năng Mềm:

- Giải quyết vấn đề: Khả năng phân tích và giải quyết các vấn đề phức tạp trong phát triển phần mềm.

- Lập trình Sáng tạo: Có khả năng tạo ra giải pháp sáng tạo và tối ưu trong việc xây dựng ứng dụng.

- Làm việc Nhóm: Có khả năng làm việc hiệu quả trong nhóm, giao tiếp và chia sẻ kiến thức với người khác.

- Tự học và Cập nhật: Ngành công nghệ thông tin luôn thay đổi nhanh chóng, và việc tự học và cập nhật kiến thức là quan trọng.

- Quản lý Thời gian: Có khả năng quản lý thời gian hiệu quả và đáp ứng các thời hạn.

- Làm việc Dưới áp lực: Có khả năng làm việc dưới áp lực và xử lý các tình huống khẩn cấp.

- Sáng tạo và Tư duy Logic: Khả năng tư duy logic và tạo ra giải pháp sáng tạo cho các vấn đề kỹ thuật.

- Ứng dụng Kỹ năng Mềm: Biết cách áp dụng kỹ năng mềm vào công việc hàng ngày để tạo môi trường làm việc tích cực.

### Kỹ năng Liên quan đến Dự án và Quản lý:

- Quản lý Dự án: Hiểu biết về quy trình phát triển phần mềm và quản lý dự án, chẳng hạn như Agile hoặc Scrum.

- Phân tích Yêu cầu: Có khả năng phân tích yêu cầu của khách hàng và biến chúng thành đặc tả kỹ thuật.

- Quản lý Phiên bản và Phát hành: Hiểu về quản lý phiên bản, phát hành ứng dụng, và quy trình triển khai.

- Thiết kế Kiến trúc: Có khả năng thiết kế kiến trúc ứng dụng và xác định cấu trúc mã nguồn.

- Quản lý Dự án Phân tán: Đối với các dự án phức tạp, có khả năng quản lý dự án phân tán hoặc hệ thống phân tán.

```Lưu ý rằng danh sách này có thể không hoàn chỉnh và có thể thay đổi tùy theo ngữ cảnh và loại dự án bạn đang tham gia. Một kỹ sư phần mềm giỏi không chỉ có kiến thức kỹ thuật mà còn có khả năng làm việc trong môi trường thực tế, giải quyết vấn đề, và làm việc với người khác để đạt được mục tiêu dự án.```

## Các nguyên lý trong thiết kế phần mềm

### SOLID
1. Single Responsibility Priciple:
Đây là nguyên lý đầu tiên (chính là chữ S đầu trong SOLID). Nguyên lý này nói rằng không nên có hơn 1 lý do để một lớp (class) thay đổi. Nghĩa là, bạn nên thiết kế class của bạn sao cho mỗi class chỉ phục vụ cho một mục đích.
```
Ví dụ: Một kịch bản như sau, chúng ta cần một tính năng lên lịch hẹn phỏng vấn ứng viên (schedule interview). Công việc chúng ta cần làm là: lưu thông tin buổi phỏng vấn, sau đó gửi mail cho ứng viên về buổi phỏng vấn. Thay vì thiết kế một class ScheduleInterview để làm tất cả các việc trên, bạn tạo một class Interview chỉ để thực hiện công việc lưu thông tin buổi phỏng vấn, và chúng ta có thêm class EmailSending dùng để thực hiện công việc gửi mail cho ứng viên.
```
2. Open/Closed Priciple:
Đây là nguyên lý thứ hai (chính là chữ O trong SOLID). Nguyên lý này nói rằng các thực thể phần mềm như: classs, modules, functions,… thì có thể thoải mái viết code để mở rộng nhưng hạn chế cho việc sửa đổi.
Từ “Closed” ở đây nghĩa là, một module đã được phát triển và tested thì code của nó chỉ được thay đổi để sửa lỗi.
Từ “Open” nghĩa là module có thể dễ dàng và thoải mái được mở rộng từ code hiện tại để phục vụ cho tính năng mới.
```
Ví dụ: một lớp cơ sở PaymentGatewayBase chứa tất cả các thuộc tính và phương thức thanh toán cơ bản. Lớp này có thể được mở rộng bởi các lớp PaymentGateway khác nhau cho các nhà cung cấp cổng thanh toán khác nhau để phục vụ các chức năng của họ. Do đó, nó được mở rộng dễ dàng và thoải mái nhưng hạn chế việc thay đổi.
```

3. Liscov Substitution Priciple:
Nguyên ly này nói rằng các đối tượng của lớp con có thể thay thế được các đối tượng của lớp cha mà vẫn đảm bảo tính đúng đắn của chương trình.
Nói cho dễ hiểu thì chỉ cho class A kế thừa class B khi class A thay thế được class B.
Nguyên lý này là cách để đảm bảo rằng kế thừa được sử dụng đúng cách.

```
Ví dụ:
– Một ví dụ cho trường hợp vi phạm nguyên lý này như sau. Giả sử chúng ta có một lớp Chim với một phương thức là Bay(). Như vậy, chúng ta có thể nói rằng 3 lớp ChimHảiÂu, ChimSáo, ChimCánhCụt đều là Chim nên chúng ta sẽ cho chúng kế thừa lớp Chim. Tuy nhiên, khi gọi Bay() thì ChimHaiAu và ChimSao chạy tốt, còn ChimCanhCut quăng lỗi vì chim cánh cụt thì không bay được.
– Giả sử chúng ta có class Student kế thừa từ class Person. Vậy theo nguyên lý này thì bất cứ nơi nào có thể dùng Person thì cũng có thể dùng Student, bởi vì Student là class con của Person.
– Trong C# chúng ta có thể dùng ForEach với List, ArrayList, LinkedList bởi vì chúng được kế thừa từ interface IEnumerable. Các class List, ArrayList,… được thiết kế đúng LSP nên chúng có thể thay thế cho IEnumerable.
```
4. Interface Segregation Priciple:
Nguyên lý này nói rằng thay vì dùng 1 interface lớn, ta nên tách thành nhiều interface nhỏ với nhiều mục đích cụ thể.
```
Ví dụ: nếu chúng ta có một interface với 20 phương thức (method), vậy thì những class implement sẽ phải implement toàn bộ 20 methods này, kể cả những methods mà nó không bao giờ sử dụng đến. Áp dụng nguyên lý này, chúng ta sẽ chia nhỏ interface lớn này ra thành những interfaces nhỏ hơn, các class chỉ cần implement những interface có chức năng mà chúng cần, không cần implement những methods mà chúng không sử dụng.
```

5. Dependency Inversion Priciple (DIP):
Nguyên lý này nói rằng, các module cấp cao không nên phụ thuộc vào các module cấp thấp. Cả hai nên phụ thuộc vào abstractions (interface).
Abstractions (Interface) không nên phục thuộc vào chi tiết, mà chi tiết nên phụ thuộc vào abstractions (interface). Nghĩa là, Các class nên giao tiếp với nhau thông qua interface, không phải thông qua implementation.
```
Ví dụ: Dependency Injection pattern là một implementation của nguyên lý này.
```

### DRY - Don't Repeat Yourself
Nguyên lý này nói rằng mỗi mẩu kiến thức nhỏ (code) chỉ có thể xảy ra chính xác một lần trong toàn bộ hệ thống. Điều này giúp chúng ta viết mã mở rộng, bảo trì và có thể sử dụng lại được

### KISS - Keep it simple, Stupid
Nguyên lý này nói rằng cố gắng giữ cho từng phần nhỏ của phần mềm đơn giản và nên tránh phức tạp chúng không cần thiết. Điều này giúp chúng ta viết code dễ bảo trì.

### YAGNI – You ain’t gonna need it
Nguyên lý này nói rằng luôn luôn thực hiện những điều khi bạn thực sự cần chúng, không bao giờ thực hiện mọi thứ trước khi bạn cần chúng.

`Create: TopDev.vn`

