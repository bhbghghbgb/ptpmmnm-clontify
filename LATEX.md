# 📘 LaTeX & Visual Studio Code Setup Guide

## What is LaTeX?

LaTeX is a high-quality typesetting system designed for producing scientific and technical documents. It excels at handling complex mathematical formulas, bibliographies, and structured documents.([GitHub][1])

### Why Use LaTeX?

- Professional-quality typesetting.
- Ideal for academic papers, theses, and technical documentation.
- Supports extensive mathematical notation.
- Cross-platform and open-source.([GitHub][1])

## Introducing Visual Studio Code & LaTeX Workshop

[Visual Studio Code (VS Code)](https://code.visualstudio.com/) is a free, open-source code editor developed by Microsoft. With the [LaTeX Workshop extension](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), VS Code becomes a powerful LaTeX editor.([Visual Studio Marketplace][2])

### Key Features of LaTeX Workshop

- Automatic PDF compilation on save.
- Integrated PDF viewer with forward and reverse SyncTeX.
- IntelliSense for LaTeX commands, citations, and references.
- Error and warning highlights from LaTeX logs.
- Snippets and shortcuts for common LaTeX commands.([Paul Wintz][3], [GitHub][4], [Visual Studio Marketplace][2])

## Comparing LaTeX Editors

| Feature                 | LaTeX Workshop (VS Code) | Overleaf         | TeXstudio |
| ----------------------- | ------------------------ | ---------------- | --------- |
| Offline Editing         | ✅                       | ❌ (Online only) | ✅        |
| Real-time Collaboration | ❌                       | ✅               | ❌        |
| Integrated PDF Viewer   | ✅                       | ✅               | ✅        |
| Customizability         | ✅                       | ❌               | ✅        |
| Plugin Support          | ✅                       | ❌               | Limited   |

## Installation Guide

### 1. Install TeX Live

**Windows:**

1. Download the TeX Live installer from the [official website](https://www.tug.org/texlive/).
2. Run the installer and follow the prompts.
3. After installation, ensure the TeX Live `bin` directory is added to your system's PATH environment variable.

**macOS:**

1. Install MacTeX from [https://tug.org/mactex/](https://tug.org/mactex/).
2. Follow the installation instructions provided.

**Linux (Debian/Ubuntu):**

```bash
sudo apt update
sudo apt install texlive-full
```

### 2. Install Visual Studio Code

Download and install VS Code from the [official website](https://code.visualstudio.com/).

### 3. Install LaTeX Workshop Extension

1. Open VS Code.
2. Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or pressing `Ctrl+Shift+X`.
3. Search for "LaTeX Workshop" and click "Install".([Programmer Sought][5], [boom1999.github.io][6])

### 4. Install ChkTeX (Optional but Recommended)

**Windows:**

1. Open Command Prompt as Administrator.
2. Run:

```bash
tlmgr install chktex
```

**macOS/Linux:**

```bash
sudo tlmgr install chktex
```

### 5. Configure LaTeX Workshop (Optional)

You can customize LaTeX Workshop settings by editing the `settings.json` file:

1. In VS Code, press `Ctrl+,` to open Settings.
2. Click on the `{}` icon in the top right to open `settings.json`.
3. Add or modify settings as needed. For example:([boom1999.github.io][6])

```json
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.view.pdf.viewer": "tab",
"latex-workshop.latex.outDir": "./out"
```

---

# 📘 Hướng Dẫn Cài Đặt LaTeX & Visual Studio Code

## LaTeX là gì?

LaTeX là một hệ thống sắp chữ chất lượng cao, được thiết kế để tạo ra các tài liệu khoa học và kỹ thuật. Nó xuất sắc trong việc xử lý các công thức toán học phức tạp, thư mục tài liệu và cấu trúc tài liệu.

### Tại sao sử dụng LaTeX?

- Sắp chữ chuyên nghiệp.
- Lý tưởng cho các bài báo học thuật, luận văn và tài liệu kỹ thuật.
- Hỗ trợ ký hiệu toán học phong phú.
- Đa nền tảng và mã nguồn mở.

## Giới thiệu Visual Studio Code & LaTeX Workshop

[Visual Studio Code (VS Code)](https://code.visualstudio.com/) là trình soạn thảo mã nguồn miễn phí và mã nguồn mở do Microsoft phát triển. Với tiện ích mở rộng [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), VS Code trở thành một trình soạn thảo LaTeX mạnh mẽ.([Visual Studio Marketplace][2])

### Tính năng chính của LaTeX Workshop

- Tự động biên dịch PDF khi lưu.
- Trình xem PDF tích hợp với SyncTeX hai chiều.
- IntelliSense cho lệnh LaTeX, trích dẫn và tham chiếu.
- Đánh dấu lỗi và cảnh báo từ nhật ký LaTeX.
- Đoạn mã mẫu và phím tắt cho các lệnh LaTeX phổ biến.([Visual Studio Marketplace][2], [GitHub][4])

## So sánh các trình soạn thảo LaTeX

| Tính năng              | LaTeX Workshop (VS Code) | Overleaf            | TeXstudio |
| ---------------------- | ------------------------ | ------------------- | --------- |
| Soạn thảo ngoại tuyến  | ✅                       | ❌ (Chỉ trực tuyến) | ✅        |
| Hợp tác thời gian thực | ❌                       | ✅                  | ❌        |
| Trình xem PDF tích hợp | ✅                       | ✅                  | ✅        |
| Tùy chỉnh              | ✅                       | ❌                  | ✅        |
| Hỗ trợ plugin          | ✅                       | ❌                  | Hạn chế   |

## Hướng dẫn cài đặt

### 1. Cài đặt TeX Live

**Windows:**

1. Tải trình cài đặt TeX Live từ [trang chính thức](https://www.tug.org/texlive/).
2. Chạy trình cài đặt và làm theo hướng dẫn.
3. Sau khi cài đặt, đảm bảo thư mục `bin` của TeX Live được thêm vào biến môi trường PATH của hệ thống.

**macOS:**

1. Cài đặt MacTeX từ [https://tug.org/mactex/](https://tug.org/mactex/).
2. Làm theo hướng dẫn cài đặt được cung cấp.

**Linux (Debian/Ubuntu):**

```bash
sudo apt update
sudo apt install texlive-full
```

### 2. Cài đặt Visual Studio Code

Tải và cài đặt VS Code từ [trang chính thức](https://code.visualstudio.com/).

### 3. Cài đặt tiện ích LaTeX Workshop

1. Mở VS Code.
2. Đi tới phần Tiện ích bằng cách nhấp vào biểu tượng Tiện ích trong Thanh hoạt động ở bên cạnh cửa sổ hoặc nhấn `Ctrl+Shift+X`.
3. Tìm kiếm "LaTeX Workshop" và nhấp vào "Cài đặt".

### 4. Cài đặt ChkTeX (Tùy chọn nhưng được khuyến nghị)

**Windows:**

1. Mở Command Prompt với quyền Quản trị viên.
2. Chạy:

```bash
tlmgr install chktex
```

**macOS/Linux:**

```bash
sudo tlmgr install chktex
```

### 5. Cấu hình LaTeX Workshop (Tùy chọn)

Bạn có thể tùy chỉnh cài đặt LaTeX Workshop bằng cách chỉnh sửa tệp `settings.json`:

1. Trong VS Code, nhấn `Ctrl+,` để mở Cài đặt.
2. Nhấp vào biểu tượng `{}` ở góc trên bên phải để mở `settings.json`.
3. Thêm hoặc chỉnh sửa các cài đặt theo nhu cầu. Ví dụ:

```json
"latex-workshop.latex.autoBuild.run": "onSave",
"latex-workshop.view.pdf.viewer": "tab",
"latex-workshop.latex.outDir": "./out"

```

[1]: https://github.com/kuxuanwang/Texlive-VSCode_Configuration_in_Mac_and_Win10 "Texlive+VSCode Configuration in Mac and Win10 - GitHub"
[2]: https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop "LaTeX Workshop - Visual Studio Marketplace"
[3]: https://paulwintz.com/latex-in-vscode/ "LaTeX in VS Code - Paul Wintz"
[4]: https://github.com/James-Yu/LaTeX-Workshop "Visual Studio Code LaTeX Workshop Extension - GitHub"
[5]: https://www.programmersought.com/article/80104527473/ "LaTeX configuration tutorial under Win10: VS Code + TexLive"
[6]: https://boom1999.github.io/2023/03/27/TexLive%2BVsCode/ "Installation for TexLive under VsCode | Haisenberg - GitHub Pages"
