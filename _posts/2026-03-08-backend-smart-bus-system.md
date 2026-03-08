---
title: "Smart Bus System - Backend API"
date: 2026-03-08
categories: 
  - Projects
  - Backend Development
tags: 
  - Java
  - Spring Boot
  - RESTful API
  - MySQL
excerpt: "Hệ thống backend cho ứng dụng quản lý và theo dõi xe buýt thông minh, cung cấp API RESTful để xử lý về vị trí xe và thông tin tuyến đường."
header:
  teaser: /assets/images/smart-bus-teaser.jpg
  overlay_image: /assets/images/smart-bus-banner.jpg
  overlay_filter: 0.5
---

## Tổng quan dự án

**Smart Bus System Backend** là hệ thống backend API được xây dựng để hỗ trợ ứng dụng quản lý xe buýt thông minh. Dự án cung cấp các API RESTful để quản lý tuyến xe, theo dõi vị trí xe buýt cung cấp thông tin cho người dùng.

## Tính năng chính

### Quản lý tuyến xe
- Tạo và cập nhật thông tin tuyến xe buýt
- Quản lý các điểm dừng trên tuyến
- Tính toán thời gian di chuyển giữa các điểm

### Theo dõi vị trí Real-time
- Tính toán khoảng cách đến điểm dừng tiếp theo

###  Quản lý người dùng
- Xác thực và phân quyền người dùng
- Quản lý thông tin tài xế và hành khách
- Lịch sử hành trình


## Công nghệ sử dụng

| Công nghệ | Mục đích |
|-----------|----------|
| **Java 11+** | Ngôn ngữ lập trình chính |
| **Spring Boot** | Framework backend |
| **Spring Security** | Xác thực và phân quyền |
| **Spring Data JPA** | ORM và database interaction |
| **MySQL** | Database chính |
| **WebSocket** | Real-time communication |
| **JWT** | Token-based authentication |
| **Maven** | Dependency management |

---

**[View on GitHub](https://github.com/camdao/BackEnd-Smart-Bus-System)** | [Report Bug](https://github.com/camdao/BackEnd-Smart-Bus-System/issues) | [Request Feature](https://github.com/camdao/BackEnd-Smart-Bus-System/issues)