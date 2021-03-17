# 事件通知
事件通知是针对资源生命周期中平台底层基础设施维护、资源重要属性变更或某些操作执行结果所发送的通知。基于事件用户可及时获知资源动态，完善云上业务的自动化运维和监控流程。<br>

## 事件列表 
云主机目前提供以下事件通知：
<table>
	<thead>
    <tr>
		    <th>事件类型</th>
      	<th>事件名称</th>
      	<th>事件代码</th>
        <th>事件描述</th>
        <th>应对建议</th>
    </tr>
	</thead>
	<tbody>
    <tr>
        <td rowspan="3">异常事件</td>
        <td> 实例创建失败</td>
        <td>SystemFailure.Delete</td>
        <td> 实例创建请求成功后，由于系统原因导致的资源回滚删除 </td>
        <td> 尝试重新创建，如仍无法成功请咨询客户</td>
    </tr>
    <tr>
        <td> 系统异常实例不可用</td>
        <td> SystemFailure.Fault</td>
        <td> 物理机故障，且实例规格不支持热迁移（带本地数据盘的规格，如存储优化型，GPU型），无法通过热迁快速恢复 </td>
        <td> 联系客服，确认本地数据可以清除后又后台操作迁移</td>
    </tr>
    <tr>
        <td> 系统异常实例迁移</td>
        <td> SystemFailure.Migrate</td>
        <td> 除用户无感热迁移外其他的迁移操作，如物理机严重故障已导致实例不可用或不支持热迁移的规格在客户确认后进行关机迁移 </td>
        <td> 关注业务影响</td>
    </tr>
    <tr>
        <td rowspan="4">欠费/到期</td>
        <td> 实例停止（资源到期）</td>
        <td>InstanceExpiration.Stop</td>
        <td> 包年包月计费实例到期后停服 </td>
        <td> 如继续使用请续费后重新启动；如不再使用请确保重要数据已备份，随后操作删除或等待系统7日后自动删除。</td>
    </tr>
    <tr>
        <td> 实例删除（资源到期）</td>
        <td> InstanceExpiration.Delete</td>
        <td> 包年包月计费实例到期7天后删除 </td>
        <td>  </td>
    </tr>
    <tr>
        <td> 实例停止（资源欠费）</td>
        <td>	InstanceUnbalanced.Stop</td>
        <td> 按配置计费实例欠费后停服 </td>
        <td> 如继续使用请充值后重新启动；如不再使用请确保重要数据已备份，随后操作删除或等待系统7日后自动删除。</td>
    </tr>
    <tr>
        <td> 实例删除（资源欠费）</td>
        <td> InstanceUnbalanced.Delete</td>
        <td> 按配置计费实例欠费7天后删除 </td>
        <td>  </td>
    </tr> 
    <tr>
        <td> 状态变更</td>
        <td> 实例状态变更</td>
        <td> StateChange </td>
        <td> 用户或系统导致的实例任何状态变更（目前仅支持创建和删除两类操作导致的状态变更） </td>
        <td> 关注状态变更是否符合预期 </td>
    </tr>        
</table> 
 
 
 
 
<div id="user-content-1"></div>

## 监控插件安装说明

云主机监控数据的采集和上报依赖于官方镜像系统组件'JCS-Agent'中的'MonitorPlugin'插件，官方镜像在2019年5月-7月期间进行升级默认安装了升级工具'ifrit'以实现JCS-Agent的自动升级。<br>

如您当前实例中未安装JCS-Agent或已安装但版本过低不具备自动升级能力，可在确保已卸载早期系统组件cloud-init和QGA的前提下，直接安装ifrit，安装完成10分钟内，JCS-Agent会被自动安装/更新为最新版本。<br>

* cloud-init和QGA卸载方法以及Ifrit安装方法详见：[官方镜像系统组件-JCS-Agent](https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image#user-content-1)
* JCS-Agent版本查看方式：
  * Linux：
  `
   ps -ef|grep MonitorPlugin
  `
  * Windows：
  `
  wmic process where caption="MonitorPlugin.exe" get caption,commandline /value
  `
  
## 监控数据说明
* 监控数据采集周期为10s，最小展示间隔为1min；
* 不同指标的默认聚合方式不同，可在监控图中查看各指标的聚合方式；
* 统计周期默认支持1小时、6小时、12小时、1天、3天、7天及14天，此外还支持您设置统计周期，最短为1分钟最长为一个月；
* 不同统计周期监控值会做对应聚合，例如6小时统计周期情况下，监控图上间隔5分钟显示一个监控值，该监控值为对应统计周期内采集值的聚合，当前仅支持以默认聚合方式查询；
* 监控数据最长保存180天，在控制台可直接用户可以观察30天的监控数据，若需要获取30天-180天的监控数据，请提交工单。

## 其他
* bps表示每秒传输bit数，ps为per second，意同/s；
* Bps表示每秒传输Byte数，ps为per second，意同/s；
* Kbps=1000bps，KBps=1000Bps。
  
 
   
