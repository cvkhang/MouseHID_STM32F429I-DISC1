# 🖱️ MouseHID_STM32F429I-DISCO

Dự án sử dụng **TouchGFX** trên bo mạch **STM32F429I-DISCO** với các tính năng:

- Di chuyển con trỏ chuột qua ILI9341  
- Click trái, click phải, giữ chuột bằng nút vật lý
- Cuộn trang bằng joystick  
- Ghi & phát lại thao tác chuột (macro)
- Điều chỉnh độ nhạy chuột và cuộn qua giao diện TouchGFX  

**Demo:** [bit.ly/demo-he-nhung](https://www.bit.ly/demo-he-nhung)
---

## 🧰 Công cụ & Phiên bản

| Công cụ                   | Phiên bản khuyến nghị |
|---------------------------|-----------------------|
| STM32CubeMX               | 6.14.0                |
| TouchGFX Designer         | 4.25.0                |
| STM32Cube FW F4           | 1.28.1                |
| STM32CubeIDE              | ≥ 1.13.0              |
| EWARM / MDK-ARM (tùy chọn)| 8.50.9                |
| STM32CubeProgrammer       | Mới nhất              |

---

## ⚙️ Hướng dẫn cài đặt & Build

1. **Cài đặt công cụ** theo bảng trên.  
2. **Clone** repo về máy:
   ```bash
   git clone https://github.com/cvkhang/MouseHID_STM32F429I-DIS1.git
   cd MouseHID_STM32F429I-DIS1
   ```
3. **Mở file** `STM32F429I_DISCO_REV_D01.ioc` bằng **STM32CubeMX**, chọn IDE (CubeIDE/EWARM/MDK-ARM) → **Generate Code**.  
4. **Mở project** trong thư mục tương ứng (ví dụ `STM32CubeIDE/`), rồi **Build** (Ctrl+B).  
5. **Kết nối bo mạch**, dùng **STM32CubeProgrammer** để nạp firmware (`.hex`/`.bin`).  
