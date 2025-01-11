# Flutter-Setup-Guide

# Hướng Dẫn Cài Đặt Flutter trên Windows và macOS

Flutter là một framework mạnh mẽ để xây dựng ứng dụng đa nền tảng từ một codebase duy nhất. Bài viết này sẽ hướng dẫn bạn từng bước cài đặt Flutter trên **Windows** và **macOS**.

---

## Yêu Cầu Hệ Thống

### Windows
- **Hệ điều hành**: Windows 10 trở lên (64-bit).
- **Bộ xử lý**: Bộ xử lý Intel hoặc AMD hỗ trợ.
- **RAM**: Tối thiểu 8GB.
- **Dung lượng đĩa trống**: Ít nhất 2.5GB (không bao gồm dung lượng dành cho IDE như Android Studio).
- **Công cụ bổ sung**: PowerShell 5.0 trở lên và Git for Windows.

### macOS
- **Hệ điều hành**: macOS Catalina (10.15) trở lên.
- **Bộ xử lý**: Chip Apple Silicon (M1/M2) hoặc Intel.
- **RAM**: Tối thiểu 8GB.
- **Dung lượng đĩa trống**: Ít nhất 2.8GB.

---

## Cài Đặt Flutter trên Windows

### 1. Tải Flutter SDK
1. Truy cập [flutter.dev](https://flutter.dev/docs/get-started/install) và tải **Flutter SDK** dành cho Windows.
2. Tệp tải về sẽ có dạng `.zip`. Hãy giải nén tệp này vào thư mục ổ đĩa chính, ví dụ: `C:\src\flutter`.

![Flutter for Windows](https://flutter.dev/assets/images/shared/brand/flutter/logo/flutter-lockup-bg.jpg)

> **Lưu ý**: Không đặt Flutter trong thư mục yêu cầu quyền quản trị, ví dụ: `C:\Program Files`.

---

### 2. Cấu Hình Biến Môi Trường
1. Mở **Control Panel** → **System** → **Advanced system settings** → **Environment Variables**.
2. Trong mục **System Variables**, tìm **Path** và nhấp **Edit**.
3. Thêm đường dẫn đến thư mục `bin` của Flutter SDK, ví dụ: `C:\src\flutter\bin`.

![Environment Variable Path](https://i.stack.imgur.com/E26eH.png)

> **Mẹo**: Kiểm tra cấu hình bằng cách chạy `flutter doctor` trong Command Prompt.

---

### 3. Cài Đặt Android Studio
1. Tải và cài đặt [Android Studio](https://developer.android.com/studio).
2. Mở **Android Studio**, đi tới **Settings** → **Appearance & Behavior** → **System Settings** → **Android SDK**.
3. Tải xuống các thành phần sau:
   - **SDK Platform** (phiên bản mới nhất).
   - **Android SDK Build-Tools**.
   - **Android Emulator**.

![Android Studio SDK](https://developer.android.com/studio/images/hero-image_2x.png)

---

## Cài Đặt Flutter trên macOS

### 1. Tải Flutter SDK
1. Truy cập [flutter.dev](https://flutter.dev/docs/get-started/install) và tải **Flutter SDK** dành cho macOS.
2. Mở tệp `.zip` vừa tải về và giải nén vào thư mục, ví dụ: `~/Development/flutter`.

---

### 2. Cấu Hình Biến Môi Trường
1. Mở **Terminal** và chỉnh sửa tệp `~/.zshrc` (hoặc `~/.bashrc` nếu dùng bash):

```bash
export PATH="$PATH:~/Development/flutter/bin"
```

2. Chạy lệnh sau để cập nhật:

```bash
source ~/.zshrc
```

> **Kiểm tra**: Chạy `flutter doctor` để xác nhận cài đặt.

---

### 3. Cài Đặt Xcode
1. Tải và cài đặt **Xcode** từ App Store.
2. Mở Xcode, vào **Preferences** → **Locations** và chọn phiên bản Command Line Tools.
3. Cài đặt các thành phần cần thiết:

```bash
sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
sudo xcodebuild -runFirstLaunch
```

![Xcode](https://developer.apple.com/assets/elements/icons/xcode/xcode-128x128_2x.png)

---

### 4. Cài Đặt Android Studio (Tùy Chọn)
1. Tải [Android Studio](https://developer.android.com/studio) và cài đặt.
2. Cấu hình tương tự như trên Windows.

---

## Kiểm Tra Cài Đặt Flutter
Chạy lệnh sau trên Terminal hoặc Command Prompt:

```bash
flutter doctor
```

Lệnh này sẽ kiểm tra toàn bộ môi trường của bạn và hiển thị các bước còn thiếu.

![Flutter Doctor](https://flutter.dev/assets/images/docs/tools/dash-diagnostics-57c63dd1cb1281b546c0550ec3262fb4dc72c7aab09c2a2c1996ecfb2c2f9409.png)

---

## Kết Luận
Bạn đã hoàn thành cài đặt Flutter trên Windows hoặc macOS. Hãy bắt đầu với một dự án mẫu bằng cách chạy:

```bash
flutter create my_first_app
cd my_first_app
flutter run
```

Chúc bạn thành công trên hành trình phát triển ứng dụng Flutter!
