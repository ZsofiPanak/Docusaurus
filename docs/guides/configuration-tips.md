---
sidebar_position: 1
---
title: Konfigurációs tippek

# Az alkalmazás konfigurációja

A globális  (```globally```) definíció azt jelenti, hogy vonatkozik minden forrás állományra.

- [**```DOCUTEST_CONFIG_IMPLEMENT_WITH_MAIN```**](#docutest_config_implement_with_main)
- [**```DOCUTEST_CONFIG_IMPLEMENT```**](#docutest_config_implement)
- [**```DOCUTEST_CONFIG_DISABLE```**](#docutest_config_disable)

Az alábbiakban az alapvető konfigurációs beállításokat olvashatod:

### **```DOCUTEST_CONFIG_IMPLEMENT_WITH_MAIN```**

```c++
#define DOCUTEST_CONFIG_IMPLEMENT_WITH_MAIN
#include "docutest.h"
```

Csak abban a forrásban definiálható amelyben a gyűjtemény implementálásra kerül. A definiáláskor létrehozza a ```main()``` belépési pontot is.

### **```DOCUTEST_CONFIG_IMPLEMENT```**

Csak abban a forrásban definiálható amelyben a gyűjtemény implementálásra kerül, azonban lehetőséget ad arra hogy más forrásból hivatkozd a ```main()``` belépési pontot.

### **```DOCUTEST_CONFIG_DISABLE```**

A beállítás hatására minden teszteset eltávolításra kerül a bináris állományokból beleértve az egyedileg definiált teszteseteket is.

 A beállítás globálisan értelmezett.

---------------

[Kezdőlap](readme.md#reference)