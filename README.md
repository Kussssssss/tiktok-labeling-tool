# TikTok Content Labeling Tool v2.0

Công cụ gắn nhãn nội dung TikTok với giao diện hiện đại và tính năng nâng cao.

## 🚀 Tính năng chính

### ✨ Giao diện hiện đại
- **Glassmorphism Design**: Giao diện trong suốt với hiệu ứng blur hiện đại
- **Responsive Design**: Tương thích với mọi thiết bị
- **Dark Mode Support**: Hỗ trợ chế độ tối
- **Smooth Animations**: Hiệu ứng chuyển động mượt mà

### 🎯 Tính năng gắn nhãn
- **Multi-label Support**: Gắn nhiều nhãn cho một video
- **Smart Video Loading**: Tự động thử các phương pháp nhúng video
- **Real-time Progress**: Theo dõi tiến độ gắn nhãn
- **Auto-save**: Tự động lưu dữ liệu

### 📊 Quản lý dữ liệu
- **CSV Import/Export**: Hỗ trợ file CSV
- **Local Storage**: Lưu trữ tạm thời trong trình duyệt
- **Backup System**: Hệ thống sao lưu tự động
- **Compression**: Nén dữ liệu để tiết kiệm dung lượng

## 📁 Cấu trúc file

```
tiktok-labeling-tool/
├── index.html          # File HTML chính
├── styles.css          # CSS cho giao diện chính
├── guideline.css       # CSS cho phần hướng dẫn
├── Guideline.csv       # File dữ liệu hướng dẫn
└── README.md           # File hướng dẫn này
```

## 🛠️ Cách sử dụng

### 1. Chuẩn bị dữ liệu
- File CSV cần có cột `id_video` chứa ID video TikTok
- Có thể thêm các cột khác như `username`, `description`, etc.

### 2. Sử dụng công cụ
1. **Mở file**: Chọn file CSV để bắt đầu
2. **Xem video**: Chọn video từ danh sách
3. **Gắn nhãn**: Chọn các nhãn phù hợp
4. **Xuất kết quả**: Tải file CSV đã gắn nhãn

### 3. Các phương pháp nhúng video
- **🎯 Smart Auto**: Tự động thử các phương pháp
- **🎬 oEmbed**: Sử dụng TikTok oEmbed API
- **📺 Blockquote**: Phương pháp nhúng native
- **🔗 External**: Link trực tiếp đến TikTok

## 🎨 Design System

### Màu sắc
```css
--primary-color: hsl(220, 100%, 60%)    /* Xanh dương chính */
--secondary-color: hsl(280, 70%, 70%)   /* Tím phụ */
--accent-color: hsl(350, 85%, 70%)      /* Hồng nhấn */
--success-color: hsl(142, 76%, 60%)     /* Xanh lá */
--warning-color: hsl(45, 95%, 80%)      /* Vàng cảnh báo */
--error-color: hsl(348, 86%, 80%)       /* Đỏ lỗi */
```

### Typography
- **Font chính**: Inter (Google Fonts)
- **Font code**: JetBrains Mono
- **Responsive**: Tự động điều chỉnh kích thước

### Spacing
```css
--space-xs: 0.25rem    /* 4px */
--space-sm: 0.5rem     /* 8px */
--space-md: 1rem       /* 16px */
--space-lg: 1.5rem     /* 24px */
--space-xl: 2rem       /* 32px */
```

## 🔧 Tính năng kỹ thuật

### Video Loading System
- **Parallel Loading**: Tải nhiều phương pháp cùng lúc
- **Caching**: Cache kết quả để tăng tốc
- **Fallback**: Tự động chuyển sang phương pháp khác nếu thất bại

### Data Management
- **Compression**: Sử dụng LZ-String để nén dữ liệu
- **Backup Rotation**: Giữ 5 bản sao lưu gần nhất
- **Validation**: Kiểm tra tính hợp lệ của dữ liệu

### Performance
- **Lazy Loading**: Tải video theo nhu cầu
- **Debouncing**: Tránh gọi API quá nhiều
- **Memory Management**: Tự động dọn dẹp bộ nhớ

## 📱 Responsive Design

### Breakpoints
- **Desktop**: > 1200px
- **Tablet**: 768px - 1200px
- **Mobile**: < 768px

### Mobile Optimizations
- Touch-friendly buttons
- Swipe gestures
- Optimized video player
- Simplified navigation

## 🔒 Bảo mật & Quyền riêng tư

- **Local Processing**: Tất cả dữ liệu xử lý tại máy local
- **No Server**: Không gửi dữ liệu lên server
- **File System Access**: Sử dụng File System Access API (nếu có)

## 🐛 Troubleshooting

### Video không hiển thị
1. Kiểm tra kết nối internet
2. Thử phương pháp nhúng khác
3. Kiểm tra URL video có hợp lệ không

### Lỗi CORS
- Đây là lỗi bình thường từ TikTok
- Không ảnh hưởng đến chức năng gắn nhãn
- Có thể bỏ qua

### Dữ liệu bị mất
1. Kiểm tra localStorage
2. Thử khôi phục từ backup
3. Kiểm tra dung lượng trình duyệt

## 🚀 Tương lai

### Tính năng sắp tới
- [ ] Batch processing
- [ ] AI-assisted labeling
- [ ] Export to multiple formats
- [ ] Collaborative labeling
- [ ] Advanced analytics

### Cải tiến kỹ thuật
- [ ] Service Worker for offline support
- [ ] WebAssembly for better performance
- [ ] IndexedDB for larger datasets
- [ ] WebRTC for real-time collaboration

## 📄 License

MIT License - Xem file LICENSE để biết thêm chi tiết.

## 🤝 Đóng góp

Mọi đóng góp đều được chào đón! Vui lòng:
1. Fork repository
2. Tạo feature branch
3. Commit changes
4. Push to branch
5. Tạo Pull Request

## 📞 Liên hệ

- **Email**: [your-email@example.com]
- **GitHub**: [your-github-username]
- **Issues**: [GitHub Issues](https://github.com/your-repo/issues)

---

**Made with ❤️ for the TikTok research community** 