---
title: "Ticket Online - Movie Ticket Booking System"
date: 2026-03-09
categories:
  - Projects
  - Full-Stack Development
tags:
  - Java
  - Spring Boot
  - Thymeleaf
  - Spring Security
  - MySQL
  - Web Application
excerpt: "Dự án MVP (Minimum Viable Product) xây dựng API đặt vé xem phim, tập trung vào việc sử dụng Redis để xử lý cơ chế giữ chỗ (seat-locking) tạm thời."
header:
  teaser: /assets/images/ticket-online-teaser.jpg # Bạn cần tạo ảnh này
  overlay_image: /assets/images/ticket-online-banner.jpg # và ảnh này
  overlay_filter: 0.5
---

## 🎬 Tổng quan dự án

**Ticket Online** là một dự án MVP (Minimum Viable Product) được xây dựng để thử nghiệm và triển khai giải pháp API cho việc đặt vé xem phim. Trọng tâm của dự án là phát triển cơ chế **giữ chỗ (seat locking)** hiệu quả bằng cách sử dụng **Redis**, đảm bảo không xảy ra xung đột khi nhiều người dùng cùng đặt một ghế.

Đây không phải là một ứng dụng full-stack hoàn chỉnh mà là một backend service tập trung vào việc xử lý logic nghiệp vụ cốt lõi của việc đặt vé.

## ✨ Tính năng chính (MVP)

- **API giữ chỗ tạm thời**: Khi người dùng chọn một ghế, hệ thống sẽ sử dụng Redis để "khóa" ghế đó trong một khoảng thời gian nhất định (ví dụ: 5 phút).
- **API xác nhận đặt vé**: Nếu người dùng hoàn tất thanh toán trong thời gian giữ chỗ, ghế sẽ được đánh dấu là đã bán.
- **API giải phóng ghế**: Nếu người dùng không hoàn tất hoặc hủy bỏ, ghế sẽ được tự động giải phóng sau khi hết thời gian khóa.
- **API xem trạng thái ghế**: Cung cấp thông tin real-time về trạng thái của các ghế trong một suất chiếu.

## 🛠️ Công nghệ sử dụng

| Công nghệ | Mục đích |
|-----------|----------|
| **Java 11+** | Ngôn ngữ lập trình chính |
| **Spring Boot** | Framework để xây dựng API |
| **Redis** | Caching và xử lý giữ chỗ tạm thời |
| **Spring Data JPA** | Tương tác với cơ sở dữ liệu |
| **MySQL** | Lưu trữ dữ liệu chính (phim, suất chiếu, vé đã bán) |
| **Maven** | Quản lý dependencies |

---

⭐ **[View on GitHub](https://github.com/camdao/ticket-online)** | 🐛 [Report Bug](https://github.com/camdao/ticket-online/issues)
