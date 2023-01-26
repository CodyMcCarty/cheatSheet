# general
```cpp
var.size() // not length
```
# list
# array
# vector
## modify
### add to end
```cpp
myVct.push_back(myvar);
```
### erase from middle
```cpp
myVct.erase(myVct.begin()+myNum);
```
# string
# map
## declare
```cpp
unordered_map<char, int> charCount;
```
## modify
make new at key:1 or ++
```cpp
charCount[letter]++; 
```
## loop
```cpp
for (auto i = myMap.begin(); i != myMap.end(); ++i)
```