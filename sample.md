# slide 1
１ページ目

---
# slide 2
２ページ目

--

１行追記

--

１行追記

--

１行を
--
分割して
--
追記

---
# slide 3

デフォルトの表示位置(左上)

---
class: middle center
# slide 4

真ん中に表示

---
class: bottom right
# slide 5

右下に表示

---
# slide 6

.left[
テキスト左寄せ
```
.left[テキスト左寄せ]
```
]

.center[
テキスト中央
]

.right[テキスト右寄せ]

```

.center[テキスト中央]

.right[テキスト右寄せ]
```

---
layout: true
.center[ title ]
---

# slide 7

`layout: ture` にすると、そのページの内容(ここでは、title の文字列)が `layout: false` にするまでずっと表示される。

```
---
layout: true
.center[ title ]
---

# slide 7
 :
---

# slide 8
 :
---
layout: false
# slide 9
 :
---
```

---

# slide 8

ここでも表示される

```
---
layout: true
.center[ title ]
---

# slide 7
 :
---

# slide 8
 :
---
layout: false
# slide 9
 :
---
```
---
layout: false
# slide 9

ここで `layout: false` にしたので、title の文字列が表示されなくなる。

```
---
layout: true
.center[ title ]
---

# slide 7
 :
---

# slide 8
 :
---
layout: false
# slide 9
 :
---
```

---
# slide 10

コードのハイライトもOK

```c
#include <stdio.h>
int main(void){
    printf("Hello World!\n");
    return 0;
}
```

---
# slide 11

css を記載すれば、２列表示も可能


.left-column[
## 左列

```c
#include <stdio.h>
int main(void){
    printf("Hello World!\n");
    return 0;
}
```
]

.right-column[
## 右列

aaa bbb
]

---
# slide 10

.center[
おしまい
]
