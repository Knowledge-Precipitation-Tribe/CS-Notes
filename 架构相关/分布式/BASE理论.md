# BASE理论
BASE理论常应用于应用的架构设计，核心思想是即使无法做到强一致性，但应该采用合适的方式保证最终一致性，BASE理论包括以下几个部分：
- 基本可用(Basically Available)：损失部分可用性，保证整体可用性
- 软状态(Soft-state)：允许系统的状态同步存在一定的延迟，不会影响系统即可
- 最终一致(Eventually Consistent)：经过一段时间后，系统能够达到一致性

BASE理论本质上是对[[CAP理论]]的延伸，是对 CAP 中 AP 方案的一个补充。