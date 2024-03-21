# Group-8---Fake-news-detection---QTDLL-voi-Apache-Spark
Phat hien tin gia
import pandas as pd

# Đọc dữ liệu từ các tệp CSV thành DataFrame
df_fake = pd.read_csv("C:/Users/User/Desktop/Fake.csv")
df_true = pd.read_csv("C:/Users/User/Desktop/True.csv")

# Ghép hai DataFrame theo chiều dọc
df_merge = pd.concat([df_fake, df_true], axis=0)

# Hiển thị 10 dòng đầu tiên của DataFrame kết quả
print(df_merge.head(10))
# Danh sách các tên cột trong DataFrame
df_merge.columns
