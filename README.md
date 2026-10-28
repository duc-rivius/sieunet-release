# Siêu Nét Player

**Trình xem phim cho Windows: tự upscale mọi video lên 4K bằng NVIDIA RTX Video Super Resolution, và tự làm phụ đề tiếng Việt cho phim tiếng Nhật / Trung / Anh bằng AI chạy ngay trên máy, không cần mạng.**

Cài bằng một cú bấm đúp, tiếng Việt từ đầu đến cuối.

> **Bản mới nhất: [Siêu Nét Player 1.5.2 beta](../../releases/tag/v1.5.2-beta)** - tải file `SieuNetPlayer-1.5.2-beta.zip`. Các bản khác ở mục [Releases](../../releases).
> Gặp lỗi hoặc góp ý: báo ở mục [Issues](../../issues).

## Có gì mới trong 1.5.2 beta

- **Sửa lỗi không thấy "Đang dịch phụ đề… %"** khi tua tới đoạn chưa dịch: nay phần trăm hiện rõ ngay chỗ phụ đề và tăng dần tới khi phụ đề có.
- Màn hình chờ khi mở phim không còn tắt sớm khi phụ đề chưa sẵn sàng.

## Có gì mới trong 1.5.1 beta

- **Sửa lỗi player không mở được** trên máy không có card NVIDIA, và trên máy card đồ hoạ đời cũ (thiếu `vulkan-1.dll`, vd Intel HD 4000–5500). Bộ cài tự xử lý, không cần làm gì thêm.
- **Quảng cáo luôn có hình** trên mọi máy, kể cả máy chưa cài Phụ đề AI (trước đây chỉ hiện chữ).

## Có gì mới trong 1.5 beta

- **Phụ đề AI tự lưu vào phim**: dịch xong cả phim thì lưu phụ đề tiếng Việt thành tệp `<tên phim>.vi.srt` ngay cạnh phim. Lần sau mở phim là có phụ đề ngay, không phải chờ dịch lại; chép phim sang máy / thư mục khác thì mang theo tệp này. Không ghi đè tệp `.vi.srt` có sẵn.
- **Tua tới đoạn chưa có phụ đề**: ngay chỗ phụ đề hiện "Đang dịch phụ đề… 45%" cho tới khi đoạn đó dịch xong, rồi phụ đề hiện ngay.
- Sửa lỗi tua lùi về đoạn chưa dịch thì phụ đề có thể chậm tới 30 giây mới hiện.
- **Màn hình chờ khi mở phim**: quảng cáo hiện 5 giây (trước đây có thể kéo dài thêm 15 giây). Phụ đề sẵn sàng là phim phát ngay; phụ đề còn đang dịch thì bấm Enter để xem luôn.
- **Số liệu quảng cáo ẩn danh**: player gửi lượt hiện / bấm quảng cáo kèm một mã máy ngẫu nhiên và cấu hình máy (card đồ hoạ, CPU, RAM, Windows, màn hình) cho người phát hành. Không gửi gì về phim bạn xem. Tắt bằng dòng `stats=no` trong `portable_config\script-opts\ads.conf`.

Cập nhật từ bản cũ: giải nén bản mới rồi chạy `CaiDat.bat`, cài đè được, không phải tải lại mô hình AI.

## Tính năng

- **Upscale 4K bằng RTX Video Super Resolution** cho mọi video, giữ 10-bit, khử xen kẽ cho DVD / TV 1080i.
- **RTX Video HDR**: biến phim SDR thành HDR bằng một phím (F4).
- **Phụ đề AI tiếng Việt, offline**: tự nhận ngôn ngữ phim, dịch phụ đề có sẵn hoặc tự nghe lời thoại rồi dịch. Không gửi âm thanh hay phụ đề lên Internet. Dịch xong thì tự lưu `.vi.srt` cạnh phim.
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

1. Tải file [`SieuNetPlayer-1.5.2-beta.zip`](../../releases/download/v1.5.2-beta/SieuNetPlayer-1.5.2-beta.zip) (bản 1.5.2 beta) rồi giải nén.
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