# Siêu Nét Player

**Trình xem phim cho Windows: tự upscale mọi video lên 4K bằng NVIDIA RTX Video Super Resolution, và tự làm phụ đề tiếng Việt cho phim tiếng Nhật / Trung / Anh bằng AI chạy ngay trên máy, không cần mạng.**

Cài bằng một cú bấm đúp, tiếng Việt từ đầu đến cuối.

> **Bản mới nhất: [Siêu Nét Player 1.4 beta](../../releases/tag/v1.4-beta)** - tải file `SieuNetPlayer-1.4-beta.zip`. Các bản khác ở mục [Releases](../../releases).
> Gặp lỗi hoặc góp ý: báo ở mục [Issues](../../issues).

## Tính năng

- **Upscale 4K bằng RTX Video Super Resolution** cho mọi video, giữ 10-bit, khử xen kẽ cho DVD / TV 1080i.
- **RTX Video HDR**: biến phim SDR thành HDR bằng một phím (F4).
- **Phụ đề AI tiếng Việt, offline**: tự nhận ngôn ngữ phim, dịch phụ đề có sẵn hoặc tự nghe lời thoại rồi dịch. Không gửi gì lên Internet.
- **Song ngữ** (F5), đổi chỗ / dời vị trí phụ đề, player nhớ lựa chọn cho các phim sau.
- **Dễ dùng**: không cần quyền Administrator, menu chuột phải tiếng Việt, bảng trạng thái (F1).

## Yêu cầu

| | |
|---|---|
| Hệ điều hành | Windows 10 / 11, 64-bit |
| Card đồ hoạ | NVIDIA GeForce RTX 20 trở lên |
| Driver | NVIDIA bản mới |
| Phụ đề AI (tuỳ chọn) | ổ trống khoảng 14 GB, RAM 16 GB trở lên |

## Cài đặt

1. Tải file [`SieuNetPlayer-1.4-beta.zip`](../../releases/download/v1.4-beta/SieuNetPlayer-1.4-beta.zip) (bản 1.4 beta) rồi giải nén.
2. Bấm đúp **CaiDat.bat** và làm theo hướng dẫn.
3. Trong **NVIDIA App > System > Video > RTX Video Enhancement**: bật Super Resolution, Quality = Manual mức 4.
4. Mở lối tắt **Siêu Nét Player**, kéo thả phim vào.

## Phím tắt

| Phím | Việc |
|---|---|
| F1 | Xem trạng thái |
| F2 | Bật / tắt AI upscale |
| F3 | Bật / tắt Phụ đề AI tiếng Việt |
| F4 | Bật / tắt RTX Video HDR |
| F5 | Phụ đề song ngữ |
| F6 | Đổi chỗ tiếng Việt và lời gốc |
| F7 | Dời phụ đề bằng phím mũi tên |

## Bản quyền

Siêu Nét Player là phần mềm miễn phí nhưng **không phải mã nguồn mở**. Bạn được tải và dùng miễn phí; không được sao chép, chỉnh sửa, dịch ngược hay phân phối lại khi chưa có sự đồng ý của tác giả.

Các thành phần bên thứ ba được tải từ nguồn gốc lúc cài và giữ giấy phép riêng của chúng: mpv (GPLv2+), uosc (LGPL-2.1), thumbfast (MPL-2.0), Python (PSF), FFmpeg (GPL-3.0), sherpa-onnx (Apache-2.0), ONNX Runtime (MIT), llama.cpp (MIT); mô hình Silero VAD (MIT), SenseVoice Small (FunASR Model License), Qwen3-ASR (Apache-2.0), Cohere Transcribe (Apache-2.0), Hy-MT2 7B (Apache-2.0).

NVIDIA, GeForce và RTX là thương hiệu của NVIDIA Corporation. Siêu Nét Player là dự án độc lập.