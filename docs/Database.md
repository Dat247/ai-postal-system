# AI POSTAL SYSTEM

## Database Design v1.0

## 1. Mục tiêu

Database quản lý toàn bộ hoạt động của bưu cục: - Điểm danh bưu tá -
Hàng đến - Phân công giao hàng - Kết quả phát - Thu gom - Hàng tồn -
KPI - Dashboard - Báo cáo AI - Hội ý đầu ca

## 2. Danh sách Sheet

    STT Sheet        Chức năng
  ----- ------------ ----------------------
      1 CONFIG       Cấu hình hệ thống
      2 EMPLOYEE     Danh sách bưu tá
      3 ROUTE        Danh sách tuyến phát
      4 CUSTOMER     Khách hàng thu gom
      5 ATTENDANCE   Điểm danh
      6 INBOUND      Hàng đến
      7 ASSIGNMENT   Phân công
      8 DELIVERY     Kết quả phát
      9 COLLECTION   Thu gom
     10 INVENTORY    Hàng tồn
     11 KPI          KPI
     12 ALERT        Cảnh báo
     13 REPORT       Báo cáo AI
     14 MEETING      Hội ý đầu ca
     15 DOCUMENT     Văn bản
     16 DASHBOARD    Dashboard
     17 LOG          Nhật ký hệ thống

## 3. EMPLOYEE

  Cột            Kiểu
  -------------- -----------------
  EmployeeID     Text
  EmployeeName   Text
  Phone          Text
  RouteID        Text
  Position       Text
  Status         Active/Inactive

## 4. ROUTE

RouteID, RouteName, District, Target

## 5. ATTENDANCE

Date, EmployeeID, CheckIn, CheckOut, LateMinute, Absent, Remark

## 6. INBOUND

Date, TrackingNo, Service, Weight, RouteID, COD

## 7. ASSIGNMENT

Date, TrackingNo, EmployeeID, AssignTime

## 8. DELIVERY

TrackingNo, EmployeeID, Status, Reason, DeliveryTime

## 9. COLLECTION

Date, CustomerID, EmployeeID, Quantity, Weight

## 10. INVENTORY

TrackingNo, ReceiveDate, DaysInStock, EmployeeID, Status

## 11. KPI

EmployeeID, DeliveryQty, SuccessRate, CollectionQty, InventoryQty,
AttendanceScore, TotalScore

## 12. REPORT

Lưu báo cáo AI.

## 13. MEETING

Lưu nội dung hội ý đầu ca.

## 14. DOCUMENT

Lưu văn bản và tóm tắt AI.

## 15. LOG

Lưu lịch sử hệ thống.
