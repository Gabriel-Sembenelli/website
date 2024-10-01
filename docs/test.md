# Welcome to MkDocs
<!--- só pode um título de #, o resto não aparece no sumário --->
<!--- precisa existir um index.md --->

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Fazendo uns testes

### Math
$$\sum_{k=0}^{100} a^k,\; 0 < |a| <1$$

### Tables
First Header | Second Header | Third Header
------------ | ------------- | ------------
Content Cell | Content Cell  | Content Cell
Content Cell | Content Cell  | Content Cell

| First Header | Second Header | Third Header |
| ------------ | ------------- | ------------ |
| Content Cell | Content Cell  | Content Cell |
| Content Cell | Content Cell  | Content Cell |

First Header | Second Header | Third Header
:----------- |:-------------:| -----------:
Left         | Center        | Right
Left         | Center        | Right

### Code

#### Python

```py
def fn():
    pass
```

```py title="custom_title.py" linenums="2" hl_lines="3"
def fn():
    for i in range(10):
        for j in range(10):
            print(i, j)
```

#### C++

```cpp
#include<bits/stdc++.h>
using namespace std;

signed main(){
    return 0;
}
```

# Utilitários

- [Math](https://squidfunk.github.io/mkdocs-material/reference/math/#katex-mkdocsyml)
- [Blogs](https://squidfunk.github.io/mkdocs-material/tutorials/blogs/basic/)
- [KaTeX](https://katex.org/docs/supported.html#environments)