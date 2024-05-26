# Armend Selmani 175004
# Control Flow Graph : 
![242310994-a64e1995-850d-48fc-9549-b8a844918171](https://github.com/armendselmanii/SI_2024_lab2_175004/assets/139174554/169da54a-0967-44fd-a3c0-fee17dc8c8c0)
# Цикломатска Комплексност:
Цикломатската комплексност на овој код е 11, истата ја добив преку формулата V (G) = E - N + 2, каде што E е бројот на ребра а N e бројот на јазли. Во случајoв Е=39, N=30 па цикломатската комплексност изнесува 11.
# Тест случаи според критериумот Every branch
TestCase1 : user = null; AllUsers=null;
Да влезе во првиот IF и да фрли excepction
TestCase2: user(username=null;password =1234fin!.; email=finki@ukim.mk) ; AllUsers = (username=null; password=1234fin!.; email=finki@ukim.mk)
Различен username, passwordot да содржи специјални знаци, ист мејл.
TestCase3: user(username=Armend; password = armend; email = finki@ukim.mk) ; AllUsers = (username=Armend; password= armend; email=finkiukim)
Passwordot да има помалце од 8 карактери и различен меил ист username.
TestCase4: user(username=Armend; password=12345678910112341; email: armend123) ; AllUsers = (username=Armend; password=1241432131; email=bilosto)
Мејлот да не содржи @ i . i password без специјален знак
TestCase5: user(username=Armend; password= finki ukim; email: finki@ukim.mk) ; AllUsers= (username=Armend; password= finki ukim; email= finki@ukim.mk)
Пасвордот да содржи празно место.
Со овие test caseovi се исполнува Every Branch критериумот.

![242367337-69e1fd7f-db22-4cbd-ad02-aada6b77d2e9](https://github.com/armendselmanii/SI_2024_lab2_175004/assets/139174554/3b63c789-b31c-41d4-a090-d1db0352809f)
# Тест случаи според критериумот Multiple Condition
Според овој критериум за условот if (user==null || user.getPassword()==null || user.getEmail()==null) имаме 4 можни сценарија
T X X
F T X
F F T
F F F
TestCase1: User == null
TestCase2: User("Armend", null, "bilosto")
TestCase3: User("Armend", "password", null)
TestCase4: User("Armend", "password", "bilosto")
