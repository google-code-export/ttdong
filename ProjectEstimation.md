

# Project Estimation #

## Timeline ##
**Timebox of development:** 7/11/2011 ~ 12/25/2011, 24 weeks, 12 sprints

**Beta Release:** 1/1/2012

**RC1:** 2/1/2012

**Release:** 2/22/2012

<br>
<h2>Product Backlog</h2>
<table><thead><th> <b>Epic</b> </th><th> <b>User Story</b> </th><th> <b>Description</b> </th><th> <b>Target User</b> </th><th> <b>Priority</b> </th><th> <b>Estimation (Sprint)</b> </th></thead><tbody>
<tr><td> 基础框架 </td><td> 网页设计 </td><td> 包括导航栏（页头），版权申明（页尾），操作面板（左侧），广告栏（右侧），内容区（中间） </td><td> / </td><td> P0 </td><td> 1 </td></tr>
<tr><td> 用户系统 </td><td> 角色组件 </td><td> 操作面板的任一选项唯一绑定于某一特定角色，用户所对应的角色组合决定了其操作面板的内容 </td><td> / </td><td> P0 </td><td> 1 </td></tr>
<tr><td>  </td><td> 注册组件 </td><td> 患者自行注册用户，医生由管理员添加，普通管理员由超级管理员添加，超级管理员网站自带 </td><td> P,A </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 登陆组件 </td><td> 需提供验证码支持 </td><td> ALL </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 更新组件 </td><td> 用于更新个人信息 </td><td> P,D </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 删除用户组件 </td><td> 仅限管理员身份用户使用 </td><td> A </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 找回密码组件 </td><td> 通过邮箱发送原始密码 </td><td> ALL </td><td> P1 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 黑名单组件 </td><td> 自动规则匹配，无需人工干预 </td><td> / </td><td> P1 </td><td> 1 </td></tr>
<tr><td> 门诊预约 </td><td> 短信系统 </td><td> 预约成功后通过短信发送预约号 </td><td> P </td><td> P0 </td><td> ? </td></tr>
<tr><td>  </td><td> 预约组件 </td><td> 用于增删改查任一预约 </td><td> / </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 基本流程 </td><td> 登陆，选择专家，选择日期，条款确认，信誉审核，成功预约 </td><td> P </td><td> P0 </td><td> 1 </td></tr>
<tr><td>  </td><td> 我的预约 </td><td> 取消活动预约，查看历史预约 </td><td> P </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 门诊管理 </td><td> 按日查看所有患者预约 </td><td> A </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td> 电话咨询 </td><td> 在线支付 </td><td> 通过网银支付系统完成付款 </td><td> P </td><td> P0 </td><td> ? </td></tr>
<tr><td>  </td><td> 订单组件 </td><td> 用于增删改查任一订单 </td><td> / </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 基本流程 </td><td> 登陆，选择专家，输入病情联系方式，条款确认，订单生成，在线支付 </td><td> P </td><td> P0 </td><td> 1 </td></tr>
<tr><td>  </td><td> 我的订单 </td><td> 查询订单状态，修改病情联系方式，取消活动订单，查看历史订单 </td><td> P </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 订单管理 </td><td> 联系专家/患者商定咨询时间，将其填入订单，并更新订单状态 </td><td> A </td><td> P0 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 订单查看 </td><td> 查看专家收到的订单信息，付款状态以及历史订单 </td><td> D </td><td> P1 </td><td> 0.5 </td></tr>
<tr><td>  </td><td> 退款组件 </td><td> 若患者取消任一已付款未完成订单，该订单进入退款流程 </td><td> P,A </td><td> P1 </td><td> ? </td></tr>
<tr><td>  </td><td> 结算组件 </td><td> 用于结算、支付专家收益 </td><td> D,A </td><td> P2 </td><td> ? </td></tr>
<tr><td> 科室管理 </td><td> 排班组件 </td><td> 用于输入、更新医生最新排班安排 </td><td> A </td><td> P1 </td><td> ? </td></tr>
<tr><td> 内容管理 </td><td> 公告新闻 </td><td> 管理网站的公告、新闻、活动等信息 </td><td> A </td><td> P1 </td><td> 1 </td></tr>
<tr><td> 文字咨询 </td><td> 提问组件 </td><td> 患者就自身病情咨询医生 </td><td> P </td><td> P2 </td><td> ? </td></tr>
<tr><td>  </td><td> 回复组件 </td><td> 医生回复患者提问 </td><td> D </td><td> P2 </td><td> ? </td></tr></tbody></table>

<i>P: Patient, D: Doctor, A: Admin</i>