Kristina Markoska 223077


2. Control Flow Graph
![Untitled Diagram drawio (3)](https://github.com/kristinamarkoska/SI_2024_lab2_223077/assets/165588196/7bb5d8e7-26df-4d1b-a75a-dd27bc66c169)




3. Цикломатската комплексност

   
   Цикломатската комплексност на овој код е 10, истата ја добив преку формулата P+1, каде што P е бројот на предикатни јазли. Во случајoв P=9, па цикломатската комплексност изнесува 10.

4. Тест случаи според критериумот Every branch
   
    1.  []
    2. Item("Stolica", "V3",350,10.0), payment = 200
    3. Item("Kebe", "75",450,5.0), payment = 2000
    4. Item("Penkalo", "",100,4.0), payment = 50
    5. Item("Dnevnik", "07",320,0.0), payment = 300
    6. Item("", "0.5",420,7.5), payment = 80
 ![image](https://github.com/kristinamarkoska/SI_2024_lab2_223077/assets/165588196/b20845f4-465d-4761-948c-9b0ff0d6029c)

Тест случаи според Multiple Condition критериумот

if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0')

Можни услови:

F && X && X -> item.getPrice() <= 300, item.getDiscount() = anything, item.getBarcode().charAt(0) = anything

T && F && X -> item.getPrice() >= 300, item.getDiscount() <= 0, item.getBarcode().chatAt(0) = anything

T && T && T -> item.getPrice() >= 300, item.getDiscount() > 0, item.getBarcode().charAt(0) == '0'
