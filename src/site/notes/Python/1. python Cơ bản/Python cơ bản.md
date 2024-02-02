---
{"aliases":null,"tags":null,"Related":null,"date":null,"URL":null,"Author":null,"dg-publish":true,"image":null,"TARGET DECK":"python2025","permalink":"/Python/1. python Cơ bản/Python cơ bản/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-01-25T17:11:56.627+07:00","updated":"2024-02-02T12:44:02.270+07:00"}
---

**[[Homepage\|Quay Lại👈]]**

Source : 
Tags:  #python 

# Bài 1 Cài đặt python và pycham IDE

## Cài đặt python

### Lưu ý khi cài đặt -> chọn vào mục Add pytho 3.8 to Path


![](https://i.imgur.com/rjLaUo9.png)
### Cài đặt Pycharm

![](https://i.imgur.com/dV9BT8t.png)

---
# Bài 2 Comment code trong python

```ad-hint
# Tại sao cần comments- > để xem lại và dễ hiểu được các đoạn code
```
## Viết  comment bắt đầu bằng một dấu #


## hoặc nếu có nhiều dòng thì có thể bắt đầu và kết thúc bằng 3 dấu "
![](https://i.imgur.com/OxEpyOK.png)

---
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
<!--ID: 1706852544435-->

print (name)

#### QUY TẮC ĐẶT TÊN BIẾN

- Có thể bắt đầu bằng dấu _
	Ví dụ _lastname ="Nguyen"
	
- có thể có chứa số
address1 = ""
address2 = ""

##### ==TÊN BIẾN KHÔNG HỢP LỆ TRONG PYTHON==
<!--ID: 1706852544441-->

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
<!--ID: 1706852544447-->

 Dưới đây là hình ảnh minh họa:
![](https://i.imgur.com/GdOxiZr.png)


Cách 2:

==Ta sẽ có một biến thông báo==
<!--ID: 1706852544454-->


message = " I am {}. I am {} years old."
print(measage.format(name, age))

![](https://i.imgur.com/5KSdues.png)

----
==VÍ DỤ KHÁC==
<!--ID: 1706852544460-->


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
<!--ID: 1706852544467-->


print(" I am " + name + ". I am " + ==str(age)== + " years old.")
<!--ID: 1706852544473-->


-> ta biến biến age thành dạng string để không bị lỗi khi ghép lệnh.
---
---
# Bài 5 Làm việc với Numbers trong Python



## ==Dữ liệu kiểu Integer==
<!--ID: 1706852544479-->

a = 2
 b = 565656
 c = -5656562444
-> Số nguyên
-> kiểm tra kiểu dữ liệu của a ,b, c
print(a, b, c)
print(type(a)) -> Lệnh  Alt shift f10-> int

## ==Dữ liệu kiểu số, kiểu float==
<!--ID: 1706852544486-->


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
<!--ID: 1706852544494-->


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
<!--ID: 1706852544501-->


==LÝ DO:   a và b trong công thức input trên là kiểu string -> ta cần chuyển sang kiểu float, vì kiểu nhập vào có thể là số nguyên hoặc float==
<!--ID: 1706852544507-->

---
![](https://i.imgur.com/qLkVxb7.png)
---
---
# Bài 6 Làm việc với string trong python

str = "toi di hoc python"

## ==bien tat ca thanh chu hoa==
<!--ID: 1706852544513-->


**print(str.upper())**
 -> Thu được kết quả : TOI DI HOC PYTHON
## ==biến tất cả thành chữ thường==
<!--ID: 1706852544520-->


**print(str.lower()) **-> toi di hoc python


## Kiểm tra độ dài của chuỗi
 **print(len(str))**

## kiểm tra từng ký tự trong chuỗi

**print(str[0])** -> chạy code -? trả về chữ t

0 là vị trí số 0.

print(str[0:3]) 

---
==number = "12"==
<!--ID: 1706852544527-->

 Kiểm tra xem số trên có phải là số không?
 
  print(number.isnumeric()) -> True

**Kiểm tra loại của number.**

print(type(number)) -> str
---
==Trường hợp ta thêm chữ sau số 12 như sau==
<!--ID: 1706852544534-->


number = "12A"

print(number.isnumeric()) -> False

mặc dù ta kiểm tra loại của number vẫn là str.

print(type(number)) -> str

---
==Ví dụ ta có chuỗi như sau, ta cần kiểm tra xem chuỗi có phải là viết hoa không==
<!--ID: 1706852544540-->


str = "HELLO"
print(str.isupper())  -> chạy lệnh TRUE

HOẶC print(str.islower())

---
==kiểm tra độ dài của str== 
<!--ID: 1706852544547-->

print(len(str))-> chạy (alt shift f10) ->10

---
# Bài 7 Làm việc với boolean trong python

Kiểu boolean là kiểu true hoặc false

ví dụ

print(4<3) -> False

print(4 == 4) -> true

---
# Bài 8 Làm việc với list trong python

## ==python list==
<!--ID: 1706852544554-->



- Sử dụng Terminal trong Pycharm
- Bây giờ ta đi khai báo biến :
fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
## ==Access item in list==
<!--ID: 1706852544561-->


```ad-note
# số thứ tự của một list bắt đầu từ vị trí thứ 0; có nghĩa là gì, ví dụ trên thì "táo"- là vị trí số 0
```

### ==Ví dụ chúng ta muốn gọi ra item ở vị trí số 0:==
<!--ID: 1706852544568-->


print(fruits[0]) ->tao
print(fruits[1]) -> chuoi
print(fruits[2]) -> cam
print(fruits[3]) -> mit

### ==Thử xem xem trong chuỗi có bao nhiêu thành viên==
<!--ID: 1706852544575-->


len(fruits) -> 7

```ad-question
# Làm thế nào để truy nhập được last item ( phần tử cuối cùng trong list)
```

==print(fruits[len(fruits)-1])== / nhưng bạn có thể sử dụng cách khác nhanh hơn được nói ở phần tiếp theo 
<!--ID: 1706852544582-->


## ==Access item in list negative indexing style, first item reverse, first item from right==
<!--ID: 1706852544588-->

fruits[-1]
fruits[-2]

## Access item in list range style [2:5] , [2:], [-4:-1]

![](https://i.imgur.com/FllgUVy.png)
  [2: 5]   : index >=2 and index <5 ; inclue 2, exclude 5
  ### ==Lấy từ item đầu tiên đến 5 [:5]==  -> chỉ gồm từ 0 cho đến phần tử số 4
<!--ID: 1706852544595-->

![](https://i.imgur.com/ovFq8Lb.png)

### ==Lấy từ item thứ 2 cho tới cuối [2:]==
<!--ID: 1706852544602-->

>>> fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
>>> fruits[2:]

![](https://i.imgur.com/xdSTMuz.png)
### ==ví dụ [-4:-1] : Sẽ bao gỗm -4 và không gồm thành phần -1==
<!--ID: 1706852544609-->


ví dụ trong chuỗi fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]

thì cà chua = -1
kiwi = -2
dua hau = -3
mit =-4

fruits[-4,-1]-> kết quả trả về sẽ gồm : mit, dua hay, kiwi và ==không bao gồm cà chua==
<!--ID: 1706852544615-->

## ==Change value of a item in a list==
<!--ID: 1706852544621-->


 fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
- Ta muốn chuyển "tao" thành "Tao"
fruits[0] = "Tao"
 
sau đó gọi lại fruits thì ta thu được kết quả

fruits = ["Tao", "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua"]
## ==loop through a list : Vòng lặp trong python==
<!--ID: 1706852544628-->


**for fruit in fruits:**
Sau đó ta in ra để kiểm tra bằng lệnh print như sau:

print(fruit)


![](https://i.imgur.com/2evIjiR.png)


## check if item in list
: để kiểm tra xem một loại hoa quả có nằm trong chuỗi không
![](https://i.imgur.com/3ihZaaj.png)
## ==list length==
<!--ID: 1706852544634-->


len(fruits)

## ==Add items to end : Thêm một item vào list==
<!--ID: 1706852544641-->

fruits.append("Sau rieng")
![](https://i.imgur.com/Fq16AXm.png)
## ==Insert item vs add item==.
<!--ID: 1706852544648-->


Ví dụ mình muốn insert quả "dua chuot" vào vị trí số 0 thì làm như sau:

fruits.insert(0, "dua chuot")
![](https://i.imgur.com/07zcV4o.png)

## Remove item -with remove()

![](https://i.imgur.com/WzNCPbu.png)

---
## ==Remove item -with pop()== 
<!--ID: 1706852544655-->

Bỏ đi một đối tượng ngoài cùng trong một list làm thế nào? #flashcard
fruits.pop()
---
-> với hàm .pop nếu không đưa ra  vị trí thì nó sẽ bỏ đi phần tử cuối cùng.
Ví dụ ta có chuỗi như sau:
![](https://i.imgur.com/2yIWxN3.png)





---
## ==Remove item -with del== #flashcard 
<!--ID: 1706852544662-->

del fruits[0]
---
Bỏ các phần tử ra khỏi một giỏ hàng #flashcard
## ==Empty a list - clear()==
<!--ID: 1706782038860-->


---
xóa toàn bộ giỏ hàng fruits đi #flashcard 
del fruits
---
## ==Copy một list==  #flashcard 
<!--ID: 1706852544669-->

list2 = fruits.copy()
---
## ==Join 2 list== 
<!--ID: 1706852544675-->

Làm thế nào để joint được 2 list lại với nhau? #flashcard 
![](https://i.imgur.com/GIiTTHl.png)
---
## Reverse order of a list : 
Cách đảo lại thứ tự trong một list? #flashcard 
fruits.reverse()
![](https://i.imgur.com/v1xmUtG.png)
---
## Sort a list
Làm thế nào để sort một list? #flashcard
**fruits.sort()**
![](https://i.imgur.com/XJ08YvL.png)
---


# Bài 9- Làm việc với các toán tử trong python 

## Arithmetic operators : +, - , * , / ,% , ** **, //
![](https://i.imgur.com/0stBizV.png)
![](https://i.imgur.com/eLRG5XU.png)
---
## Assigment operators:  =, +=, -=

==x += 2 Có nghĩa là gì?== :: Tăng X lên 2 đơn vị
<!--ID: 1706852544428-->

là lấy x cộng thêm 2 và trả về kết quả.
==ví dụ:== 
x = 5
x +=2
>>> 7

x -= 2 Có nghĩa gì? ::  # giảm x đi 2 đơn vị

là lấy giá trị đó trừ đi và trả về kết quả.
==Ví dụ==
x = 5
x -=2 
>>> 3
