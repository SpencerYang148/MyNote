## Hook特点
1. **向下兼容、无破坏性升级**
2. **无需修改组件结构的情况下复用状态逻辑，这些逻辑可以单独测试并复用**（以往需要复用状态逻辑，就会存在 providers，consumers，高阶组件，render props 等其他抽象层组成的组件形成的“嵌套地狱”）
3. **将组件中相互关联的部分拆分成更小的函数，组件更容易理解**（避免充斥生命周期，以及关联的逻辑被分隔到不同的生命周期）
4. **函数式编程的便利，同时避免了class难以理解的this问题和编译冗余**