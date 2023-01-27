# general
```cpp
int i = 25;
string s = to_string(i);
int j = int(i-'0');
j == i; //true
```
# list
# array
# vector
## modify
### add to end
```cpp
myVct.push_back(myvar);
```
add vector to end myVctr
```cpp
myVctr.insert(myVctr.end(), v[i].begin(), v[i].end());
```
### erase from middle
```cpp
myVct.erase(myVct.begin()+myNum);
```
# string
```cpp
std::stringstream ss;

//put arbitrary formatted data into the stream
ss << 4.5 << ", " << 4 << " whatever";

//convert the stream buffer into a string
std::string str = ss.str();
```
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
could also use size_t
```cpp
for (auto i = myMap.begin(); i != myMap.end(); ++i){
    myVctr[i->second].push_back(i->first);
}
```
or 
```cpp
for (auto p : myMap) {
    myVctr[p.second].push_back(p.first);
}
```