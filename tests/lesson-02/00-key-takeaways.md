Git commands hữu ích cho Automation Tester:

📌 Thường dùng nhất (Essential):
Command Lý do
git init Khởi tạo repo mới cho test project
git add <file> Thêm test files vào commit
git commit -m "message" Lưu lại thay đổi test
git status Check trạng thái trước khi commit (file màu đỏ vùng working directory, màu xanh đã staged)
git clone <url> Clone test repository từ remote
git push / git pull Đồng bộ code với team
git checkout <branch> Chuyển branch để test feature mới

📌 Có ích cho quản lý code (Recommended):
Command Lý do
git log Xem lịch sử thay đổi test
git diff So sánh thay đổi giữa các version
git branch Tạo branch riêng cho test case mới
git merge Gộp test code sau khi hoàn thành

📌 Ít dùng hơn (Advanced):
Command Lý do  
git stash Lưu tạm thay đổi khi cần switch branch gấp
git tag Đánh dấu version release
git reset <file> Bỏ staging file không muốn commit

📌 Ít liên quan cho Automation Tester:
Command Lý do
git remote add Thường đã có sẵn khi clone
git revert Dùng khi cần undo commit cụ thể
git reset --hard Nguy hiểm, dễ mất data - tránh dùng

📌Git config
Command Lý do
git config --global user.name "Your Name" Thiết lập tên người dùng cho commit toàn hệ thống
git config --global user.email "your.email@example.com" Thiết lập email cho commit toàn hệ thống
git config user.name "Your Name" Thiết lập tên người dùng cho commit trong repo hiện tại

📌Git -commit convention <type>: <subject>
Benefits:
Sử dụng convention giúp team hiểu nhanh mục đích commit
Phân loại commit rõ ràng giúp quản lý code hiệu quả hơn  
 Giúp team nhanh chóng nắm được nội dung thay đổi mà không cần đọc chi tiết code

# Type Dùng khi Ví dụ

feat Thêm feature mới feat: add login functionality
fix Sửa bug fix: resolve login error
docs Thêm/sửa tài liệu docs: update README
refactor Viết lại code, ko đổi chức năng refactor: clean up utils
test Thêm test test: add unit tests for login
chore Công việc lặt vặt (config, build) chore: update dependencies

git commit -m "feat: add login test case"   
git commit -m "fix: update test data for registration"   
git commit -m "docs: update README with test instructions"

# Summary

- Khởi tạo repo mới:
  `git init`. (làm 1 lần duy nhất cho project)

- Tạo repo Github và liên kết mới repo local với remote:
  `git remote add origin <url>` (làm 1 lần duy nhất cho project)

- Thêm file vào staging:
  `git add <file>` hoặc `git add .` để thêm tất cả file đã thay đổi. (làm mỗi khi có thay đổi cần commit)

- Commit file vào Repository area:
  `git commit -m "message"` (làm mỗi khi có thay đổi cần commit)

- Push code lên remote:
  `git push origin main`(làm mỗi khi có thay đổi cần commit)
