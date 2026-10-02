Câu 1 (Value Types vs Reference Types):

Value Types (struct, int, bool, float...) lưu trữ trực tiếp giá trị trên Stack (hoặc nằm trong một object khác nếu là kiểu thành phần). Khi gán hoặc truyền tham số, giá trị sẽ được sao chép hoàn toàn.

Reference Types (class, string, array...) lưu trữ tham chiếu (địa chỉ ô nhớ) trên Stack, trong khi vùng nhớ chứa dữ liệu thực sự nằm trên Heap. Khi gán, chỉ có địa chỉ tham chiếu được copy, cả hai biến cùng trỏ tới một vùng dữ liệu trên Heap.

Câu 2 (Init-only Properties):

Khác biệt: Từ khóa init thay thế cho set, cho phép gán giá trị cho thuộc tính chỉ trong quá trình khởi tạo đối tượng (ví dụ qua object initializer hoặc constructor). Sau khi khởi tạo xong, thuộc tính trở thành read-only, không thể thay đổi giá trị từ bên ngoài nữa, giúp đảm bảo tính bất biến (immutability).

Ứng dụng thực tế: Dùng cho các đối tượng DTO (Data Transfer Object) hoặc các cấu hình không được phép thay đổi trạng thái sau khi đã khởi tạo.

Câu 3 (virtual và override trong Đa hình):

virtual được đặt ở phương thức của lớp cha nhằm cho phép lớp con có thể ghi đè (override) hành vi đó.

override được đặt ở phương thức của lớp con để viết lại/triển khai lại logic riêng cho phù hợp với lớp con đó, duy trì tính đa hình khi gọi thông qua tham chiếu lớp cha.

Câu 4 (Thành phần static):

Thành phần static thuộc về lớp (class) chứ không thuộc về bất kỳ thể hiện (object instance) cụ thể nào. Do đó, nó được nạp sẵn vào bộ nhớ chung khi chương trình chạy và không thể truy cập thông qua từ khóa new từ một đối tượng cụ thể.
