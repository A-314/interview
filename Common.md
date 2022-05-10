## 1. Как работает класс StringJoiner?
Как позволяет объединять несколько строк, а в конструктор передать метод разделитель. Данный класс появился в Java 8.
- StringJoiner joiner = new StringJoiner(",");
 joiner.add("bar");
 joiner.add("baz");
 String joined = joiner.toString()_
-  joined = new StringJoiner("-").add("foo").add("bar").add("baz").toString();_
- Также String использует два новых статических метода join() StringJoiner*
- // join(CharSequence delimiter, CharSequence... elements)
String joined = String.join("/", "2014", "10", "28" ); _
## 2. Как работает String.format
String.format("a = %d, b = %d, c = %d", 1, 4, 3)
где строка мы пишем %s, если число — %d
