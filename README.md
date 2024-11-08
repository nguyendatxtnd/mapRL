# lưu ý trước khi mở các map 
1. tải thư mục chứa các model sử dụng trong map về thư mục home:

        git clone https://github.com/nguyendatxtnd/models.git

- build lại worksapce:

        catkin_make
  
2. 
- thay đổi username của thiết bị trong các đường dẫn trong file .world bằng cách chạy file replace_path.py trong package mymap ( sửa biến device_name trong code là username của thiết bị)
- sau đó chạy file launch tương ứng, VD:

          roslaunch file_launch file_map.launch

- khi chạy nếu có gặp lỗi liên quan đến tiến trình gazebo hay xung đột thì có thể thử kiểm tra xem có tiến trình gazebo nào đang chạy hay không thì tắt nó đi, rồi chạy lại.
- kiểm tra các tiến trình gazebo đang chạy:

            ps aux | grep gazebo

- xóa các tiến trình gazebo đang chay:

            pkill -f gazebo
  
