<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:0d1117,50:1a1e2e,100:2d1b69&text=LƯỜNG%20VIỆT%20NHẬT&fontColor=e6edf3&fontSize=42&fontWeight=700&animation=fadeIn&fontAlignY=35&desc=Full-Stack%20Web%20Developer%20·%20Node.js%20·%20React%20·%20MongoDB&descAlignY=55&descSize=16&descColor=a78bfa"/>

<br/>

[![Gmail](https://img.shields.io/badge/nhatluong1252006@gmail.com-0d1117?style=for-the-badge&logo=gmail&logoColor=ea4335)](mailto:nhatluong1252006@gmail.com)
[![GitHub](https://img.shields.io/badge/2006JohCice-0d1117?style=for-the-badge&logo=github&logoColor=e6edf3)](https://github.com/2006JohCice)
[![Facebook](https://img.shields.io/badge/Facebook-0d1117?style=for-the-badge&logo=facebook&logoColor=1877f2)](https://www.facebook.com/luong.viet.nhat.349100)
<!-- [![Portfolio]()](#) -->

<sub>📍 Hà Nội, Việt Nam · Sẵn sàng cho vị trí <b>Full-Stack Web Developer</b> · Fulltime & Onsite</sub>

</div>

---

## 👋 Giới thiệu

Sinh viên năm 3 ngành Công nghệ Thông tin , chuyên phát triển ứng dụng web full-stack với **JavaScript, React 19 và Node.js/Express**.

Thiết kế cơ sở dữ liệu, viết REST API, xử lý xác thực, đến giao diện hoàn chỉnh.

> **Mục tiêu:** Tham gia đội ngũ kỹ thuật thực chiến, học chuẩn quy trình sản phẩm và đóng góp vào codebase ngay trong 3 tháng đầu.

---

<div align="center">

# 🍽️ Oder — Nền tảng quản lý nhà hàng & đặt món trực tuyến

**Multi-tenant SaaS · Tự phát triển từ đầu · Demo vận hành**

<br/>

[![Xem mã nguồn](https://img.shields.io/badge/XEM_MÃ_NGUỒN-2d1b69?style=for-the-badge&logo=github&logoColor=white)](https://github.com/2006JohCice/Oder)
[![Demo trực tiếp](https://img.shields.io/badge/DEMO_TRỰC_TIẾP-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://oder-xi.vercel.app/)

</div>

<br/>

### 📋 Bài toán

Nhiều nhà hàng và cửa hàng F&B nhỏ tại Việt Nam vẫn quản lý đơn hàng bằng sổ tay, gọi điện thoại đặt bàn và không có hệ thống theo dõi doanh thu. Tôi đã xây dựng **một nền tảng hoàn chỉnh** thay thế toàn bộ quy trình đó — từ đặt bàn, gọi món, thanh toán, đến quản trị đa nhà hàng.

### 🏗️ Kiến trúc hệ thống

```
┌─────────────────────────────────────────────────────────────────┐
│                        FRONTEND (React 19)                      │
│  ┌──────────────┐  ┌──────────────────┐  ┌───────────────────┐  │
│  │  🛒 Client   │  │ 🏪 Restaurant    │  │  🛡️ Admin Panel  │  │
│  │   Panel      │  │  Owner Panel     │  │  (Super Admin)    │  │
│  │              │  │                  │  │                   │  │
│  │ • Đặt món    │  │ • Dashboard      │  │ • Quản lý toàn bộ │  │
│  │ • Đặt bàn    │  │ • Quản lý menu   │  │ • RBAC & phân     │  │
│  │ • Thanh toán │  │ • Xử lý đơn      │  │   quyền           │  │
│  │ • Đánh giá   │  │ • Quản lý bàn    │  │ • SEO & Marketing │  │
│  │ • Chat       │  │ • Voucher        │  │ • Báo cáo & Backup│  │
│  │ • AI gợi ý   │  │ • Chat với KH    │  │ • Thông báo       │  │
│  └──────┬───────┘  └────────┬─────────┘  └─────────┬─────────┘  │
│         │                   │                      │            │
│         └───────────────────┼──────────────────────┘            │
│                             │                                   │
│                      REST API + Socket.IO                       │
├─────────────────────────────┼───────────────────────────────────┤
│                        BACKEND (Node.js / Express)              │
│                             │                                   │
│  ┌──────────┐  ┌────────────┴───┐  ┌──────────┐  ┌──────────┐  │
│  │Controllers│  │  Middlewares   │  │ Validate │  │ Helpers  │  │
│  │ (38 files)│  │ Auth/Role/Upload│ │ (Input)  │  │(Mail/JWT)│  │
│  └─────┬────┘  └────────────────┘  └──────────┘  └──────────┘  │
│        │                                                        │
│  ┌─────┴──────────────────────────────────────────────────────┐ │
│  │              MongoDB (22 Collections / Models)              │ │
│  │  User · Product · Order · Cart · Restaurant · Table         │ │
│  │  Voucher · Category · Notification · Chat · Feedback        │ │
│  │  Visit · Policy · SEO · Advertisement · Report ...          │ │
│  └─────────────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────────┘
```

### 🎯 Tính năng chi tiết

<table>
<tr>
<td width="50%">

#### 🛒 Client Panel — Người dùng cuối
- Tìm kiếm nhà hàng, duyệt menu theo danh mục
- Thêm sản phẩm vào giỏ hàng, chỉnh số lượng
- **Đặt bàn online** với chọn khu vực, số khách, thời gian
- Thanh toán đơn hàng kèm áp dụng **voucher giảm giá**
- Theo dõi trạng thái đơn hàng realtime
- **Đánh giá & phản hồi** nhà hàng
- Lưu nhà hàng yêu thích, tích điểm thành viên
- **Chat realtime** với nhà hàng qua Socket.IO
- **Gợi ý món ăn bằng AI** (OpenAI / Google GenAI)
- Hỗ trợ **đa ngôn ngữ** (Tiếng Việt, English, 한국어, Italiano)

</td>
<td width="50%">

#### 🏪 Restaurant Owner Panel — Chủ nhà hàng
- **Dashboard** thống kê doanh thu, đơn hàng, đánh giá (Recharts)
- Quản lý sản phẩm: CRUD, upload ảnh, sắp xếp vị trí
- **Quản lý đơn hàng**: duyệt, cập nhật trạng thái theo vòng đời
- **Sơ đồ bàn trực quan**: kéo thả, chọn hình dạng (tròn/chữ nhật)
- Tạo & quản lý **voucher** (giảm % hoặc giảm tiền cố định)
- Chat với khách hàng, nhận thông báo tin nhắn mới
- Xem & phản hồi đánh giá của khách
- Báo cáo doanh thu theo thời gian

</td>
</tr>
<tr>
<td width="50%">

#### 🛡️ Admin Panel — Quản trị viên hệ thống
- Quản lý toàn bộ nhà hàng trên nền tảng (duyệt/khóa/xóa)
- Quản lý tài khoản: thêm, sửa, xóa, phân quyền
- **RBAC (Role-Based Access Control)** với hệ thống role linh hoạt
- Quản lý danh mục sản phẩm, sản phẩm toàn hệ thống
- **Voucher nền tảng** (platform-wide voucher)
- Quản lý quảng cáo (advertisements)
- **SEO management**: tạo/chỉnh sửa bài viết SEO qua TinyMCE
- **Hệ thống thông báo** cho toàn nền tảng
- Quản lý chính sách, điều khoản sử dụng
- **Backup dữ liệu** sản phẩm
- Cài đặt hệ thống tổng thể

</td>
<td width="50%">

#### ⚙️ Kỹ thuật nổi bật
- **Multi-tenant architecture**: mỗi nhà hàng là một tenant độc lập
- **Realtime communication**: Socket.IO cho chat, typing indicator, thông báo
- **AI Integration**: OpenAI + Google GenAI cho gợi ý món ăn thông minh
- **22 Mongoose models** với database indexing tối ưu
- **38 controller files** phân tách theo Admin/User/Merchant
- **Role system**: User → Owner → Staff → Admin
- **Email system**: Nodemailer + Resend cho OTP & thông báo
- **File upload**: Multer cho ảnh sản phẩm & avatar
- **Fuzzy search**: Fuse.js cho tìm kiếm gần đúng
- **Visit analytics**: Theo dõi lượt truy cập theo ngày
- **Export**: PDF (jsPDF) + Excel (xlsx) cho báo cáo
- **Map integration**: Leaflet cho định vị nhà hàng

</td>
</tr>
</table>

### 🗃️ Cơ sở dữ liệu — 22 Collections

```
📊 Core Business          🔐 Auth & Users           📦 Others
├── Product               ├── UserAccount           ├── Notification
├── Order                 ├── UserAdmin             ├── ChatMessage
├── Cart                  ├── ForgotPassword        ├── Advertisement
├── Restaurant            ├── Decentralization      ├── SeoPost
├── Table                 │   (RBAC)                ├── Policy
├── Voucher               │                         ├── Visit
├── Category              │                         ├── SearchHistory
├── Feedback              │                         └── RestaurantReport
└── InfoUserOrder         │
```

### 🛠️ Technology Stack

<div align="center">

| Layer | Technologies |
|---|---|
| **Frontend** | ![React](https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black) ![Bootstrap](https://img.shields.io/badge/Bootstrap_5-7952B3?style=flat-square&logo=bootstrap&logoColor=white) ![Recharts](https://img.shields.io/badge/Recharts-FF6384?style=flat-square&logoColor=white) ![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=leaflet&logoColor=white) ![i18next](https://img.shields.io/badge/i18next-26A69A?style=flat-square&logo=i18next&logoColor=white) |
| **Backend** | ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express_5-000000?style=flat-square&logo=express&logoColor=white) ![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat-square&logo=socketdotio&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white) |
| **Database** | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat-square&logoColor=white) |
| **AI** | ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) ![Google AI](https://img.shields.io/badge/Google_GenAI-4285F4?style=flat-square&logo=google&logoColor=white) |
| **Tools** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) |

</div>

### 📸 Screenshots

<div align="center">

#### Admin Dashboard
<img width="960" alt="Admin Dashboard" src="https://github.com/user-attachments/assets/536d8125-861f-457e-95ac-136a9fff7dec"/>

#### Product Management
<img width="960" alt="Product Management" src="https://github.com/user-attachments/assets/2601c175-8554-41d1-950d-fdea5b872a6f"/>

#### Role-Based Access Control
<img width="960" alt="RBAC System" src="https://github.com/user-attachments/assets/6fed0274-e59d-4baf-b134-664f7252e196"/>

#### Additional Features
<img width="960" alt="Features" src="https://github.com/user-attachments/assets/7aaa4d8b-5bfe-48ef-b825-57c05c5fadf9"/>

</div>

### 🔐 Demo Credentials

| Panel | Email | Password |
|---|---|---|
| **Admin** | `1234@gmail.com` | `1` |

> ⚠️ Vui lòng không chỉnh sửa hoặc xóa tài khoản demo để người khác cũng có thể trải nghiệm.

### 💡 Bài học rút ra

Đây là dự án **tâm huyết nhất** của tôi — đã trải qua nhiều lần refactor và mở rộng từ một hệ thống quản lý đơn hàng đơn giản thành nền tảng F&B multi-tenant hoàn chỉnh. Ba bài học đáng giá nhất:

1. **Thiết kế database sai từ đầu thì sửa cực kỳ tốn kém** — với 22 model liên kết chặt, thay đổi một schema ảnh hưởng dây chuyền đến controller, validation và frontend.
2. **Multi-tenant architecture đòi hỏi tư duy phân tách dữ liệu ngay từ đầu** — mỗi query đều phải filter theo `restaurant_id`, mỗi middleware đều phải verify quyền sở hữu.
3. **Realtime không chỉ là emit/listen** — phải xử lý room management, reconnection, và notification routing chính xác giữa User ↔ Restaurant ↔ Admin.

---

## 🚀 Dự án khác

<table>
<tr>
<td width="50%">

### 💬 Chatbox — Ứng dụng nhắn tin realtime
> Chat 1-1 và nhóm với Socket.IO, xác thực OTP qua email, hiển thị trạng thái "đang nhập…"

**Stack:** React · Node.js · Express · Socket.IO
<br/>
[→ Xem mã nguồn](https://github.com/2006JohCice/Chatbox)

</td>
<td width="50%">

### 🗺️ WebGIS — Ứng dụng bản đồ & dữ liệu không gian
> Hiển thị và truy vấn dữ liệu bản đồ trên nền web với GeoServer, PostGIS và OpenLayers

**Stack:** JavaScript · PostgreSQL · PostGIS · GeoServer · OpenLayers
<br/>
[→ Xem mã nguồn](https://github.com/2006JohCice/GIS)

</td>
</tr>
<tr>
<td width="50%">

### 🎮 BuyGameShop — Giao diện thương mại điện tử
> Layout responsive trên mọi thiết bị, component hóa bằng JavaScript thuần, không framework

**Stack:** HTML · CSS · JavaScript
<br/>
[→ Xem mã nguồn](https://github.com/2006JohCice/BuyGameShop)

</td>
<td width="50%">

### 📊 Thêm dự án sắp tới...
> Đang phát triển các dự án mới tập trung vào Docker, System Design và Clean Architecture

**Theo dõi GitHub để cập nhật!**

</td>
</tr>
</table>

---

## 🧰 Kỹ năng tổng hợp

| Nhóm | Công nghệ |
|---|---|
| **Ngôn ngữ** | JavaScript, PHP, Java, Python, C/C++, SQL |
| **Frontend** | React 19, Vite, HTML5, CSS3, Bootstrap 5, Responsive Design |
| **Backend** | Node.js, Express 5, REST API, JWT / Cookie Auth, Socket.IO |
| **Cơ sở dữ liệu** | MongoDB, Mongoose, PostgreSQL, PostGIS, MySQL |
| **AI / API** | OpenAI API, Google Generative AI, Nodemailer, Resend |
| **WebGIS** | OpenLayers, GeoServer, QGIS, WMS/WFS |
| **Công cụ** | Git, GitHub, VS Code, Postman, Linux, Vercel |

<sub>Tất cả công nghệ trên đều đã được sử dụng trực tiếp trong các dự án thực tế, không phải chỉ đọc tài liệu.</sub>

---

## 🎓 Học vấn

**Đại học Tài nguyên và Môi trường Hà Nội (HUNRE)** — Hà Nội
<br/>
Sinh viên năm 3 · Dự kiến tốt nghiệp: 2027

Môn học liên quan: Lập trình web, Cơ sở dữ liệu, Hệ thống thông tin địa lý (GIS), Cấu trúc dữ liệu & Giải thuật.

---

## 🎯 Định hướng phát triển

Đang học chuyên sâu để sẵn sàng làm việc ở môi trường sản phẩm thực tế:

`Docker & Deployment` · `System Design` · `Clean Architecture` · `Advanced Node.js` · `Kiểm thử tự động` · `CI/CD`

---

## 📊 Hoạt động GitHub

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=2006JohCice&show_icons=true&hide_border=true&theme=github_dark&bg_color=0D1117&title_color=a78bfa&icon_color=a78bfa&text_color=8b949e&rank_icon=github"/>
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=2006JohCice&layout=compact&hide_border=true&theme=github_dark&bg_color=0D1117&title_color=a78bfa&text_color=8b949e"/>

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=2006JohCice&theme=github-dark-blue&hide_border=true&background=0D1117&ring=a78bfa&fire=a78bfa&currStreakLabel=a78bfa"/>

</div>

---

<div align="center">

### 📬 Liên hệ

Tôi luôn sẵn sàng trao đổi về cơ hội thực tập, việc làm hoặc dự án hợp tác.

**Email:** [nhatluong1252006@gmail.com](mailto:nhatluong1252006@gmail.com)
**GitHub:** [2006JohCice](https://github.com/2006JohCice)

---

<sub>⭐ Nếu bạn thấy dự án hữu ích, hãy cho một star trên GitHub! Cảm ơn bạn đã ghé thăm.</sub>

<sub>Cập nhật lần cuối: 09/2026</sub>

</div>
