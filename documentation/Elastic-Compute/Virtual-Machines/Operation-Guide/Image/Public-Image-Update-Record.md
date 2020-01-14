# 官方镜像更新记录
* [CentOS](public-image-update-record#user-content-1)
* [Ubuntu](public-image-update-record#user-content-2)
* [Windows Server](public-image-update-record#user-content-3)

<div id="user-content-1"></div>

## CentOS
<table>
	<thead>
    <tr>
        <th>更新时间及地域</th>
      	<th>涉及镜像版本</th>
      	<th>更新内容</th>
        <th>相关参考</th>
    </tr>
  	</thead>
    <tbody>     
    <tr>
        <td>2019-07-03 北京</td>
      	<td>CentOS 7.6</td>
      	<td>发布上线</td>
        <td> </td>
    </tr>    	    
    <tr>
        <td>2019-07-30 北京</td>
      	<td rowspan="4">CentOS 7.4, CentOS 7.3, CentOS 7.2, CentOS 7.2 NatGateway<br>CentOS 6.9, CentOS 6.8, CentOS 6.6, CentOS 6.5</td>
      	<td rowspan="4">* 安装运维组件Ifrit<br>* 更新JCS-Agent以支持Ifrit管理<br>* 安装安全辅助插件Jdog-Monitor</td>
        <td rowspan="4">*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a> </td>
    </tr>   
    <tr>
        <td>2019-05-29 广州</td>
    </tr>  
    <tr>
        <td>2019-05-22 上海</td>
    </tr> 
    <tr>
        <td>2019-05-14 宿迁</td>
    </tr> 
    <tr>
        <td>2019-03-26 北京/广州/宿迁/上海</td>
      	<td>CentOS 7.1</td>
      	<td>* 镜像下线</td>
        <td> </td>
    </tr>
    <tr>
        <td>2018-12-13 北京</td>
      	<td rowspan="3">CentOS 7.4, CentOS 7.3, CentOS 7.2, CentOS 7.2 NatGateway, CentOS 7.1<br>CentOS 6.9, CentOS 6.8, CentOS 6.6, CentOS 6.5</td>
      	<td rowspan="3">* 更新JCS-Agent以支持启动脚本（userdata）<br>* NTP关闭Monlist功能以避免反射式分布式拒绝服务攻击</td>
        <td rowspan="3">*<a href="https://docs.jdcloud.com/cn/virtual-machines/userdata">自定义脚本</a> <br>*<a href="https://docs.jdcloud.com/cn/security-instruction/ntp-monlist-vulnerability">NTP服务和Monlist漏洞</a></td>
    </tr>   
    <tr>
        <td>2018-12-11 广州</td>
    </tr>  
    <tr>
        <td>2018-12-06 上海/宿迁</td>
    </tr> 
    <tr>
        <td>2018-10-17 北京/宿迁</td>
      	<td rowspan="2">CentOS 7.4, CentOS 7.3, CentOS 7.2, CentOS 7.2 NatGateway, CentOS 7.1<br>CentOS 6.9, CentOS 6.8, CentOS 6.6, CentOS 6.5</td>
      	<td rowspan="2">* JCS-Agent替换QGA(qemu-guest-agent)<br>* 关闭SSH DNS反向解析功能</td>
        <td rowspan="2">*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a></td>
    </tr>   
    <tr>
        <td>2018-10-11 广州/上海</td>
    </tr>  
    <tr>
        <td>2018-05-18 北京/广州/宿迁/上海</td>
      	<td>CentOS 7.4, CentOS 7.3, CentOS 7.2, CentOS 7.2 NatGateway, CentOS 7.1<br>CentOS 6.9, CentOS 6.8, CentOS 6.6, CentOS 6.5</td>
      	<td>* CVE-2018-1111 DHCP Client 代码执行漏洞</td>
        <td>*<a href="https://www.jdcloud.com/cn/notice/detail/63/type/4">漏洞说明</a> </td>
    </tr>
    <tr>
        <td>2018-02-01 北京/广州/宿迁/上海</td>
      	<td>CentOS 7.4, CentOS 6.9</td>
      	<td>* 发布上线</td>
        <td> </td>
    </tr>    
    <tr>
        <td>2018-01-11 北京/广州/宿迁/上海</td>
      	<td>CentOS 6.7, CentOS 6.4, CentOS 6.3, CentOS 6.1</td>
      	<td>* 镜像下线</td>
        <td> </td>
    </tr>
</tbody>
</table>





<div id="user-content-2"></div>

## Ubuntu
<table>
	<thead>
    <tr>
        <th>更新时间及地域</th>
      	<th>涉及镜像版本</th>
      	<th>更新内容</th>
        <th>相关参考</th>
    </tr>
  	</thead>
    <tbody>    
    <tr>
        <td>2019-12-19 北京/广州/宿迁/上海</td>
      	<td>Ubuntu 18.04</td>
      	<td>* 发布上线</td>
        <td> </td>
    </tr>    
    <tr>
        <td>2019-07-04 北京</td>
      	<td rowspan="4">Ubuntu 16.04, Ubuntu 14.04</td>
      	<td rowspan="4">* 安装运维组件Ifrit<br>* 更新JCS-Agent以支持Ifrit管理<br>* 安装安全辅助插件Jdog-Monitor</td>
        <td rowspan="4">*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a> </td>
    </tr>  
    <tr>
        <td>2019-05-30 广州</td>
    </tr>  
    <tr>
        <td>2019-05-23 上海</td>
    </tr> 
    <tr>
        <td>2019-05-16 宿迁</td>
    </tr> 
    <tr>
        <td>2018-12-13 北京</td>
      	<td rowspan="4">Ubuntu 16.04, Ubuntu 14.04</td>
      	<td rowspan="4">* 更新JCS-Agent以支持启动脚本（userdata）<br>* NTP关闭Monlist功能以避免反射式分布式拒绝服务攻击</td>
        <td rowspan="4">*<a href="https://docs.jdcloud.com/cn/virtual-machines/userdata">自定义脚本</a> <br>*<a href="https://docs.jdcloud.com/cn/security-instruction/ntp-monlist-vulnerability">NTP服务和Monlist漏洞</a></td>
    </tr>   
    <tr>
        <td>2018-12-12 宿迁</td>
    </tr>  
    <tr>
        <td>2018-12-11 广州</td>
    </tr> 
    <tr>
        <td>2018-12-07 上海</td>
    </tr> 
    <tr>
        <td>2018-10-18 北京/宿迁</td>
      	<td rowspan="2">Ubuntu 16.04, Ubuntu 14.04</td>
      	<td rowspan="2">* JCS-Agent替换QGA(qemu-guest-agent)</td>
        <td rowspan="2">*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a></td>
    </tr>   
    <tr>
        <td>2018-10-09 广州/上海</td>
    </tr> 
    <tr>
        <td>2018-03-23 北京/广州/宿迁/上海</td>
      	<td>Ubuntu 12.04</td>
      	<td>* 镜像下线</td>
        <td> </td>
    </tr>  
</tbody>
</table>




<div id="user-content-3"></div>

## Windows Server

<table>
	<thead>
    <tr>
        <th>更新时间及地域</th>
      	<th>涉及镜像版本</th>
      	<th>更新内容</th>
        <th>相关参考</th>
    </tr>
  	</thead>
    <tbody>    
    <tr>
        <td>2019-08-27 北京/广州/宿迁/上海</td>
      	<td>Windows Server 2016 数据中心版 中文版<br>Windows Server 2012 R2 标准版 中文版<br>Windows Server 2008 R2 数据中心版 中文版</td>
      	<td>* 补丁更新<br>* CVE-2019-1181/1182 RDP远程执行代码漏洞修复<br>* 安装安全插件Jdog-Monitor</td>
        <td>* <a href="https://www.jdcloud.com/cn/notice/detail/741/type/5">漏洞说明</a><br>* <a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a> </td>
    </tr>    
    <tr>
        <td>2019-07-04 北京</td>
      	<td rowspan="2">Windows Server 2016 数据中心版 中文版<br>Windows Server 2012 R2 标准版 中文版<br>Windows Server 2008 R2 数据中心版 中文版</td>
      	<td rowspan="2">* 补丁更新</td>
        <td rowspan="2"> </td>
    </tr>   
    <tr>
        <td>2019-07-04 广州/宿迁/上海</td>
    </tr>  
    <tr>
        <td>2019-05-16 北京/广州/宿迁/上海</td>
      	<td>Windows Server 2016 数据中心版 中文版<br>Windows Server 2012 R2 标准版 中文版<br>Windows Server 2008 R2 中文版</td>
      	<td>* 补丁更新<br>* CVE-2019-0708 RDP远程代码执行高危漏洞修复<br>* 安装运维组件Ifrit<br>* 更新JCS-Agent以支持Ifrit管理</td>      
	<td>*<a href="https://www.jdcloud.com/cn/notice/detail/678/type/5">漏洞说明</a> <br>*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a>  </td>
    </tr>  
    <tr>
        <td>2018-12-13 北京</td>
      	<td rowspan="4">Windows Server 2016 数据中心版 中文版<br>Windows Server 2012 R2 标准版 中文版<br>Windows Server 2008 R2 中文版</td>
      	<td rowspan="4">* 更新JCS-Agent以支持启动脚本（userdata）<br>* 补丁更新</td>
        <td rowspan="4">*<a href="https://docs.jdcloud.com/cn/virtual-machines/userdata">自定义脚本</a> </td>
    </tr>   
    <tr>
        <td>2018-12-12 宿迁</td>
    </tr>  
    <tr>
        <td>2018-12-11 广州</td>
    </tr> 
    <tr>
        <td>2018-12-07 上海</td>
    </tr> 
    <tr>
        <td>2018-09-19 北京/广州/宿迁/上海</td>
      	<td>Windows Server 2008 R2 中文版</td>
      	<td rowspan="2">* MS15-034 远程执行代码漏洞修复</td>
        <td rowspan="2"> </td>
    </tr>   
    <tr>
        <td>2018-09-12 北京/广州/宿迁/上海</td>
      	<td>Windows Server 2012 R2 标准版 中文版</td>	    
    <tr>
        <td>2018-05-31 广州/宿迁/上海</td>
      	<td rowspan="2">Windows Server 2016 数据中心版 中文版<br>Windows Server 2012 R2 标准版 中文版<br>Windows Server 2008 R2 中文版</td>
      	<td rowspan="2">* JCS-Agent替换QGA(qemu-guest-agent)<br>* 激活方式从MAK调整为KMS</td>
        <td rowspan="2">*<a href="https://docs.jdcloud.com/cn/virtual-machines/default-agent-in-public-image">官方镜像系统组件</a><br>* <a href="https://docs.jdcloud.com/cn/virtual-machines/windows-cloud-host-adjustment-activation-mode-is-kms">Windows云主机调整激活方式为KMS</a></td>
    </tr>   
    <tr>
        <td>2018-07-16 北京</td>
    </tr> 
    <tr>
        <td>2018-05-31 北京/广州/宿迁/上海</td>
      	<td>Windows Server 2016 数据中心版 中文版</td>
      	<td>* 发布上线</td>
        <td> </td>
    </tr>  	    
</tbody>
</table>
