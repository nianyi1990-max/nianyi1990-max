---
merits: mermaid
---
```mermaid
graph TD
  A[CPU(中央处理器)] -->|数据总线| B[内存(存储程序和数据)]
  A -->|控制总线| C[输入/输出设备(键盘、鼠标、显示器)]
  B -->|地址总线| A
  C -->|数据总线| A
  D[控制单元(指令解码)] --> A
  E[算术逻辑单元(ALU)(执行运算)] --> A
  F[寄存器组(存储临时数据)] --> A
  G[程序计数器(PC)(下一条指令地址)] --> D
  H[指令寄存器(IR)(当前指令)] --> D
  I[内存地址寄存器(MAR)(要访问的内存地址)] --> B
  J[内存数据寄存器(MDR)(读取或写入的数据)] --> B
  K[累加器(ACC)(存储运算结果)] --> E
  L[状态寄存器(PSW)(处理器状态信息)] --> D
  style A fill:#f9f,stroke:#333,stroke-width:2px
  style B fill:#ccf,stroke:#333,stroke-width:1px
  style C fill:#cfc,stroke:#333,stroke-width:1px
  style D fill:#f99,stroke:#333,stroke-width:1px
  style E fill:#9f9,stroke:#333,stroke-width:1px
  style F fill:#9ff,stroke:#333,stroke-width:1px
```
