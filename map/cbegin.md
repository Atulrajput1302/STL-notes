# cbegin

**Description :** This is a built-in function in C++ STL which returns a constant iterator referring to the first element in the map container. Since map container contains the element in an ordered way, cbegin() will point to that element that will come first according to the container’s sorting criterion.

**Example** :

```cpp
// C++ program to illustrate the map::cbegin() function 
#include <bits/stdc++.h> 
  
int main() { 
  
    // initialize container 
    std::map<int, int> mp; 
  
    // insert elements in random order 
    mp.insert({ 2, 30 }); 
    mp.insert({ 1, 40 }); 
    mp.insert({ 3, 60 }); 
    mp.insert({ 4, 20 }); 
    mp.insert({ 5, 50 }); 
  
    auto ite = mp.cbegin(); //cbegin() 
  
    std::cout << "The first element is: "; 
    std::cout << "{" << ite->first << ", "
         << ite->second << "}\n"; 
  
    // prints the elements 
    std::cout << "\nThe map is : \n"; 
    std::cout << "KEY\tELEMENT\n"; 
    for (auto itr = mp.cbegin(); itr != mp.cend(); ++itr) { 
        std::cout << itr->first << '\t' << itr->second << '\n'; 
    } 
    return 0; 
} 
```
**[Run Code](https://rextester.com/ERYQ22608)**
