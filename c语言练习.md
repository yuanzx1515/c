![photo_2023-11-18_01-59-43.jpg](photo_2023-11-18_01-59-43.jpg)

```
#include <stdio.h>

int main() {
    // 从用户获取输入
    int a, n;
    printf("请输入a的值：");
    scanf("%d", &a);
    printf("请输入n的值：");
    scanf("%d", &n);

    // 初始化 Sn 和当前项 current_term
    int sn = 0;
    int current_term = a;

    // 使用 for 循环计算 Sn
    for (int i = 0; i < n; ++i) {
        sn += current_term;
        current_term = current_term * 10 + a;
    }

    // 输出结果
    printf("S%d = %d\n", n, sn);

    return 0;
}
