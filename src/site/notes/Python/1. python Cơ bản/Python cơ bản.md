---
{"aliases":null,"tags":null,"Related":null,"date":null,"URL":null,"Author":null,"dg-publish":true,"image":null,"TARGET DECK":"python2025","permalink":"/Python/1. python Cơ bản/Python cơ bản/","dgPassFrontmatter":true,"noteIcon":"2","created":"2024-02-29T09:58:30.011+07:00","updated":"2024-02-28T15:07:10.000+07:00"}
---

**[[Homepage\|Quay Lại👈]]**

Source : 
Tags: #python 

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
## Viết comment bắt đầu bằng một dấu #


## hoặc nếu có nhiều dòng thì có thể bắt đầu và kết thúc bằng 3 dấu "
![](https://i.imgur.com/OxEpyOK.png)

---
# Bài 3 Khai báo biến cơ bản trong python
### Bước 1 Tạo một file mới:

Chọn file đã có sẵn-> chuột phải->python file


![](https://i.imgur.com/BCLBE72.png)
### Đặt tên file là Variable
---
![](https://i.imgur.com/zbP4bQf.png)
  TÊN BIẾN
age = 25
name = "Thanh"

print (age)
print (name)

#### QUY TẮC ĐẶT TÊN BIẾN

- Có thể bắt đầu bằng dấu _
	Ví dụ _lastname ="Nguyen"
	
- có thể có chứa số
address1 = ""
address2 = ""

##### <span style="background:#40a9ff">TÊN BIẾN KHÔNG HỢP LỆ TRONG PYTHON</span>

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
Sau đó chạy lệnh ( phím tắt : ALT SHIFT F10)

 Dưới đây là hình ảnh minh họa:
![](https://i.imgur.com/GdOxiZr.png)


Cách 2:

Ta sẽ có một biến thông báo



message = " I am {}. I am {} years old."
print(measage.format(name, age))

![](https://i.imgur.com/5KSdues.png)

----
VÍ DỤ KHÁC

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
<span style="background:#ff4d4f">Để khắc phục lỗi ta sửa lại như sau</span>



print(" I am " + name + ". I am " + str(age) + " years old.")



-> ta biến biến age thành dạng string để không bị lỗi khi ghép lệnh.
---
---
# Bài 5 Làm việc với Numbers trong Python



##<span style="background:#ff4d4f"> Dữ liệu kiểu Integer</span>
a = 2
 b = 565656
 c = -5656562444
-> Số nguyên
-> kiểm tra kiểu dữ liệu của a ,b, c
print(a, b, c)
print(type(a)) -> Lệnh Alt shift f10-> int

## <span style="background:#40a9ff">Dữ liệu kiểu số, kiểu float</span>

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
## Dữ liệu kiểu Complex : là số ảo -> hiện tại chúng ta sẽ chưa quan tâm đến kiểu số này.

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
-> Chạy chương trình này ta bị LỖI

LÝ DO: a và b trong công thức input trên là kiểu string -> ta cần chuyển sang kiểu float, vì kiểu nhập vào có thể là số nguyên hoặc float
---
![](https://i.imgur.com/qLkVxb7.png)
---
---
# Bài 6 Làm việc với string trong python

str = "toi di hoc python"

## <span style="background:#40a9ff">bien tat ca thanh chu hoa</span>
**print(str.upper())**
 -> Thu được kết quả : TOI DI HOC PYTHON
## <span style="background:#40a9ff">biến tất cả thành chữ thường</span>
**print(str.lower()) **-> toi di hoc python
## Kiểm tra độ dài của chuỗi
 **print(len(str))**
## kiểm tra từng ký tự trong chuỗi
**print(str[0])** -> chạy code -? trả về chữ t
0 là vị trí số 0.
print(str[0:3]) 
---
number = "12"

 Kiểm tra xem số trên có phải là số không?
 
  print(number.isnumeric()) -> True

**Kiểm tra loại của number.**

print(type(number)) -> str
---
Trường hợp ta thêm chữ sau số 12 như sau

number = "12A"

print(number.isnumeric()) -> False

mặc dù ta kiểm tra loại của number vẫn là str.

print(type(number)) -> str

---
Ví dụ ta có chuỗi như sau, ta cần kiểm tra xem chuỗi có phải là viết hoa không
str = "HELLO"
print(str.isupper()) -> chạy lệnh TRUE

HOẶC print(str.islower())

---
kiểm tra độ dài của str
print(len(str))-> chạy (alt shift f10) ->10

---
# Bài 7 Làm việc với boolean trong python

Kiểu boolean là kiểu true hoặc false

ví dụ

print(4<3) -> False

print(4 == 4) -> true

---
# Bài 8 Làm việc với list trong python

##<span style="background:#40a9ff"> python list</span>
- Sử dụng Terminal trong Pycharm
- Bây giờ ta đi khai báo biến :
fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
## <span style="background:#40a9ff">Access item in list</span>

```ad-note
# số thứ tự của một list bắt đầu từ vị trí thứ 0; có nghĩa là gì, ví dụ trên thì "táo"- là vị trí số 0
```

### <span style="background:#40a9ff">Ví dụ chúng ta muốn gọi ra item ở vị trí số 0:</span>
print(fruits[0]) ->tao
print(fruits[1]) -> chuoi
print(fruits[2]) -> cam
print(fruits[3]) -> mit

### <span style="background:#40a9ff">Thử xem xem trong chuỗi có bao nhiêu thành viên</span>

len(fruits) -> 7

```ad-question
# Làm thế nào để truy nhập được last item ( phần tử cuối cùng trong list)
```

print(fruits[len(fruits)-1]) / nhưng bạn có thể sử dụng cách khác nhanh hơn được nói ở phần tiếp theo 

## Access item in list negative indexing style, first item reverse, first item from right

fruits[-1]
fruits[-2]

## Access item in list range style [2:5] , [2:], [-4:-1]

![](https://i.imgur.com/FllgUVy.png)
  [2: 5] : index >=2 and index <5 ; inclue 2, exclude 5
  ### Lấy từ item đầu tiên đến 5 [:5] -> chỉ gồm từ 0 cho đến phần tử số 4
![](https://i.imgur.com/ovFq8Lb.png)

### Lấy từ item thứ 2 cho tới cuối [2:]

>>> fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
>>> fruits[2:]

![](https://i.imgur.com/xdSTMuz.png)
### ví dụ [-4:-1] : Sẽ bao gỗm -4 và không gồm thành phần -1

ví dụ trong chuỗi fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
thì cà chua = -1
kiwi = -2
dua hau = -3
mit =-4

fruits[-4,-1]-> kết quả trả về sẽ gồm : mit, dua hay, kiwi và <span style="background:#40a9ff">không bao gồm cà chua</span>

## Change value of a item in a list
 fruits = ["tao" , "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua" ]
- Ta muốn chuyển "tao" thành "Tao"
fruits[0] = "Tao"
 
sau đó gọi lại fruits thì ta thu được kết quả

fruits = ["Tao", "chuoi", "cam", "mit", "dua hau", "kiwi", "ca chua"]
## loop through a list : Vòng lặp trong python

**for fruit in fruits:**
Sau đó ta in ra để kiểm tra bằng lệnh print như sau:
print(fruit)
![](https://i.imgur.com/2evIjiR.png)
## check if item in list
: để kiểm tra xem một loại hoa quả có nằm trong chuỗi không
![](https://i.imgur.com/3ihZaaj.png)
## ==list length==

len(fruits)

## ==Add items to end : Thêm một item vào list==
fruits.append("Sau rieng")
![](https://i.imgur.com/Fq16AXm.png)
## ==Insert item vs add item==.

Ví dụ mình muốn insert quả "dua chuot" vào vị trí số 0 thì làm như sau:
fruits.insert(0, "dua chuot")
![](https://i.imgur.com/07zcV4o.png)

## Remove item -with remove()
![](https://i.imgur.com/WzNCPbu.png)
---
## ==Remove item -with pop()== 

Bỏ đi một đối tượng ngoài cùng trong một list làm thế nào? 
fruits.pop()
---
-> với hàm .pop nếu không đưa ra vị trí thì nó sẽ bỏ đi phần tử cuối cùng.
Ví dụ ta có chuỗi như sau:
![](https://i.imgur.com/2yIWxN3.png)

---
## ==Remove item -with del== 

del fruits[0]
---
Bỏ các phần tử ra khỏi một giỏ hàng 
## ==Empty a list - clear()==

---
xóa toàn bộ giỏ hàng fruits đi  
del fruits
---
## ==Copy một list==   

list2 = fruits.copy()
---
## ==Join 2 list== 


Làm thế nào để joint được 2 list lại với nhau? 
![](https://i.imgur.com/GIiTTHl.png)
---
## Reverse order of a list : 
Cách đảo lại thứ tự trong một list? 
fruits.reverse()
![](https://i.imgur.com/v1xmUtG.png)
---
## Sort a list
Làm thế nào để sort một list? 
**fruits.sort()**
![](https://i.imgur.com/XJ08YvL.png)
---


# Bài 9- Làm việc với các toán tử trong python 

## Arithmetic operators : +, - , * , / ,% , ** **, //
![](https://i.imgur.com/0stBizV.png)
![](https://i.imgur.com/eLRG5XU.png)
---
## Assigment operators: =, +=, -=

### ==x += 2 Có nghĩa là gì?== :: Tăng X lên 2<span style="background:#ff4d4f"> đơn vị</span>
<!--ID: 1709107630602-->


là lấy x cộng thêm 2 và trả về kết quả.
==ví dụ:== 
x = 5
x +=2
>>> 7

### x -= 2 Có nghĩa gì? :: # giảm x đi 2 đơn vị
<!--ID: 1709107630608-->


là lấy giá trị đó trừ đi và trả về kết quả.
==Ví dụ==
x = 5
x -=2 
Kết quả trả về: 3
### x *=2 Có nghĩa là gì ? ::
 nghĩa là 2 lần x ( nhân với 2)
### x /=2 Có nghĩa là gì? ::
 nghĩa là x chia cho 2
### x %=2 nghĩa là gì ? ::
Nghĩa là lấy x chia cho 2 và<span style="color:#000000"> lấy phần dư</span>
 ![](https://i.imgur.com/HGy4dfe.png)

## Comparison operators:

ví dụ  1 == 1 ::
Kết quả trả về là true
![](https://i.imgur.com/G7ZJPNa.png)

<span style="background:#ff4d4f">1 !=1</span> :: Có phải 1 khác một hay không -> trả về kết quả là False
<!--ID: 1706865579528-->

kết quả trả về là False

![](https://i.imgur.com/Bey99kF.png)
1 != 2 :: kết quả trả về là True
<!--ID: 1706865579540-->


1 > 2 :: Kết quả trả về là False 
<!--ID: 1706865579547-->


1 < 2 :: Kết quả là True
<!--ID: 1706865579553-->


1<= 2 :: Kết quả trả về là True
![](https://i.imgur.com/i4jz5Du.png)
<!--ID: 1706865579560-->


2 >=2 :: True
2 <=2 :: True 
<!--ID: 1706865579567-->
<span style="background:#40a9ff">## Logical operators : and, or, not </span>

True and True :: Kết quả True 
<!--ID: 1709107630615-->


True or False ::  Kết quả True
<!--ID: 1709107630621-->


False or True :: Kết quả True 
<!--ID: 1709107630628-->

False and True :: Kết quả False 
<!--ID: 1709107630634-->

True and False :: Kết quả False 
<!--ID: 1709107630641-->


### not sẽ biến True thành False và ngược lại 


not True :: Kết quả là False 
<!--ID: 1709107630648-->

not False :: Kết quả là True 
<span style="background:#40a9ff">## Membership operators :  in, not in  </span>
![](https://i.imgur.com/IcXRQZc.png)
<!--ID: 1709107630654-->


---

# Bài 10 Làm việc với Tupe trong python </span></span>

## Ta có một list như sau 

![](https://i.imgur.com/o92xNKa.png)
 ### Ta có một Tuple như sau:
![](https://i.imgur.com/DvsCbPD.png)
### Ta thử truy  nhập vào các phần tử trong chuỗi Tuple 
![](https://i.imgur.com/NbTWMdh.png)
### Sự khác nhau khi ta truy nhập vào chuỗi và Tuple 

![](https://i.imgur.com/AvPgPDj.png)
### Thử thay đổi một thành phần trong Tuple 
![](https://i.imgur.com/eYdMMjc.png)
<span style="background:#ff4d4f">## Workaround</span>
 x = list(fruits_tuple)  # Ta đặt một
 x[0] = "TAO"  # Đổi cái thành phần đầu tiên thành TAO
 fruits.tuple = tuple(x) # Định nghĩa lại tupe 
 
![](https://i.imgur.com/iPjJ8mJ.png)
<span style="background:#ff4d4f">### Vì là tupe không cho thay đổi nên ta WORKAROUND </span>

<span style="background:#40a9ff">chuyển tuple -> list ; khi đó ta đối thành phần trong list -> Rồi lại chuyển list đó thành tuple.</span>

![](https://i.imgur.com/dvAPGrM.png)
# Bài 11 Làm việc với Set trong Python </span>
## set in python : unordered and unindexed, curly brackets 

![](https://i.imgur.com/dD2aMd6.png)
![](https://i.imgur.com/TLPg29e.png)
---
![](https://i.imgur.com/SBnHsxV.png)
![](https://i.imgur.com/N7dwaPZ.png)
![](https://i.imgur.com/IGmbLMI.png)


<span style="background:#40a9ff">### Remove một đối tượng ở trong set</span>

![](https://i.imgur.com/OpMiWko.png)
### Ngoài cách sử dụng remove thì chúng ta còn một cách nữa là dùng <span style="background:#ff4d4f">DISCARD</span>  để loại một phần tử ra khỏi set

![](https://i.imgur.com/TS8mXiy.png)


```ad-question
Vậy thì REMOVE và discard khác nhau ở chỗ nào ?
```

![](https://i.imgur.com/GthP3r5.png)

![](https://i.imgur.com/KrhU3qi.png)


<span style="background:#40a9ff">## Nối 2 set </span>

>>> set1 = {"a","b","c"}                                              
>>> set2 = {"d","e"}
>>> set1.<span style="color:#000000"><span style="color:#000000">union</span></span>(set2)
{'b', 'd', 'a', 'e', 'c'}


![](https://i.imgur.com/X8vuzTS.png)


```ad-note
Giẳ sử ta có set3 ={1,2,3,a,b,c}

Bây giờ ta Union (ghép ) với set4 = {2,3,4} -> Tức là có giá trị: 2,3 trùng nhau thì khi ghép vào chúng sẽ không add trùng nữa. Ta sẽ có kết quả 
set5={1,2,3,4,a,b,c}

Dưới đây là hình minh họa:
![](https://i.imgur.com/iUuTPb3.png)

```

# Bài 12 Làm việc với dictation trong python
## Python dictionary: unordered, changeable and indexed:

kiểu dữ liệu dictionnayry được khai báo như sau 


<span style="background:#9254de">Ten_biến = { "key" : "value"} </span>
---

```python 
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"
		  ,"year":2019}
print(type(laptop))
print(laptop)
```
## Access dictionary item

```python  
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019}    
print(laptop["brand"])
print(laptop["model"])
```
CÁCH 2 : DÙNG <span style="background:#ff4d4f">GET</span>


```python  
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019} 
print(laptop.get("brand"))
print(laptop.get("year"))
# laptop.get("year") = 2020 , không hỗ trợ đổi năm). Nếu muốn đổi phải làm như sau:
# laptop["year"] = 2020
print(laptop)

```
![](https://i.imgur.com/LBMfdTn.png)


### Print key, value of laptop dictionary
```python
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019} 
for x in laptop:
 print(x, laptop[x])
```
<span style="background:#40a9ff">KẾT QUẢ :</span>

![](https://i.imgur.com/EnerqL3.png)

![](https://i.imgur.com/s6ixe0K.png)


#### <span style="background:#40a9ff">Print all values of laptop dictionary</span>
```python
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year": 2019} 
# print(laptop.get("brand"))
# print(laptop.get("year"))
# laptop.get("year") = 2020 , không hỗ trợ đổi năm). Nếu muốn đổi phải làm như sau:
# laptop["year"] = 2020
# print(laptop)
for x in laptop.values():
 print(x)
```

kết quả thu được :
![](https://i.imgur.com/tgPrMw8.png)

## <span style="background:#40a9ff">CHECK IF KEY EXISTS IN DICTIONARY</span>
```python
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019} 
print("brand" in laptop)

```

![](https://i.imgur.com/b9Ym4Tz.png)
## <span style="background:#40a9ff">Add key, value pair</span>
```python
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019} 
laptop["color"] = "black"
print(laptop)

```
### Kết quả :![](https://i.imgur.com/leySj1E.png)

## <span style="background:#40a9ff">Bỏ- Revmove value</span>
```python
laptop = {"brand": "Lenovo","model":"Thinkpad X1 6"  ,"year":2019, "color": "Black"} 
laptop.pop("color")
print(laptop)

```
### Kết quả:
![](https://i.imgur.com/vDFv4FJ.png)
## Copy một dictionary
dict2 = dict(laptop)

## nested dictionary
```python
ibm = {
	"model1": {"name": "Think pad X1", "screensize": 14},
	"modell2": {"name": "Think pad X270", "screensize": 12.5}

}
```
### Access vào name của model1 ?

```python
ibm = {
 "model1": {"name": "Think pad X1", "screensize": 14}, 
"model2": {"name": "Think pad X270", "screensize": 12.5}}

print(ibm["model1"]["name"])
```

![](https://i.imgur.com/6QrVUJo.png)
---
# Bài 13 Câu lệnh rẽ nhánh If  ELIF ELSE trong python

```ad-info
Ở bài này mình sẽ kiểm tra độ dài một chuỗi. sau đó nếu quá ngắn/quá dài thì sẽ trả về một thông báo ( if then else)
```
## kiểm tra độ dài một chuỗi
```python
input = input("Hay nhap so tuoi cua ban") # trường hợp này khi nhập vào thì số tuổi nhập vào là một string. Ta cần chuyển sang dạng interger để kiểm tra nên có câu lệnh sau đây  
age = int(input)  
if age < 16:  
    print("Ban khong du tuoi de tham gia chuong trinh nay")

```


```ad-info
Chúng ta viết một chương trình nhập vào một con số, và kiểm tra số đó là số chẵn hay số lẻ.
```

![](https://i.imgur.com/4qibP7z.png)

```ad-info
viết một chương trình kiểm tra tam giác đều, cân thường
<span style="color:#000000">tam giác đều thì a = b =c 
tam giác cân thì a =b , b=c, a=c
tam giác thường thì a,b,c sẽ khác nhau</span>
```

```python
a = float(input("nhap canh a\n"))  
b = float(input("nhap canh b\n"))  
c = float(input("nhap canh c\n"))  
if a == b and b == c and a ==c:  
  
    print("day la tam giac deu")  
elif a !=b and b != c and a != c:  
    print("day la mot tam giac thuong")  
else:  
    print("day la mot tam giac can")
```

Kết quả là :

![](https://i.imgur.com/Q6QF5TQ.png)

Nhưng bài tập trên vẫn chưa đúng. vì điều kiện để có một tam giác phải thêm điều kiện 
a + b >c 
a+ c > b
b+c > a

Thêm điều kiện trên như nào được nhỉ?



## Bài tập 1: 
### In số lớn hơn : cho a = 4, b = 6, viết câu lệnh IF để in ra số lớn hơn
mình tự viết - haha sai luôn rồi
```python
a = 4
b = 6
if a > b
	print(a)
Else:
	print(b)
```

Đúng ở đây.

```python
a = 4
b = 6
if a > b
	print("day la so lon hon: " + str(a))
Else:
	print("day la so lon hon: " + str(b))
```
vì a là một sô interger thì ta phải chuyển nó sang dạng str đã

![](https://i.imgur.com/zWsg6H9.png)
## Bài tập 2: 
### Viết chương trình cho phép người dùng nhập vào chiều dài 2 cạnh của hình chữ nhật . In ra thông báo nếu là hình vuông hay hình chữ nhật và tính diện tích của hình.

<span style="background:#ff4d4f">Đây là bài Hà tự làm</span>

```python
chieu_dai = input(float("Nhap vao chieu dai hinh chu nhat\n"))
chieu_rong = input(float("Nhap vao chieu rong hinh chu nhat\n"))
dien_tich = chieu_dai ** chieu_rong
if chieu_dai == chieu_rong:
	print("Day la hinh vuong có dien tich là " + str(dien_tich))
else: 
	print("Day la hinh chu nhat có dien tich là " + str(dien_tich))
```

há há, sai rồi.
<span style="background:#40a9ff">Sử lại thôi </span>

```python
chieu_dai = float(input("Nhap vao chieu dai hinh chu nhat\n"))
chieu_rong = float(input("Nhap vao chieu rong hinh chu nhat\n"))
dien_tich = chieu_dai * chieu_rong
if chieu_dai == chieu_rong:
	print("Day la hinh vuong có dien tich là " + str(dien_tich))
else: 
	print("Day la hinh chu nhat có dien tich là " + str(dien_tich))
```

# Bài 14 Vòng Lặp For trong python 

```ad-info
For trong python dùng để lặp qua nhiều kiểu dữ liệu : list, tupe, set, dictionary, string..
```

```python
fruits = ["chuoi" , "tao", "le" ]
for fruit in fruits:
	print(fruit)
message = "HELLO"
for c in message:
	print(c)
```
<span style="background:#ff4d4f">KẾT QUẢ ĐÂY:</span>
![](https://i.imgur.com/BWCOX9h.png)

```ad-info
Sẽ lặp một chuỗi, và kiểm tra từng ký tự , nếu chữ cái bằng chữ l thì ta sẽ dừng lại thì làm thế nào?
```

```python
message = "HELLO"
for c in message:
	if c == "L":
		print("Da tim thay")
		break
```

Chạy code và kết quả là:
![](https://i.imgur.com/81dTyMo.png)

Ngược với break- ở phần trên nếu vẫn muốn tiếp tục hàm for thì ta làm thế nào 

```ad-note ví dụ ta muốn in 3 lần chữ HELLO
THÌ LÀM THẾ NÀO?
```

```python
for x in range(3):
	print("Hello")
```
<span style="background:#ff4d4f"> range(3) : được hiểu lầ 0,1,2</span>
Ta có thể in thêm số thứ tự của những thành phần bên trên.

```python
for x in range (3):
	print("Hello " + str(x))
```

```python
for x in range(10,20):  # bao gồm 10 đến 19, không bao gồm 20.
	print(x)
```

<span style="background:#ff4d4f">IN RA SỐ LẺ TỪ 1 ĐẾN 20 THÌ LÀM THẾ NÀO?</span>
	in số lẻ từ 1-20, step là 2
```python
for x in range(1,20,2):
	print(x)
```


```python
fruits = ["chuoi" , "tao", "le" ]
prices = [2, 3, 4]
for fruit in fruits:
	for price in prices:
		print(fruit, price)
```

chạy code thu được kết quả:
giải thích kết quả một chút :
	- Ở vòng lặp đầu tiên, chuối đi vào vòng lặp thì nó sẽ in ra với 3 kết quả với price.
	
![](https://i.imgur.com/oT70xy9.png)


Trong trường hợp mà chúng ta muốn : giả sử gặp một đối tượng nào đó nó sẽ nhảy ra khỏi vòng lặp thì làm sao.

```python
for i in [1,2,3,4]:
	pass
```

# Bài 15 Vòng lặp White Loop trong Python 
```python
i = 1
while i < 6:
	print(i)
	i  += 1
```
 Giải thích : khi i bằng i thì so sánh với 6. Nếu nhỏ hơn thì in ra i. rồi tiếp tục cộng thêm 1 và tiếp tục so sánh.


Ở ví dụ trên thì đến số 5 là điều kiện trên kết thúc. Nhưng nếu ở ví dụ khác mà số 6 kia lớn, thì nó sẽ rơi vaofa một vòng lặp vô tận. VẬY PHẢI NGẮT HOẶC DỪNG VÒNG LẶP TRÊN BẰNG CÁCH NÀO?. thêm vào <span style="background:#ff4d4f">break </span>

![](https://i.imgur.com/K7ZTnRq.png)
 đến khi i = 3 thì sẽ không lặp nữa. -> Tức là hàm này luôn luôn đùng- thì vòng lặp này không dừng được-> vậy phải tăng i lên.

```python
i = 1
while i < 6:
	if i == 3:
		 break 
	i +=1
	print(i)
```

kết quả sau khi chạy;

![](https://i.imgur.com/3VLtLBS.png)

- Khi kết thúc vòng lặp thì ta chạy thêm một đoạn code nữa 
ví dụ như sau

```python
i = 1
while i < 6:
	print(i)
	i +=1
else:
	print("kết thúc vòng lặp")
```

kết quả :![](https://i.imgur.com/UXmprN8.png)


# Bài  16 Làm việc với function trong python 

Nhắc lại phần tên biến.

Tên biến hợp lệ
Tên biến không hợp lệ:
	- bắt đầu bằng số, 
	- chứa ký tự đặc biệt.
	- chứa dấu gạch ngang
	- chứa khoảng trắng.
![](https://i.imgur.com/ot4YUbi.png)


```ad-info
# viết chương trình function để đổi từ inch sang cm
```

![](https://i.imgur.com/31QsxDH.png)

```python
def convert_cm(inches = 0, feet = 0):  # keyword argerguments
	inches_to_cm = 2.54 * inches
	feet_to_cm = 2.54 * 12 * feet
	return feet_to_cm + inches_to_cm
print(convert_cm(inches = 1))
print(convert_cm(feet = 1))
print(convert_cm(inches=1, feet=1))
	
```
![](https://i.imgur.com/EvTHTsm.png)



```ad-info
# viết chương trình function để tính diện tích hình tròn bán kính r
```

```python
def dien_tich_hinh_tron(r): # r is required argument
	s = 3.14 * r ** 2
	return s
dien_tich = dien_tich_hinh_tron(10)
print(dien_tich)
```

![](https://i.imgur.com/DHNxrhB.png)

# Bài 17  Luyện tập vòng lặp For và câu điều kiện IF

```ad-todo
# ❓ Lập danh sách những số chia hết cho 7 nhưng không chia hết cho 5
# ❓Trong khoảng 2000 đến 3200 ( bao gồm cả 2000 và 3200)
```

```python
result = []
for i in range(2000, 3201):
	if (i % 7 == 0) and (i % 5 != 0):
		result.append(i)
print(result)
```

KẾT QUẢ THU ĐƯỢC:

![](https://i.imgur.com/QAAKkdi.png)
