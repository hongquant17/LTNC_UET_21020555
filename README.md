# LTNC_UET_21020555

# _Cursor Custodian_

## Thông tin chung
- Bài tập lớn cuối khóa: Cursorphobia (Lập trình nâng cao - INT2215 1)
- Sinh viên: Trần Hồng Quân - 21020555

## Mô tả chi tiết
## _Nhân vật_
- Nhân vật chính của game được sinh ra với một điều đặc biệt là sợ con trỏ chuột, tức khi ta di chuột đến thì nhân vật sẽ di chuyển theo hướng ngược lại. Ngoài ra thì nếu chuột chạm vào nhân vật thì nhân vật đó sẽ "chết", phần nào lí giải cho chứng sợ con trỏ chuột này.

## _Cách chơi_
- Cách chơi hết sức đơn giản, hoàn toàn sử dụng chuột, ấn chuột thì nhân vật sẽ nhảy lên.
- Phần vật lý của game cho phép con trỏ càng gần nhân vật thì tốc độ của nó càng nhanh, cũng như là nó sẽ càng nhảy cao hơn.
- Độ khó của game được tăng dần theo điểm (khoảng cách đã di chuyển), điểm càng cao thì map sẽ chạy nhanh hơn, phản hồi của nhân vật cũng nhanh hơn (`SDL_Delay()`).

## Video Gameplay



## _Hình ảnh sơ bộ_
![image](https://user-images.githubusercontent.com/92194647/168730531-c1e0039d-d757-4d35-8b5f-012441c08241.png)
![image](https://user-images.githubusercontent.com/92194647/168730105-92e8bf37-e26c-4b2b-b4dc-1903e4125451.png)
![image](https://user-images.githubusercontent.com/92194647/168730128-d604c984-ba2f-4c25-b7bc-0912284df9c9.png)
![image](https://user-images.githubusercontent.com/92194647/168730219-2376ace5-b21c-4912-adec-aa02dc31f976.png)
![image](https://user-images.githubusercontent.com/92194647/168730244-5edf602c-b562-47a8-b4a1-307ad4194651.png)

## _Các kĩ thuật sử dụng_

_**SDL2**_
- Kĩ thuật liên quan đến tilemap, render nhiều đối tượng, tại nhiều vị trí,...
- Load hình ảnh, âm thanh, animation đơn giản,...

_**C++**_
- Kiến thức cơ bản: mảng, vector, chuỗi, random,...
- Lập trình hướng đối tượng sơ cấp: class; vận dụng tính đóng gói, kế thừa;...

_**Kĩ thuật khác**_
- Tính toán, căn chỉnh các đối tượng.
- Vận dụng toán học để áp dụng tính vật lý cho game.
- Đóng gói game để có thể dễ dàng install trên thiết bị khác.


## _Cài đặt_
- Tải các file theo đường dãn: https://drive.google.com/drive/u/0/folders/1TIZpdjf2GdVgC7fx6RN6pSo8n-Hl33qA, mở file setup.exe vào làm theo chỉ dẫn.
- Để gỡ bỏ, vào Control Panel -> Uninstall a program, tìm Setup1 và gỡ.



**Trong trường hợp thiếu file \*.dll :**
- Truy cập vào đường link ở trên, tải về file "System32" và "SysWOW64".
- Giải nén file vừa tải về.
- Copy file .dll trong file "System32" dán vào trong thư mục "C:\Windows\System32".
- Copy file .dll trong file "SysWOW64" dán vào trong thư mục "C:\Windows\SysWOW64".
- Thoát ra ngoài và chạy lại chương trình.

## _Nguồn tham khảo_
- Về thư viện SDL2: https://lazyfoo.net/tutorials/SDL/index.php
- Về cách triển khai các kĩ thuật:
    - https://www.youtube.com/watch?v=QQzAHcojEKg&list=PLhfAbcv9cehhkG7ZQK0nfIGJC_C-wSLrx&ab_channel=Let%27sMakeGames
    - https://www.youtube.com/channel/UCl7dSJloxuCa9IBFml7sakw


## _Kết luận_
- Sau khi tương đối hoàn thành BTL kết thúc học phần INT2215 1, em thấy phần quan đáng chú ý là lập trình hướng đối tượng (OOP) để xây dựng từng đối tượng cho game, việc code sẽ gọn gàng và dễ tham khảo, suy luận hơn.
- Có phần comment hai hàm trong code là điều em nhận ra, không phải lỗi font khi render mà do hàm `c_str()` có vấn đề khi gọi ở hàm `main`, em sửa bằng cách thay vì gọi nó, em dùng `to_string` ngay trong hàm `main`, có thể hơi rối nhưng lại hữu ích và vấn đề đã được giải quyết.
- Em nghĩ để phát triển hơn, có thể thêm những đối tượng để cản trở nhân vật, ví dụ như gai, chạm vào sẽ "chết", background có thể thay đổi cho sinh động hơn,... Về phần code thì cần chia lại file, tối giản hàm `main`.


## Lời cuối
  Cảm ơn mọi người đã dành thời gian đọc và đánh giá project!
  
  
  
 ### Mức điểm tự đánh giá: 9~9.5/10
