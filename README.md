**1. Clone wallet sources**

```
git clone https://github.com/interplanetaryreservecurrency/UNIVERSAL.git
```

* cd UNIVERSAL**

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "Latnum")
set(CN_CURRENCY_DISPLAY_NAME "latnum")
set(CN_CURRENCY_TICKER "LTN")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../latnum cryptonote
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/interplanetaryreservecurrency/Latnum.git cryptonote
```


**4. Build**

```
mkdir build && cd build && cmake .. && make
```
