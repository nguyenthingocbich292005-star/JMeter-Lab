# Apache JMeter Performance Testing Lab

## Giới thiệu

Bài thực hành này nhằm tìm hiểu công cụ kiểm thử hiệu năng **Apache JMeter** và thực hiện gửi HTTP Request để kiểm tra thời gian phản hồi của hệ thống.

# Công cụ sử dụng

* Apache JMeter 5.6.3
* Java JDK
* Github

# Các bước thực hiện

## 1. Cài đặt Java

Cài đặt Java JDK để chạy Apache JMeter.

Kiểm tra phiên bản Java:

```bash id="s4yx1w"
java -version
```

## 2. Cài đặt Apache JMeter

Tải JMeter từ trang chủ Apache:

https://jmeter.apache.org/

Sau khi giải nén, chạy file:

```text id="vw4v4m"
jmeter.bat
```

## 3. Tạo Test Plan

Trong JMeter thực hiện:

* Tạo Thread Group
* Tạo HTTP Request
* Thêm Listener:

  * View Results Tree
  * Summary Report

## 4. Cấu hình kiểm thử

| Thành phần        | Giá trị |
| ----------------- | ------- |
| Number of Threads | 1       |
| Ramp-Up Period    | 1       |
| Loop Count        | 1       |
| Method            | GET     |


# Kết quả thực hiện

## Summary Report

<img width="1511" height="949" alt="Screenshot 2026-06-03 180829" src="https://github.com/user-attachments/assets/eca57203-74eb-4fc6-aee7-d9e93490f075" />


## Kết quả phân tích

| Thông số              | Giá trị  |
| --------------------- | -------- |
| # Samples             | 1        |
| Average Response Time | 1005 ms  |
| Min                   | 1005 ms  |
| Max                   | 1005 ms  |
| Error %               | 0.00%    |
| Throughput            | 59.7/min |

# Nhận xét

* Request được gửi thành công
* Không xuất hiện lỗi trong quá trình kiểm thử
* Hệ thống phản hồi ổn định
* Có thể sử dụng Summary Report để theo dõi:

  * thời gian phản hồi
  * số lượng request
  * throughput
  * tỷ lệ lỗi

# File đính kèm

* `ngocbich-jmeter-test.jmx`

# Kiến thức học được

Sau bài thực hành em đã:

* Biết cách cài đặt Apache JMeter
* Tạo HTTP Request
* Chạy Performance Test
* Đọc kết quả Summary Report
* Sử dụng Github để lưu trữ bài thực hành

# Tài liệu tham khảo

Video hướng dẫn:

https://www.youtube.com/watch?v=NTyY8wKSvik
