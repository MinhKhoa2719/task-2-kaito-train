# task-2-kaito-train

# Khái niệm : GitHub là một dịch vụ lưu trữ trên web cho các dự án có sử dụng hệ thống kiểm soát Git revision.

-GitHub cung cấp chức năng social networking như feeds, followerd và network graph để các Developer học hỏi kinh nghiệm làm việc thông qua lịch sử commit. Nếu commit dùng để mô tả chức năng của đoạn code. thì commit messenge trên Git dùng để mô tả hành động mà DEV vừa thực hiện trên code.

-Một tài khoản GitHub với nhiều repositories và tham gia vào những project đa dạng khác nhau đem đến cho bạn nhiều lợi ích đáng kể, có thể thay đổi sự nghiệp của bạn 

# 1- GitHub có 3 lợi ích chính 

Nhìn vào lịch sử hoạt động của một tài khoản GItHub cho bạn biết nhiều điều:

Thời gian bắt đầu,các project từng tham gia, một developer nhiều kinh nghiệm sẽ có nhiều Git Hub repositoties đa dạng và tham gia vào nhiều technology patterns thường chú ý đến những đoạn code chất lượng với doccumentation tốt. đặc biệt ,tôi quan tâm nhiều về việc Developer tương tác với các contributor khác trên GitHub. điều này cho thấy họ muốn cải thiện code của mình và muốn cống hiến cho các open source khác

Developer đều nên đầu tư một tài khỏan Github chất lượng và ghi vào CV của mình. vì nó tăng cơ hội làm việc cho Developer

# 2- Github giúp cải thiện coding skill

GitHub tạo một môi trường khuyến khích cải thiện coding skill bằng cách theo dõi và so sánh những thay đổi thường xuyên, trong cộng đồng hàng trăm nghìn contributor của GIthub, khi tương tác với họ tôi dễ dàng học được hàng tấn kinh nghiệm để cải thiện code của mình trong vòng 30p thay vì phải bỏ ra nhiều giờ tìm kiếm thông tin trên internet



# 3- Github giúp học hỏi nhiều kỹ năng mới 

Github có 1 kho tài liệu tuyệt vời giúp tôi học hỏi nhiều kỹ năng mới.Phần helps và guides có nhiều bào viết hầu hết như tất các chủ đề liên quan đến Git mọi người có thể nghĩ đến để lên trình code. đọc source trên Git(repositories), và phần explore là phần dẫn đến những open source nổi tiếng

Bạn có biết tạo ra SSh key? Github

Bạn tự hỏi về quy trình làm việc của một GItHub tốt?





# *Kết nối với GitHub bằng SSH

Về SSH

Sử dụng giao thức SSH,bạn có thể kết nối và xác thực với các máy chủ và dịch vụ từ xa. với khóa SSh bạn có thể kết nối với GitHub mà không cần cung cấp tên người dùng hoặc mật khẩu của mình mỗi lần truy cập

# Kiểm tra các khóa ssh hiện có

Trước khi tạo khóa ssh bạn có thể kiểm tra xem mình có bất kỳ khóa ssh nào hiện có hay không

# Tạo khóa SSH mới và thêm các khóa đó vào SSH-agent

Sau khi bạn đã kiểm tra các khóa SSH hiện có bạn có thể tạo một khóa ssh mới để sử dụng cho việc xác thực,sau đó thêm nó vào ssh-agent

# Thêm khóa ssh mới vào tài khoản GitHub của bạn

Để định cấu hình tài khoản GitHub của bạn để sử dụng khóa ssh mới (hoặc hiện có;)bạn cũng cần thêm nó vào tài khoản GitHub của mình

# kiểm tra kết nối ssh của bạn

Sau khi thiết lập khóa ssh của bạn và thêm vào tài khoản GitHub bạn có thể kiểm tra kết nối của mình

# Làm việc với mật khẩu của khóa ssh

Bạn có thể bảo mật khóa ssh của mình và định cấu hình tác nhân xác thực để bạn không phải nhập lại cụm mật khẩu mỗi khi sử dụng khóa ssh



.




# DeMO sử dụng khóa SSH ( SSH key )

SSh keys là một phương thức xác nhận với máy chủ thông qua truy cập ssh bằng việc đối chiếu giữa một cặp keys bao gồm một khóa riêng tư(private key) và khóa công khai(public key) tương ứng,


SSh key sử dụng giao thức xác thực hỏi và trả lời trong đó một bên tronhf bày một câu hỏi và một bên khác phải cung cấp một câu trả lời hợp lệ để được chứng thực

Thông thường một người dùng đăng nhập VPS thông qua username root và password của user đó ,người dùng có thể mất quyền truy cập VPS nếu bị quên mất hoặc tiết lộ mật khẩu hay bị dò tìm mật khẩu qua Brute Force Attack, do đó việc sử dụng ssh keys sẽ đảm bảo bảo mật hơn rất nhiều so với phương pháp truyền thống.


# MỘT CÁCH ĐƠN GIẢN TA CÓ THỂ HIỂU SO SÁNH PRIVATE KEY NHƯ LÀ CHÌA KHÓA CÒN PUBLIC KEY LÀ Ổ KHÓA



Khi tạo ra một ssh key gồm có 3 thành phần:

+Public Key (dạng file và string) – Bạn sẽ copy ký tự key này sẽ bỏ vào file ~/.ssh/authorized_keys trên server của bạn.

+Private Key (dạng file và string) – Bạn sẽ lưu file này vào máy tính, sau đó sẽ thiết lập cho PuTTY, WinSCP, MobaXterm,..để có thể login.

+Keypharse (dạng string, cần ghi nhớ) – Mật khẩu để mở private key, khi đăng nhập vào server nó sẽ hỏi cái này.


.


Hiện tại, hầu hết các các phần mềm SSH đều có công cụ tạo Keys. Để đảm bảo bảo mật, bạn cần tạo cặp Keys mã hóa bởi thuật toán RSA2 với độ dài ít nhất 2048bit.

Quá trình tạo bạn cũng có thể nhập mật khẩu sử dụng Passphrase cũng như note về mục đích sử dụng Key Comment.


PuTTy với ứng dụng PuTTygen. Ngoài ra, bạn có thể dùng (PuTTygen Portable).


*ZOC với menu File/Create SSh Key Files.


*Bitvise SSH với Client key manager/Generate New.




# Tạo SSH


# Tạo SSH Keys bằng PuTTyGen: 


Lựa chọn SSH-2 RSA và 2048 như hình rồi ấn Generate đồng thời rê chuột xung quanh khung trắng để khởi tạo các chuỗi ngẫu nhiên. Nếu bạn đã có Private 
Key thì chỉ cần nhấn Load để tạo Public Key tương ứng(dùng khi convert Private Key dạng OpenSSH sang).



Sau khi tạo xong, màn hình hiển thị Public Key. Bạn có thể thiết lập Passphrase và Key Comment. Bạn nhấn Save private key để lưu lại.





![hinh1](https://user-images.githubusercontent.com/54676091/91632319-351eb980-ea0a-11ea-923e-d5a87a783f46.png)



# Tạo SSH Keys bằng ZOC Client:



![hình2](https://user-images.githubusercontent.com/54676091/91632325-38b24080-ea0a-11ea-8b16-ea288352fbc8.png)



# Tạo SSH Keys bằng Bitvise SSH Client:



![hinh3](https://user-images.githubusercontent.com/54676091/91632328-39e36d80-ea0a-11ea-84b7-e8a2b59ff7a6.png)







# Thêm Public Key vào VPS

Đối với server Linux, bạn cần lưu thông tin Public Key tại ~/.ssh/authorized_keys để xác thực đăng nhập sử dụng SSH Keys.







*mkdir ~/.ssh/

*nano ~/.ssh/authorized_keys



.





Copy toàn bộ nội dung Public key (dạng ssh-rsa AAAA...) chèn thêm phía cuối file. Nhấn Ctrl+O để lưu lại nội dung và Ctrl+X để thoát khỏi editor.



Bật chế độ đăng nhập bằng SSH Keys: kích hoạt (uncomment) các tham số sau trong SSH Config tại /etc/ssh/sshd_config



*PubkeyAuthentication yes

*AuthorizedKeysFile .ssh/authorized_keys


# Sau đó, khởi động lại SSH Service



*service sshd restart



# 3. Sử dụng SSH Keys

Để sử dụng SSH Keys truy cập VPS, các bạn chỉ cần login thông qua các phần mềm SSH như PuTTy, Bitvise, ZOC và lựa chọn file Private Key đã tạo khi trước.



# Lưu ý: Thường xuyên đăng nhập bằng SSH Client nào thì dùng chính phần mềm ý tạo SSH Keys.


# Đối với PuTTy

Nếu sử dụng OpenSSH Keys (keys tạo bởi lệnh trong Linux/MacOS,…), bạn cần dùng PuTTygen để convert Private Key sang chuẩn đăng nhập với PuTTy.




![hình 4](https://user-images.githubusercontent.com/54676091/91632331-3bad3100-ea0a-11ea-817a-ac1cd057b3f3.png)





# Đối với ZOC




![hinh 5](https://user-images.githubusercontent.com/54676091/91632332-3d76f480-ea0a-11ea-9f28-e68f41147b4d.png)





Nếu passphrase được thiết lập, phần mềm sẽ yêu cầu bạn nhập trong quá trình đăng nhập. Nếu không, bạn sẽ được truy cập thẳng vào server.



# 4. Cấu hình sử dụng SSH Keys

Để gia tăng bảo mật, bạn nên thay đổi port truy cập SSH mặc định (22) và theo dõi truy cập SSH với Fail2ban.



Bên cạnh đó, cũng nên vô hiệu hóa đăng nhập sử dụng mật khẩu bằng cách chỉnh sửa tham số sau trong /etc/ssh/sshd_config:



*PasswordAuthentication no


Sau đó, khởi động lại SSH Service



*service sshd restart




Qua bài viết này, hi vọng các bạn đã hiểu được SSH Keys là gì, cách thức sử dụng cũng như tầm quan trọng của nó. Các bạn cũng nên bỏ hẳn cách thức đăng nhập bằng mật khẩu truyền thống, tránh bị lộ/dò mật khẩu.






# Sử dụng VScode để làm việc với GitHub





