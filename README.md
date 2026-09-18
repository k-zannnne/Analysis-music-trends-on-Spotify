#  Analysis of Music Trends on Spotify

Dự án phân tích xu hướng và đặc trưng âm nhạc trên Spotify nhằm tìm hiểu các yếu tố ảnh hưởng đến độ phổ biến (*Popularity*) của bài hát, xu hướng âm nhạc qua các năm và thói quen thưởng thức của người nghe.

---

##  Tổng quan dự án (Project Overview)

Dự án tập trung khai thác bộ dữ liệu từ Spotify bao gồm thông tin chi tiết về bài hát, nghệ sĩ cùng các chỉ số âm thanh đặc trưng (*Audio Features* như `danceability`, `energy`, `valence`, `tempo`,...).

### Mục tiêu chính:
* **Phân tích đặc trưng âm thanh:** Tìm hiểu mối liên hệ giữa các chỉ số như độ sôi động (*energy*), độ bắt nhịp (*danceability*) với mức độ yêu thích của người nghe.
* **Xu hướng theo thời gian:** Phân tích sự thay đổi trong thị hiếu âm nhạc qua các năm và xu hướng độ dài bài hát (*duration*).
* **Xây dựng Dashboard:** Trực quan hóa dữ liệu trên Power BI/Tableau giúp đưa ra cái nhìn tổng quan và các nhận định kinh doanh (*Business Insights*).

---

##  Cấu trúc thư mục (Project Structure)

```text
spotify-trend-analysis/
├── data/
│   ├── raw/                  # File dữ liệu thô gốc (chưa chỉnh sửa)
│   └── processed/            # File dữ liệu sạch dùng cho Power BI Dashboard
├── notebooks/
│   ├── 01_data_cleaning.ipynb # Làm sạch, xử lý dữ liệu & Feature Engineering
│   └── 02_eda_analysis.ipynb # Phân tích khám phá dữ liệu (EDA) & Trực quan hóa
├── dashboards/
│   ├── spotify_dashboard.pbix# File Dashboard Power BI
│   └── screenshots/          # Ảnh chụp giao diện các trang Dashboard
├── .gitignore                # Khai báo loại bỏ file rác, venv, checkpoint
├── requirements.txt          # Danh sách các thư viện Python sử dụng trong dự án
└── README.md                 # Giới thiệu dự án
