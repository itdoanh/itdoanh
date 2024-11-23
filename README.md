Hi fellows👋
- 👋 Hi, I’m Đoàn Văn Doanh
- 📫 How to reach me: <a href="https://fb.com/itdoanh">Facebook</a>

INSERT INTO KHACHHANG (ma_kh, ho_ten, n_sinh, dia_chi, so_dt, ngay_mh, gia_tri_hd) VALUES
('KH001', 'Nguyen Van A', '1980-05-10', 'Hanoi', '0123456789', '2015-01-01', 500000),
('KH002', 'Tran Thi B', '1990-08-20', 'HCM', '0123456790', '2016-03-15', 300000),
('KH003', 'Le Thi C', '1985-12-30', 'Da Nang', '0123456791', '2017-06-25', 450000);

INSERT INTO NHANVIEN (ma_nv, ten_nv, so_dt, ngay_vao_lam) VALUES
('NV001', 'Nguyen Van B', '0123456789', '2015-01-01'),
('NV002', 'Tran Thi D', '0123456792', '2016-02-15'),
('NV003', 'Le Thi E', '0123456793', '2017-05-20');

INSERT INTO SANPHAM (ma_sp, ten_sp, dvt, noi_sx, don_gia) VALUES
('SP001', 'Dau Xao', 'cay', 'Trung Quoc', 35000),
('SP002', 'Mung Tay', 'quyen', 'Viet Nam', 25000),
('SP003', 'Banh Bao', 'cay', 'Trung Quoc', 15000),
('SP004', 'Gao', 'kg', 'Viet Nam', 20000),
('SP005', 'Nuoc Yen', 'chai', 'Singapore', 60000);

INSERT INTO HOADON (ma_hd, t_gian, ma_kh, ma_nv, gia_tri_hd) VALUES
('HD001', '2017-01-01', 'KH001', 'NV001', 500000),
('HD002', '2017-01-02', 'KH002', 'NV002', 300000),
('HD003', '2017-01-02', 'KH003', 'NV003', 450000);

INSERT INTO CTHOPDONG (ma_hd, ma_sp, so_luong) VALUES
('HD001', 'SP001', 10),
('HD001', 'SP002', 5),
('HD002', 'SP003', 7),
('HD003', 'SP004', 3);

-- Dữ liệu cho bảng Khoa
INSERT INTO Khoa (makhoa, tenkhoa, dienthoai) VALUES
('K01', 'Toan', '0123456789'),
('K02', 'DaiLy', '0123456790'),
('K03', 'QLTN', '0123456791');
GO

-- Dữ liệu cho bảng GiangVien
INSERT INTO GiangVien (magv, hotengv, luong, makhoa) VALUES
(1, 'Nguyen Thi A', 10000, 'K01'),
(2, 'Tran Thi B', 12000, 'K02'),
(3, 'Le Thi C', 11000, 'K01');
GO

-- Dữ liệu cho bảng SinhVien
INSERT INTO SinhVien (masv, hotensv, makhoa, namsinh, quequan) VALUES
(101, 'Le Van Son', 'K01', 1995, 'Hanoi'),
(102, 'Nguyen Minh Hieu', 'K02', 1996, 'HCM'),
(103, 'Pham Mai Lan', 'K03', 1997, 'Da Nang'),
(104, 'Hoang Anh Tuan', 'K01', 1995, 'Hanoi');
GO

-- Dữ liệu cho bảng DeTai
INSERT INTO DeTai (madt, tendt, kinhphi, NoiThucTap) VALUES
('DT01', 'Phan Mem Quan Ly', 5000000, 'HCM'),
('DT02', 'Xay Dung Web', 3000000, 'Hanoi'),
('DT03', 'Phat Trien App', 7000000, 'Da Nang');
GO

-- Dữ liệu cho bảng HuongDan
INSERT INTO HuongDan (masv, madt, magv, ketqua) VALUES
(101, 'DT01', 1, 8),
(102, 'DT02', 2, 7),
(103, 'DT03', 3, 9),
(104, 'DT01', 1, 6);
GO
