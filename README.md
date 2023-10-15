# Hello World 👋

<!---
/*
class GameDev
{
public:
    GameDev(std::string name,
            std::string pronouns,
            std::vector<std::string> mainRoles,
            std::vector<std::string> languagesSpoken) :
        name(name), pronouns(pronouns), mainRoles(mainRoles), languagesSpoken(languagesSpoken)
    {
    }

    void SayHi()
    {
        std::cout << "Hi! Welcome to my GitHub profile, I hope you find some of my work interesting!" << std::endl;
    }

private:
    std::string name;
    std::string pronouns;
    std::vector<std::string> mainRoles;
    std::vector<std::string> languagesSpoken;
}
*/
-->

```c++
#include <iostream>
#include <string>
#include <vector>
#include <memory>

#include "GameDev.h"

int main()
{
    std::string myName = "Mark Melia";
    std::string myPronouns = "He|Him";
    std::vector<std::string> myMainRoles {"Gameplay Programmer", "AI Programmer", "Game Designer"};
    std::vector<std::string> myLanguagesSpoken {"Spanish", "English", "Catalan", "French"};

    std::unique_ptr<GameDev> me = std::make_unique<GameDev>(myName, myPronouns, myMainRoles, myLanguagesSpoken);
    me->SayHi(); // Hi! Welcome to my GitHub profile, I hope you find some of my work interesting!

    std::cin.get();
    return 0;
}
```
