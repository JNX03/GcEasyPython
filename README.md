## การทำงานของ `if`, `if-else`, `else`, `while loop`, `for loop`, การอ่านและเขียนไฟล์, และ List ใน Python

### 1. การใช้งานคำสั่ง `if`, `if-else`, และ `else`
คำสั่ง `if` และ `else` ใช้ในการควบคุมทิศทางของโปรแกรม โดยตรวจสอบเงื่อนไขและทำงานตามที่กำหนด

#### คำสั่ง `if`:
```python
age = 18
if age >= 18:
    print("คุณเป็นผู้ใหญ่")
```

#### คำสั่ง `if-else`:
```python
age = 16
if age >= 18:
    print("คุณเป็นผู้ใหญ่")
else:
    print("คุณยังเป็นเด็ก")
```

#### คำสั่ง `elif` (else if):
```python
score = 75
if score >= 90:
    print("คุณได้เกรด A")
elif score >= 80:
    print("คุณได้เกรด B")
elif score >= 70:
    print("คุณได้เกรด C")
else:
    print("คุณต้องปรับปรุง")
```

### 2. การใช้งาน `while loop` และ `for loop`
การใช้ `while` และ `for` loops ใช้สำหรับการวนซ้ำใน Python

#### `while loop`:
```python
i = 1
while i <= 5:
    print(i)
    i += 1  # เพิ่มค่า i ทีละ 1 ทุกครั้งที่วนลูป
```

#### `for loop`:
```python
for i in range(1, 6):
    print(i)
```

#### คำสั่ง `break` และ `continue`:
```python
# การใช้ break
i = 1
while i <= 10:
    if i == 5:
        break  # หยุดลูปเมื่อ i เท่ากับ 5
    print(i)
    i += 1

# การใช้ continue
for i in range(1, 6):
    if i == 3:
        continue  # ข้ามการพิมพ์ค่า i เมื่อ i เท่ากับ 3
    print(i)
```

### 3. การเขียนและอ่านไฟล์
Python มีคำสั่งสำหรับการอ่านและเขียนไฟล์

#### การเปิดไฟล์และอ่านข้อมูล:
```python
# อ่านทั้งไฟล์
file = open('filename.txt', 'r')
content = file.read()  # อ่านข้อมูลทั้งหมดในไฟล์
print(content)
file.close()  # ปิดไฟล์หลังจากอ่านเสร็จ
```

#### การเขียนไฟล์:
```python
# เขียนข้อมูลใหม่ลงไฟล์
file = open('filename.txt', 'w')
file.write("Hello, World!\n")  # เขียนข้อมูลลงในไฟล์
file.close()
```

#### การใช้งาน `with`:
```python
# อ่านไฟล์ด้วย with
with open('filename.txt', 'r') as file:
    content = file.read()
    print(content)

# เขียนไฟล์ด้วย with
with open('filename.txt', 'w') as file:
    file.write("This is a new line.")
```

### 4. การใช้งาน List
ใน Python `List` ใช้สำหรับเก็บข้อมูลหลายค่าภายในตัวแปรเดียว สามารถเข้าถึงค่าต่าง ๆ ได้ผ่าน index

```python
List = [x, y, z]
```

#### การจัด index ของ List:
- จากซ้ายไปขวา: `0, 1, 2`
- จากขวาไปซ้าย (index ติดลบ): `-1, -2, -3`

#### การใช้ `for` loop กับ List:
```python
for num in List:
    print(num)
```

คำสั่งนี้จะทำให้ `num` ถูกแทนที่ด้วยแต่ละค่าใน List เริ่มจากตัวแรกไปจนถึงตัวท้ายสุด

---

### เพื่อทดลองการทำงานของ Python

สามารถทดสอบคำสั่งต่าง ๆ และเรียนรู้เพิ่มเติมผ่าน [Google Colab ที่นี่](https://colab.research.google.com/drive/1JI7sZ5Ed4nyACaCvFtIpCR3bWvpXLV9d?usp=sharing). 
