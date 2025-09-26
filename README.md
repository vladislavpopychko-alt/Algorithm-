# Сравнение создания массивов (списков) и организации стеков в Java, Python и C++ (Попычко Владислав Андреевич , УИЮО-10-24)
## Создание массива (списка)
### Java
```java
public class Arrays{
    public static void main(String[]){
        List mylist=new ArrayList();
    mylist.add("P");
    mylist.add("Q")
    mylist.add("R")
    }
}
```
- Используется `Arrays` из Java Collections Framework
- Явное указание типа через дженерики (`<String>`)
- Метод `add()` для добавления элементов

### Python
```py
list=['volleyball', 'football','basketball','soccer','skiing']
list.append('skating')
```
- Используется встроенный тип `list` как динамический массив
- Метод 'list.append()' для добавления элементов
- Динамическая типизация 

### C++
```cpp
std::vector<std::string> vec;
vec.push_back("элемент1");
vec.push_back("элемент2");
```
- Используется `std::vector` из STL как динамический массив
- Указание типа элементов (`std::string`)
- Метод `push_back()` для добавления элементов
## Организация стека
### Java
```java
Stack<String> stack = new Stack<>();
stack.push("элемент1");
stack.push("элемент2");
String top = stack.pop();
```
- Используется класс `Stack` из java.util
- Метод `pop()` одновременно возвращает и удаляет элемент
- Использование дженериков для типизации
### Python
```py
stack = []
stack.append("элемент1")
stack.append("элемент2")
top = stack.pop()
```
- Используется обычный список как стек
- `append()` для добавления, `pop()` для извлечения
- Мин. синтаксис, встроенная поддержка
### C++
```cpp
std::stack<std::string> st;
st.push("элемент1");
st.push("элемент2");
std::string top = st.top();
st.pop();
```
- Используется специализированный класс `std::stack`
- `top()` получает элемент, `pop()` удаляет
- Явное указ. типа данных
## Вывод
Эти языки демонстрируют разные подходы к созданию массивов (списков) и организации стеков. C++ использует контроль и эффективность, Java делает ставку на безопасность и структуру, а Python ставит выше всего простоту и скорость написания кода

