## Relational_Data_Model

1) NhanVien (MaNV, HoTen, ChucVu, Sdt, Email, GioiTinh, NgaySinh, DiaChi, LoaiNV, NgayVaoLam, Muc Luong,  #MaBP)
2) NhanVienThuNgan (#NVTN_Ma,TrinhDo, TongDoanhThuCa)
3) NhanVienBanHang (#NVBH_Ma, SoLuongKhachHangTuVan, DoanhSoCaNhan)
4) NhanVienQuanLyGiaoHang (#NVQLGH_Ma, KinhNghiem)
5) NhanVienKho (#NVK_Ma, SolanKiemKe)
6) NhanVienChamSocKhachHang (#NVCSKH_Ma, DiemDanhGiaHaiLong)
7) QuanLiCuaHang (#QLCH_Ma, NgayBoNhiem)
8) BoPhan (MaBP, TenBoPhan, #QLCH_Ma)
9) KhachHang (MaKH, HoTen, SoDienThoai, DiaChi)
10) SanPhamGoc (MaSP, TenSP, GiaGoc, #MaLoaiSP, #MaBST)
11) BienTheSP(MaBT, TenBienThe, MucTonKhoToiThieu, SoLuongTonKho, #MaSP)
12) LoaiSanPham (MaLoaiSP, TenLoaiSP)
13) BoSuuTap(MaBST, TenBST, NgayRaMat, MoTa)
14) ThuocTinh(MaThuocTinh, TenThuocTinh, GhiChu)
15) GiaTriThuocTinh(MaGiaTri, GiaTri, #MaThuocTinh)
16) PhieuDatHang (MaPhieuDH, TongTien, NgayTao, GhiChu, #NVBH_Ma)
17) HoaDon (MaHD, TongTienThanhToan, TrangThaiThanhToan,PhuongThucThanhToan, NgayTao, GhiChu, #MaPhieuDH,  #NVTN_Ma )
18) PhieuDoiTra (MaPhieuDoiTra, SoLuongSPDoiTra, TrangThaiDoiTra, LyDo, NgayYeuCau, NgayTao, #NVTN_Ma, #MaHD, #MaKH)
19) KhuyenMai (MaKM, MucGiamGia, DieuKienApDung, #QLCH_Ma)
20) KhieuNaiKhachHang (MaKhieuNai, NoiDung, TrangThaiXuLy, NgayGuiPhanHoi, #MaKH)
21) DonGiaoHang (MaDonGiao, NgayBatDauGiao, GhiChu, NgayTao, #NVGH_Ma, #MaPhieuDH, #Ma_DonViVC)
22) DonViVanChuyen (MaDonViVC, TenDonViVC)
23) PhieuXuatKho (MaPhieuXuat, NgayTao, GhiChu, #NVK_Ma, #MaPhieuDH)
24) PhieuNhapKho (MaPhieuNhap, NgayTao, GhiChu, #NVK_Ma, #MaCongTy)
25) CongTyCungCap (MaCongTy, TenCongTy)
26) BienTheSP_GiaTriThuocTinh
ThuocTinhCuaBienThe(#MaBT, #MaGiaTri)
27) SanPham_PhieuDatHang
ChiTietDonDatHang(#MaSP, #MaPhieuDH, SoLuongSanPham, GiaSanPhamKhiDat)
28) SanPham_PhieuXuatKho
ChiTietPhieuXuatKho(#MaSP, #MaPhieuXuat, SoLuongSPXuat)
29) SanPham_PhieuNhapKho
ChiTietPhieuNhapKho (#MaSP, #MaPhieuNhap, SoLuongSPNhap)
30) CongTyCungCap_SP (#MaSP, #MaCongTy, SoLuongSPCungCap)
31) PhieuDatHang_KhuyenMai
DonDHApDungKM(#MaPhieuDH, #MaKM, NgayApDung, TyLeGiamThucTe, GhiChu)
32) BienTheSP_KhuyenMai
SPApDungKM(#MaBT, #MaKM, NgayApDung, TyLeGiamThucTe, GhiChu)
33) KNKH_NVCSKH 
ChiTietXuLyKhieuNai(#MaKhieuNai, #NVCSKH_Ma, NgayXuLy, GhiChu, KetQuaXuLy) 
