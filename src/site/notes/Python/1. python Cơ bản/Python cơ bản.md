---
{"aliases":null,"tags":null,"Related":null,"date":null,"URL":null,"Author":null,"dg-publish":true,"image":null,"permalink":"/Python/1. python Cơ bản/Python cơ bản/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-01-25T17:11:56.627+07:00","updated":"2024-01-29T14:11:53.674+07:00"}
---

**[[Homepage\|Quay Lại👈]]**

Source : 
Tags:  #python 

---

# Bài 1 Cài đặt python và pycham IDE

## Cài đặt python

### Lưu ý khi cài đặt -> chọn vào mục Add pytho 3.8 to Path


![](https://i.imgur.com/rjLaUo9.png)
### Cài đặt Pycharm

![](https://i.imgur.com/dV9BT8t.png)

# Bài 2 Comment code trong python

```ad-hint
# Tại sao cần comments- > để xem lại và dễ hiểu được các đoạn code
```
## Viết  comment bắt đầu bằng một dấu #


## hoặc nếu có nhiều dòng thì có thể bắt đầu và kết thúc bằng 3 dấu "
![](https://i.imgur.com/OxEpyOK.png)

# Bài 3 Khai báo biến cơ bản trong python
### Bước 1  Tạo một file mới:

Chọn file đã có sẵn-> chuột phải->python file


![](https://i.imgur.com/BCLBE72.png)
### Đặt tên file là Variable
---
![](https://i.imgur.com/zbP4bQf.png)
  TÊN BIẾN
age = 25
name = "Thanh"

print (age)========
print (name)

#### QUY TẮC ĐẶT TÊN BIẾN

- Có thể bắt đầu bằng dấu _
	Ví dụ _lastname ="Nguyen"
	
- có thể có chứa số
address1 = ""
address2 = ""

##### ==TÊN BIẾN KHÔNG HỢP LỆ TRONG PYTHON==
**Đây là những ví dụ về các biến không hợp lệ**
2age
my?age
my-age
my age

##### KHAI BÁO BIẾN NHANH CHÓNG TRONG PYTHON

age, name = 25, "Thanh"

HOẶC 

emp1, emp2, emp3 = 400

---
Ta có thể kiểm tra bằng lệnh print 

print(emp1)
print(emp2)
print(emp3)
---
# BÀI 4 Sử dụng input Prompt để lấy dữ liệu cơ bản
```ad-note
# ở đây mình sẽ viết một chương trình py mà chương trình này có thể tương tác được với người dùng, ví dụ như hỏi tên, hỏi tuổi và sẽ output ra một câu : tên tôi là... bao nhiêu tuổi.
```
Ta làm như sau
age = input("How old are you?")
name = input("What is your name?")

print(" I am " + name + ". I am " + age + " years old.")

---
==Sau đó chạy lệnh ( phím tắt : ALT SHIFT F10)==
 Dưới đây là hình ảnh minh họa:
![](https://i.imgur.com/GdOxiZr.png)


Cách 2:

==Ta sẽ có một biến thông báo==

message = " I am {}. I am {} years old."
print(measage.format(name, age))

![](https://i.imgur.com/5KSdues.png)

----
==VÍ DỤ KHÁC==

age = 18
name = "Thanh"

Nếu ta chạy lệnh :

message = " I am {}. I am {} years old."
print(measage.format(name, age))

Thì sẽ gây ra LỖI. 
Lý do là do age -> là số, không phải kiểu str.

Để kiểm tra kiểu dữ liệu ta có thể chạy lệnh như sau:

print(type(age)) 
pring(type(name))
---
age -> kiểu int
name-> kiểu str

---
==Để khắc phục lỗi ta sửa lại như sau==

print(" I am " + name + ". I am " + ==str(age)== + " years old.")

-> ta biến biến age thành dạng string để không bị lỗi khi ghép lệnh.
---
# Bài 5 Làm việc với Numbers trong Python



## ==Dữ liệu kiểu Integer==
a = 2
 b = 565656
 c = -5656562444
-> Số nguyên
-> kiểm tra kiểu dữ liệu của a ,b, c
print(a, b, c)
print(type(a)) -> Lệnh  Alt shift f10-> int

## ==Dữ liệu kiểu số, kiểu float==

x = 1.1
y = 4345.25

-print(type(x))-> float
```ad-note
### VÍ DỤ : GIỜ MÌNH MUỐN CHUYỂN TỪ KIỂU FLOAT SANG KIỂU INTERGER THÌ LÀM SAO?
x = int(x)
print(type(x))
- Khi chuyển từ kiểu float sang in thì nó chỉ lấy phần nguyên
```

Trường hợp chuyển từ int-> float thì làm thế nào?

b = float(b)
print(type(b))
## ==Dữ liệu kiểu Complex== : là số ảo -> hiện tại chúng ta sẽ chưa quan tâm đến kiểu số này.

ví dụ z = 5j
---
PHẦN BÀI TẬP
```ad-question
# viết một chương trình nhập vào cạnh của hình chữ nhật, trả lại cho người dùng diện tích, và chu vi hình chữ nhật
```

a = input("Chiều dài hình chữ nhật là?")
b = input("chiều rộng hình chữ nhật là?)

meassage = "Diện tích hình chữ nhật {}"
print(measage.format(a*b))
-> Chạy chương trình này ta bị ==LỖI==

==LÝ DO:   a và b trong công thức input trên là kiểu string -> ta cần chuyển sang kiểu float, vì kiểu nhập vào có thể là số nguyên hoặc float==
---
![](https://i.imgur.com/qLkVxb7.png)
---
# Bài 6 Làm việc với string trong python

str = "toi di hoc python"

## ==bien tat ca thanh chu hoa==

print(str.upper())
 -> Thu được kết quả : TOI DI HOC PYTHON
## ==biến tất cả thành chữ thường==

print(str.lower()) -> toi di hoc python


## Kiểm tra độ dài của chuỗi
 print(len(str))

## kiểm tra từng ký tự trong chuỗi

print(str[0]) -> chạy code -? trả về chữ t