# OOP_JAVA_PROJECT1
Web theo dõi sức khỏe dành cho người dùng. Cung cấp các lời khuyên và tính toán các chỉ số về cơ thể

Thành viên nhóm
1. Bạch Hồng Vinh
2. Hoàng Đức Hiếu
3. Đào Tuấn Phong
   
Mô tả 
1. Xác định yêu cầu
Chức năng chính:
•	Theo dõi sức khỏe: Người dùng có thể nhập thông tin về cân nặng, chiều cao, chỉ số BMI, và các thông tin sức khỏe khác.
•	Cung cấp thông tin dinh dưỡng: Cung cấp các kế hoạch ăn uống phù hợp với mục tiêu sức khỏe của người dùng (giảm cân, tăng cơ, duy trì sức khỏe).
•	Đề xuất bài tập thể dục: Cung cấp các bài tập thể dục dựa trên mục tiêu sức khỏe và thể trạng của người dùng.
•	Theo dõi tiến độ: Cho phép người dùng theo dõi sự tiến bộ của họ qua thời gian.
•	Gợi ý và nhắc nhở: Gửi thông báo nhắc nhở về việc tập luyện và ăn uống.

Yêu cầu phi chức năng:
•	Giao diện thân thiện: Dễ sử dụng và trực quan cho người dùng.
•	Bảo mật thông tin: Đảm bảo bảo mật dữ liệu sức khỏe của người dùng.
•	Tương thích đa nền tảng: Có thể truy cập và sử dụng trên di động và máy tính.

2. Phân tích thiết kế ra lớp
Dưới đây là một số lớp chính có thể có trong ứng dụng:
•	User: Lớp đại diện cho người dùng. Chứa thông tin cá nhân và tiến độ sức khỏe.
•	HealthRecord: Lớp để lưu trữ thông tin sức khỏe như cân nặng, chiều cao, chỉ số BMI.
•	DietPlan: Lớp cho kế hoạch ăn uống, bao gồm các món ăn và lượng calo.
•	ExercisePlan: Lớp cho bài tập thể dục, bao gồm loại bài tập và thời gian thực hiện.
•	ProgressTracker: Lớp để theo dõi tiến độ sức khỏe và mục tiêu của người dùng.
•	Notification: Lớp để quản lý thông báo và nhắc nhở cho người dùng.

3. Xây dựng biểu đồ lớp (UML)
Dưới đây là mô tả bằng văn bản về biểu đồ lớp:

![image](https://github.com/user-attachments/assets/8e4bade6-261e-4ffa-b580-c40bb702a0d6)


+-----------------+
|      User       |
+-----------------+
| - userID        |
| - name          |
| - age           |
| - email         |
| - password      |
+-----------------+
| + register()    |
| + login()       |
| + updateInfo()  |
+-----------------+



+-----------------+
|   HealthRecord  |
+-----------------+
| - height        |
| - weight        |
| - bmi           |
| - healthStatus  |
+-----------------+
| + updateRecord()|
| + getBMI()      |
+-----------------+

+-----------------+
|    DietPlan     |
+-----------------+
| - meals         |
| - calories      |
+-----------------+
| + addMeal()     |
| + removeMeal()  |
| + getPlan()     |
+-----------------+

+-----------------+
|   ExercisePlan  |
+-----------------+
| - exercises     |
| - duration      |
+-----------------+
| + addExercise() |
| + removeExercise()|
| + getPlan()     |
+-----------------+

+-----------------+
| ProgressTracker  |
+-----------------+
| - goals         |
| - progress      |
+-----------------+
| + trackProgress()|
| + setGoals()    |
+-----------------+

+-----------------+
|   Notification   |
+-----------------+
| - message       |
| - date          |
+-----------------+
| + sendReminder()|
| + schedule()    |
+-----------------+
