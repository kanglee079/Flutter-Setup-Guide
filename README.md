# Flutter Installation Guide for Windows and macOS

Flutter is a powerful framework for building cross-platform applications from a single codebase. This guide will walk you through the steps to set up Flutter on **Windows** and **macOS**.

---

## System Requirements

### Windows
- **Operating System**: Windows 10 or later (64-bit).
- **Processor**: Intel or AMD processor.
- **RAM**: Minimum 8GB.
- **Free Disk Space**: At least 2.5GB (not including space for IDEs like Android Studio).
- **Additional Tools**: PowerShell 5.0 or later and Git for Windows.

### macOS
- **Operating System**: macOS Catalina (10.15) or later.
- **Processor**: Apple Silicon (M1/M2) or Intel.
- **RAM**: Minimum 8GB.
- **Free Disk Space**: At least 2.8GB.

---

## Installing Flutter on Windows

### 1. Download Flutter SDK
1. Visit [flutter.dev](https://flutter.dev/docs/get-started/install) and download the **Flutter SDK** for Windows.
2. The downloaded file will be a `.zip`. Extract it to a folder in the main drive, e.g., `C:\src\flutter`.

![Flutter for Windows](https://flutter.dev/assets/images/shared/brand/flutter/logo/flutter-lockup-bg.jpg)

> **Note**: Do not install Flutter in a directory that requires admin permissions, such as `C:\Program Files`.

---

### 2. Configure Environment Variables
1. Open **Control Panel** → **System** → **Advanced system settings** → **Environment Variables**.
2. In the **System Variables** section, locate **Path** and click **Edit**.
3. Add the path to the `bin` directory of the Flutter SDK, e.g., `C:\src\flutter\bin`.

![Environment Variable Path](https://i.stack.imgur.com/E26eH.png)

> **Tip**: Verify the configuration by running `flutter doctor` in Command Prompt.

---

### 3. Install Android Studio
1. Download and install [Android Studio](https://developer.android.com/studio).
2. Open **Android Studio**, navigate to **Settings** → **Appearance & Behavior** → **System Settings** → **Android SDK**.
3. Install the following components:
   - **SDK Platform** (latest version).
   - **Android SDK Build-Tools**.
   - **Android Emulator**.

![Android Studio SDK](https://developer.android.com/studio/images/hero-image_2x.png)

---

## Installing Flutter on macOS

### 1. Download Flutter SDK
1. Visit [flutter.dev](https://flutter.dev/docs/get-started/install) and download the **Flutter SDK** for macOS.
2. Extract the downloaded `.zip` file to a folder, e.g., `~/Development/flutter`.

---

### 2. Configure Environment Variables
1. Open **Terminal** and edit the `~/.zshrc` file (or `~/.bashrc` if using bash):

```bash
export PATH="$PATH:~/Development/flutter/bin"
```

2. Apply the changes by running:

```bash
source ~/.zshrc
```

> **Check**: Run `flutter doctor` to verify the installation.

---

### 3. Install Xcode
1. Download and install **Xcode** from the App Store.
2. Open Xcode, go to **Preferences** → **Locations**, and select the Command Line Tools version.
3. Install required components:

```bash
sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
sudo xcodebuild -runFirstLaunch
```

![Xcode](https://developer.apple.com/assets/elements/icons/xcode/xcode-128x128_2x.png)

---

### 4. Install Android Studio (Optional)
1. Download [Android Studio](https://developer.android.com/studio) and install it.
2. Configure it similarly to the Windows setup.

---

## Verify Flutter Installation
Run the following command in Terminal or Command Prompt:

```bash
flutter doctor
```

This command will check your environment and display any missing dependencies.

![Flutter Doctor](https://flutter.dev/assets/images/docs/tools/dash-diagnostics-57c63dd1cb1281b546c0550ec3262fb4dc72c7aab09c2a2c1996ecfb2c2f9409.png)

---

## Conclusion
You have successfully installed Flutter on Windows or macOS. Start a sample project by running:

```bash
flutter create my_first_app
cd my_first_app
flutter run
```

Good luck on your Flutter development journey!


Vietnamese
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
