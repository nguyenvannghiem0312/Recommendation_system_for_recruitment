# Hướng dẫn chạy code

1. **Yêu cầu tiên quyết**
    - Đảm bảo bạn đã cài đặt Python trên máy tính của mình. Nếu chưa, bạn có thể tải Python tại https://www.python.org/ và cài đặt theo hướng dẫn.
    - Phiên bản Python nhóm sử dụng là Python 3.10.9

2. **Mã nguồn**
    - Đảm bảo phải có mã nguồn của dự án.

3. **Cài đặt thư viện phụ thuộc**
    - Mở terminal hoặc command prompt, điều hướng đến thư mực chứa file requirements.txt.
    - Chạy lệnh sau để cài đặt các thư viện cần thiết:
        ```
        pip install -r requirements.txt
        ```
    - Cần cài gói en_core_web_sm của Spacy để chạy được NER:
        ```
        python -m spacy download en_core_web_sm
        ```
    Hoặc cài theo hướng dẫn tại đường link: https://realpython.com/natural-language-processing-spacy-python/#lemmatization
4. **Dữ liệu**
    - Đảm bảo phải có Data để chạy chương trình bao gồm:
    + Job-description: 897 file .json.
    + resume: 897 file .json.
    + match_paraphrase-MiniLM-L6-v2.csv là file chứa kết quả các độ đo mà nhóm đã chạy trước.
5. **Chạy code**
    - Cần chỉnh sửa đường dẫn dẫn đến file data ngay ở Cell 2 theo thư muc.
    - Nhấn "Run All" để chạy toàn bộ cell
    - Chỉnh sửa các thông số của mô hình ở Cell 1 tiêu dề "Thử nghiệm" và gọi đến hàm "recommend_top_k_cv"

5. **Xem kết quả**
    - Sau khi chạy thành công, chương trình sẽ hiển thị kết quả.

6. **Sửa lỗi (nếu có)**
    - Nếu gặp lỗi trong quá trình chạy, hãy xem thông báo lỗi để tìm hiểu nguyên nhân.
    - Kiểm tra lại các yêu cầu tiên quyết và cài đặt lại thư viện phụ thuộc nếu cần thiết.
    - Kiểm tra mã nguồn và điều chỉnh các lỗi nếu có.

Lưu ý: Hướng dẫn chạy code này chỉ mang tính chất tổng quan. Các dự án cụ thể có thể có cấu hình và yêu cầu riêng, vui lòng kiểm tra tài liệu và mã nguồn của dự án cụ thể để biết cách chạy chính xác. Nếu có thắc mắc về code, vui lòng liên hệ: nghiem.nv206206@sis.hust.edu.vn, son.nh206165@sis.hust.edu.vn, hai.td20206197@sis.hust.edu.vn
