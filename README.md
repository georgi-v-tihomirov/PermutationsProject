# PermutationsProject
## Introduction  
Едно от фундаменталните понятия в математиката е функция. В дискретната математика и в часност в компютърните науки се нуждаем от разглеждането на понятието функция на теоретико-множествено ниво. Ние използваме функции при дефинирането на дискретни структури като редици и стрингове, при оценяване времевата сложност на дадена програма и съоветно ефективността на даден алгоритъм. Алгоритмите за сортиране например са пряко свързани с биекциите (взаимно-еднозначни съответствия) върху крайно множество елементи - така наречените пермутации. Пермутациите на n-елемента с дефинирана операция композиция (◦) образуват дискретна структура, наречена пермутационна група, която има редица интересни свойства.

![alt text](https://raw.githubusercontent.com/KingGVT/PermutationsProject/master/PermutationsImage1.PNG?token=AYwFVc5uqgCQAjIHBbgNPTW0JtegdjlGks5cYvdlwA%3D%3D)  

### Постановка
Изготвянето на проекта предполага реализация на C++ на редица функции, свързани с понятието пермутация.


#### Пермутации
Функция от множеството A в множеството B наричаме съответствие f, което съпоставя на всеки елемент a ∈ A единствен елемент b ∈ B. Елемента b наричаме образ на a и означаваме с f(a), а елемента a наричаме първообраз на b. Функцията означаваме с f : A → B, като множеството A наричаме дефиниционна област.
###### Задача 1. 
Да се дефинира двумерен динамичен масив, който има размерност 2 реда и n стълба, с помощта на който ще представяме функция върху множество с n елемента.
###### Задача 2. 
Да се дефинира функция на С++ за запълване на двумерен масив по зададено от потребителя множество от стойности на функция.
Една функция f : A → B наричаме инективна или инекция, ако тя приема различни стойности в различни точки от дефиниционната си област, т.е. ако x, y ∈ A и x 6= y, то f(x) 6= f(y).
###### Задача 3. 
Да се дефинира функция на С++, която проверява дали записана в масив функция е инекция.
Една функция f : A → B наричаме сюрективна или сюрекция, ако всеки елемент от множеството B има първообраз.
###### Задача 4. 
Да се дефинира функция на С++, която проверява дали записана в масив функция е сюрекция.
Една функция f : A → B наричаме биективна или биекция, ако тя е едновременно инекция и сюрекция. Казваме още, че f е взаимно еднозначно съответствие между A и B. Ако A е крайно множество, то |A| = |B| и f наричаме
пермутация.
###### Задача 5. 
Да се дефинира функция на С++, която проверява дали записана в масив функция е пермутация.
Нека n ∈ N. Ако с Pn означим броя на пермутациите на n-елемента, то Pn = n! = 1.2.3. ...n.
###### Задача 6.
Да се дефинира функция на С++, която намира броя на пермутациите на зададеното от потребителя множество.


#### Неподвижни точки
Ако f : A → B и f(x) = x, за някое x ∈ A, то x наричаме неподвижна точка за функцията f. Ако всяка точка от множеството A е неподвижна, то функцията f наричаме идентитет върху A и означаваме с idA или само с id, ако
множеството A се подразбира.
###### Задача 7.
Да се дефинира функция на С++, която проверява дали записана в масив пермутация има неподвижна точка.
###### Задача 8.
Да се дефинира функция на С++, която намира броя на неподвижните точки на една пермутация.
###### Задача 9. 
Да се дефинира функция на С++, която проверява дали записана в масив пермутация е идентитет.


#### Независими цикли
Съществува компактен начин за представяне на една пермутация σ върху крайно множество S, т. нар. представяне като произведение на независими цикли. Започвайки от някой произволен елемент на S, да речем x, записваме редицата *(x, σ(x), σ(σ(x)), .. .)*
от последователни образи на σ дотогава, докато съответния образ не е равен на x. Затварянето на скобата дава съответния цикъл на σ. След това продължаваме с избор на произволен друг елемент y от S, който не е бил включен в някои от предходните цикли и така формираме нов цикъл включващ y. Тъй като S е крайно множество този процес ще е краен и ни води до образуването на всички цикли на пермутацията. В случай когато дължината на един цикъл е единица (т.е. елемента е неподвижен) е прието за по-добра компактност да се пропуска, като се подразбира. Това представянене е еднозначно с точност до циклично пренареждане на елементите в цикъла и пренареждане на самите цикли. 

![alt text](https://raw.githubusercontent.com/KingGVT/PermutationsProject/master/PermutationsImage2.PNG?token=AYwFVTgExz07bsl6gn6mF_0_HNk3wRYsks5cYvmiwA%3D%3D)
