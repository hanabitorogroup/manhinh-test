# King Long Motion Menu Lab

Prototype độc lập cho màn hình quảng cáo/menu động 16:9. Repo này không kết nối Firebase và không phụ thuộc app production.

## Chạy
Mở `index.html` bằng trình duyệt hoặc static server. Màn hình tự chạy 3 scene, mỗi scene 8 giây.

## Điều khiển
- ← / →: scene trước/sau
- Space: pause/play
- F hoặc nút ⛶: fullscreen

## Kiến trúc
- `js/scenes.js`: dữ liệu scene
- `js/player.js`: timeline/player
- `css/screen.css`: renderer + animation

Bản lab dùng hình món minh hoạ bằng CSS để kiểm tra motion engine. Khi duyệt chuyển động, có thể thay bằng PNG/WebP món thật nền trong suốt mà không đổi player.

## Mục tiêu
TV 1920×1080 chạy quảng cáo theo layer: background → food → headline → description → price, thay vì render sẵn MP4.