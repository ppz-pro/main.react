# React APP

一种前端框架

+ app (top level module, business)
	+ ui (root ui)
	+ ss (global state and services)
	+ modules
		+ module1 (maybe pages)
			+ ui (page)
			+ ss (service and state)
				+ http api
				+ state
				+ hooks
			+ modules
				+ module1
		+ module2
	+ init.ts (名字使用 init 而非 index：语义性更强)
+ common (bussness 无关代码）
	+ utils
	+ cmps
	+ hooks

> 子模块：如果一个模块（A）只与另一个唯一模块（B）操作，那么 A 是 B 的子模块。因为 A 只与 B 交互，所以就不存在“跨子模块交互”，但首子模块影响的“全局状态”会影响依赖于此状态的其他模块。
