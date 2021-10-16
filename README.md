# Mã hóa/Giải mã liệu có quan trọng trong Thế chiến thứ 2?

# Giới thiệu

Trong thế chiến thứ 2, sau khi Adolf Hitler phát xít hóa thành công bộ máy cai trị của nước Đức và bắt đầu xâm lược Ba Lan vào 1/9/1939, hàng loạt cuộc chiến lớn nhỏ đã xảy ra trên khắp thế giới tiêu biểu trong đó có thể kể đến trận ở Dunkirk (1940), trận Trân Châu Cảng (1941), trận Normandie (1944),… Và Napoleon đã từng nói: “Trong chiến tranh 90% là thông tin.” Vậy nên thông tin về các trận đánh, cách bố trí quân đội, thời điểm, địa điểm luôn là những thứ cực kỳ quan trọng của một lực lượng. Vì lý do đó Enigma đã ra đời như một công cụ mã hóa thông tin cho Phát Xít Đức. Ban đầu Enigma được sử dụng trong lĩnh vực thương mại ở những năm 20 của thế kỷ trước nhưng sau đó nó được sử dụng như một công cụ mã hóa/giải mã thông tin của quân Đức.

![image](https://user-images.githubusercontent.com/77542991/137595965-ad2cf6d5-6c10-4d12-ab1a-bf840df7dbe7.png)

# Mã hóa 1 đoạn thông điệp

![image](https://user-images.githubusercontent.com/77542991/137595975-eb2621ab-80c2-4d60-ad87-1e3c72581ca7.png)

Sơ đồ đấu dây của Enigma với các mũi tên và các số từ 1 đến 9 cho biết dòng điện chạy từ điểm nhấn phím đến đèn đang sáng như thế nào. Các Một chìa khóa được mã hóa với D đèn. D sinh ra A, nhưng A không bao giờ sinh ra A; thuộc tính này là do một tính năng được cấp “khóa” duy nhất và có thể bị khai thác bởi các nhà phân tích mật mã trong một số tình huống.

Hãy bắt đầu với thông điệp: 
+ NUMBERPHILE

Thông điệp đã được mã hóa:
+ YTHMYIURFGW

Chú ý:
+ Ở ký tự đầu tiên ký tự N -> Y và ở ký tự thứ 5 E -> Y
+ Ở ký tự thứ 5 E -> Y và ở ký tự cuối E -> W	

Như các bạn thấy thì việc mã hóa Enigma không hề giống theo kiểu mã hóa của Caesar Cypher (luôn cố định độ dịch chuyển ứng với mỗi bộ mã duy nhất). Cách mã hóa này vô cùng đặc biệt và khiến nó trở thành vấn đề lớn nhất của cuộc chiên thông tin này.
Để có được cơ chế mã hóa đặc biệt này là nhờ vào hệ thông rotor xoay của Enigma. Với lần mã hóa đầu tiên A -> G nhưng ở lần thứ 2 có thể A -> C.

![image](https://user-images.githubusercontent.com/77542991/137596020-54e4ee74-5fbc-4da8-996d-6dd222472c08.png)

# Tổng số trường hợp nếu giải “vét cạn” máy Enigma

Đây là lúc áp dụng kiến thức Xác suất thống kê :> mặc dù môn này mình toàn ngủ trong giờ học ;> (Các bạn có thể tham khảo về “Turing machine” để có thể hiểu rõ hơn về độ phức tạp mà mình giải thích bên dưới nhé) 

**Phần đầu tiên là Rotor**

![image](https://user-images.githubusercontent.com/77542991/137596030-81fa4135-9205-473f-bec6-93a2ec501d79.png)

Trong rotor đầu tiên sẽ có 5 “bộ”, đến rotor thứ 2 sẽ có 4 “bộ” và đến rotor  thứ 3 sẽ có 3 “bộ”.
(1)Như vậy phần rotor sẽ có 5*4*3 = 60 trường hợp

**Phần thứ 2 là về “Vị trí bắt đầu” của ký tự:** 

![image](https://user-images.githubusercontent.com/77542991/137596097-8330f736-a5d4-4021-b029-607807421985.png)

Trong bảng chữ cái tiếng anh sẽ có 26 ký tự cho rotor 1 2 và 3
(2)Vậy trong trường hợp của “Vị trí bắt đầu” sẽ có 26*26*26 = 17576 trường hợp

**Phần thứ 3 là về “bảng phích cắm”:**

![image](https://user-images.githubusercontent.com/77542991/137596208-be017f0e-774b-4f82-abb6-d66db9653cdc.png)

Đây chính là yếu tố tạo nên thương hiệu của Enigma sau khi được quân đội Đức đưa vào sử dụng trong quân đội. Như mọi người đã biết trong bảng chữ cái tiếng anh sẽ có 26 ký tự (1 dây cắm sẽ liên kết 2 ký tự) như vậy việc chuyển đổi giữa 26 ký tự sẽ là 26*25*24*…*1 vậy se là (3) 26! trường hợp
Nhưng chúng ta không sử dụng hết 26! trường hợp. Chúng ta chỉ có 10 dây cắm cho “bảng phích cắm” như vậy chỉ có 20 ký tự được sử dụng và 6 ký tự bỏ qua vậy ta sẽ (4) chia 6! trường hợp
Trong 10 cặp ký tự được kết nối bởi dây cắm, chúng ta sẽ không quan tâm đến thứ tự các cặp như cặp AB trước cặp CD hay cặp CD trước cặp AB chúng ta sẽ không quan tâm đến vì vậy chúng ta (5) chia 10! trường hợp
Và trong mỗi cặp ký tự việc A liên kết với B hay B liên kết với A là như nhau nên việc hoán đổi này là không cần thiết vì vậy chúng ta sẽ chia cho 2 trong mỗi cặp và chúng ta có 10 cặp vạy chúng sẽ (6) chia 2^10 trường hợp
Tóm lại là sẽ có bao nhiêu trường hợp khi mã hóa 1 thông tin bằng Enigma?
Đơn giản thôi bạn hãy nhân tất cả các trường hợp (nếu chỉ ghi trường hợp là nhân còn phần ghi chia thì ta sẽ chia cho số đó) (các trường hợp sẽ được đánh số 1 2 3 4 5 6) phía trên lại thì chúng ta sẽ có con số: 

**158,962,555,217,826,360,000 (gần 159 tỷ tỷ trường hợp)**

Và trong mỗi máy sẽ có một tờ giấy bảng mã đi kèm để biết trong ngày đó sử dụng bảng mã nào phù hợp.

![image](https://user-images.githubusercontent.com/77542991/137596218-9516ddcf-085d-419f-ad14-e7f920d1a41b.png)

**Giải mã Enigma**

Sau khi đã hiểu được hoạt động của chiếc máy Enigma chúng ta hãy giải quyết bài toán gửi gói tin của quân Đức và việc bắt và giải mã gói tin của quân Đồng Minh.
Hơn số lượng trường hợp khủng khiếp bên trên, quân Phát Xít còn gửi cả những bức điện giả kèm những bức điện thực nhầm đánh lạc hướng quân Đồng Minh trong việc giải mã. Một ngày quân Đức có thể gửi đến hàng trăm bức điện thông qua radio và quân Đồng Minh bắt những “gói tin” đó bằng việc ngồi nghe radio và ghi lại, họ không dùng Wireshark để bắt gói tin như ngày nay =)))
Có những tài liệu đã cho rằng những bức điện thực thường có những thông điệp như: wetterbericht (dự báo thời tiết); Heil Hitler (Chào Hitler); Heil, mein Fuhrer (Chào, lãnh đạo của tôi); hay Sieg Heil (Chào chiến thắng). Đây chính là những thông điệp để biết đâu là bức điện thực đâu là bức điện giả.
Và việc giải mã bức mật khá phức tạp (các bạn có thể dễ dàng tìm đọc trên wikipedia) nhưng ở đây mình sẽ nêu cách giải đơn giản nhất. Đầu tiên việc vét cạn như trường hợp đã đề cập bên trên là không khả thi, thay vào đó Alan Turing (nhà toán học, logic học và mật mã học người Anh) đã tạo ra máy Bombe để giải mã theo cơ chế loại trừ. Đó là máy Bombe sẽ cho dòng điện chạy qua cặp T-A nhưng dòng điện lại tiếp tục chạy qua cặp T-G như vậy nó sẽ loại tất cả các trường hợp liên quan và qua trường hợp khác để thực hiện. Nhờ vào phương pháp giải mã này thì việc giải mã 1 bức điện của quân Phát Xít chỉ diễn ra trong 20 phút.

![image](https://user-images.githubusercontent.com/77542991/137596159-27c5c43b-6ed9-484c-99e3-76c3282b2a9a.png)

![image](https://user-images.githubusercontent.com/77542991/137596163-a390ca26-5cb0-49ea-9770-427e64c39154.png)
 
# Kết quả:

Nhờ những thông tin giải mã này đã góp phần không nhỏ trong việc chiến thắng các trận chiến, tiêu biểu là trận Stalingrad (1942 – 1943), trận Normandie (1944), trận Ardennes (1944 – 1945). Các nhà sử học ước tính việc giải mã Enigma rút ngắn thời gian của Thế chiến II được khoảng 2 năm, cứu sống 14 triệu mạng người. Đây là bí mật được chính phủ quốc gia sở tại giữ kín suốt 50 năm. Công trình của Turing là cảm hứng cho nhiều thế hệ các nhà khoa học nghiên cứu “Cỗ máy Turing” mà ngày nay chúng ta gọi nó là máy tính (computer).

# Nguồn tham khảo:
Wikipedia

Numberphile

# Tác giả:

Do kiến thức còn hạn chế và việc mình viết bài viết với tinh thần đóng góp và xây dựng kiến thức, mong nhận được sự đóng góp từ mọi người. 

Võ Anh Kiệt – ATTN2020
