# Changelog

Mọi thay đổi đáng chú ý của AIMS-mini được ghi lại trong tệp này.

Định dạng theo [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
đánh số phiên bản theo [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2026-11-06

Bản phát hành Lab 05 (`release/lab05`).

### Added
- `Cart.sort_by_title()` và `Cart.sort_by_cost()` sắp xếp giỏ hàng
- `aims.search.search_by_category()` tìm đĩa theo thể loại
- CI với GitHub Actions: chạy test cho mọi PR vào `master` và `release/**`

### Fixed
- `search_by_title()` không phân biệt hoa thường (#24)

## [1.0.0] - 2026-11-06

Phiên bản ổn định đầu tiên (Lab 04).

### Added
- `aims.__version__` và dòng in phiên bản `AIMS-mini v1.0.0` khi chạy `main.py`
- `CHANGELOG.md`

### Changed
- Cam kết API công khai ổn định: `Cart`, `DigitalVideoDisc`, `search_by_title()`

## [0.3.0] - 2026-11-05

Bản nộp Lab 03 (`release/lab03`).

### Added
- `Cart.total_cost_with_discount(percent)` tính tổng tiền sau giảm giá (#11)
- Thông báo giỏ hàng bằng tiếng Việt (#12)
- Bộ test `tests/test_cart.py`, `tests/test_discount.py`

### Fixed
- Giỏ hàng nhận đĩa thứ 21 dù giới hạn là 20 (#10)
- `total_cost_with_discount()` trả về số tiền được giảm thay vì tổng sau giảm;
  thêm kiểm tra `percent` trong khoảng 0–100 (#9)

### Removed
- Hiển thị tiêu đề đĩa trong thông báo thêm đĩa (#13), đã được revert (#15)

## [0.2.0] - 2026-11-05

Bản nộp Lab 02 (`release/lab02`).

### Added
- `Cart.print_cart()` in chi tiết giỏ hàng; báo "The cart is empty" khi giỏ trống (#4)
- `aims.search.search_by_title()` tìm đĩa theo tiêu đề (#5)
- Biểu đồ use case `docs/use-case.md` (#6)
- Pull request template (#3)

## [0.1.0] - 2026-11-05

Bản nộp Lab 01 (`release/lab01`).

### Added
- Lớp `DigitalVideoDisc`, `Cart` và chương trình demo `main.py`

### Changed
- Chuyển mã nguồn vào package `aims/` (#1)

[Unreleased]: https://github.com/DHTHEFOOL/it3180-202416515-aims/compare/v1.1.0...HEAD
[1.1.0]: https://github.com/DHTHEFOOL/it3180-202416515-aims/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/DHTHEFOOL/it3180-202416515-aims/compare/v0.3.0...v1.0.0
[0.3.0]: https://github.com/DHTHEFOOL/it3180-202416515-aims/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/DHTHEFOOL/it3180-202416515-aims/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/DHTHEFOOL/it3180-202416515-aims/releases/tag/v0.1.0
