# trmclr
A [130 lines header](https://github.com/matovitch/trmclr/blob/master/trmclr.hpp) for coloring your terminal outputs

## Example

```c++
#include "trmclr.hpp"
#include <iostream>

int main()
{
    trmclr::Style fancy_style(trmclr::Background::LIGHT_BLUE    |
                              trmclr::Foreground::WHITE         |
                              trmclr::Attribute::UNDERLINED     |
                              trmclr::Attribute::BOLD);

    trmclr::Style basic_style(trmclr::Attribute::DEFAULT);

    std::cout << fancy_style << "Hello " 
              << basic_style << "World!" << std::endl;

    return 0;
}
```
