# Titanic - Machine Learning from Disaster

#### Summer 2025 EDA Project @rhynofuyu

---

## 1. Giới thiệu

Dự án này thực hiện phân tích dữ liệu thám hiểm (EDA) trên bộ dữ liệu Titanic nổi tiếng, nhằm tìm hiểu các yếu tố ảnh hưởng đến khả năng sống sót của hành khách.

---

## 2. Tổng quan dữ liệu

- **Nguồn dữ liệu:** Titanic-Dataset.csv
- **Các biến chính:**
  - Categorical: Survived, Pclass, Sex, SibSp, Parch, Embarked
  - Numerical: Age, Fare

---

## 3. Phân tích biến phân loại

### 3.1. Tỉ lệ sống sót (`Survived`)
- Số lượng và tỉ lệ sống sót được trình bày bằng bảng và biểu đồ cột.

### 3.2. Giới tính (`Sex`)
- Nữ có tỉ lệ sống sót cao gấp ~4 lần nam.
- Biểu đồ so sánh tỉ lệ sống sót theo giới tính.

### 3.3. Hạng vé (`Pclass`)
- Hành khách hạng 1 có tỉ lệ sống sót cao nhất, tiếp theo là hạng 2, thấp nhất là hạng 3.

### 3.4. Gia đình đi cùng (`SibSp`, `Parch`)
- Đi một mình có tỉ lệ tử vong cao hơn.
- Có 1-2 người thân đi cùng giúp tăng khả năng sống sót.

### 3.5. Cảng lên tàu (`Embarked`)
- Southampton có tỉ lệ tử vong cao nhất, Cherbourg thấp nhất.

---

## 4. Phân tích biến số

### 4.1. Tuổi (`Age`)
- Trẻ em (0-5 tuổi): tỉ lệ sống sót cao nhất (~67.5%)
- Người già (65+): tỉ lệ sống sót gần như 0%
- Người trưởng thành (20-30): tỉ lệ sống sót thấp (~34-36%)

### 4.2. Giá vé (`Fare`)
- Giá vé càng cao, tỉ lệ sống sót càng lớn.
- Hành khách trả giá vé cao có ưu tiên lên xuồng cứu sinh.

---

## 5. Phân tích kết hợp

- **Giới tính + Hạng vé:** Nữ ở hạng 1, 2 có tỉ lệ sống sót vượt trội.
- **Gia đình nhỏ (1-3 người):** Tỉ lệ sống sót tốt nhất.
- **Kết hợp nhiều biến:** Heatmap thể hiện rõ các nhóm có khả năng sống sót cao/thấp.

---

## 6. Kết luận EDA

- **Yếu tố quan trọng nhất:** Giới tính, tuổi, hạng vé.
- **Nguyên tắc "phụ nữ và trẻ em trước" được áp dụng rõ rệt.**
- **Địa vị xã hội và kinh tế ảnh hưởng lớn đến khả năng sống sót.**
