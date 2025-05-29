<h1> Quickly deploy the Python runtime environment </h1>

<h2> Overview </h2>

<p>Python is a widely used high-level programming language. Python's design philosophy emphasizes code readability and a simple and straightforward syntax, which makes it a popular language for beginners to learn, and is also used by many professional developers for large projects. For more information, see <a href = "https://www.python.org/">Python website </a>. </p>

<p> This service supports deployment on existing ECS instances (Linux) and deployment on new ECS instances (Linux). </p>

<h2> Billing instructions </h2>

<p> The cost of deploying the Python runtime environment on the computing nest mainly involves:</p>

<ul>
<li> Selected vCPU and Memory Specifications </li>
<li> Disk capacity </li>
<li> Internet bandwidth </li>
</ul>

<p> Billing method: Pay-As-You-Go (hourly)</p>

<p> The estimated cost is visible in real time when the instance is created. </p>

<h2> Permissions required for RAM accounts </h2>

<p> The Python runtime environment needs to access and create resources such as ECS and VPC. If you use a RAM user to create a service instance, you need to add the corresponding resource permissions to the account of the RAM user before creating the service instance. For more information about how to add RAM permissions, see <a href = "https://help.aliyun.com/document_detail/121945.html"> Authorize RAM users </a>.
. The required permissions are shown in the following table. </p>

<table>
<thead>
<tr>
<th> Permission policy name </th>
<th> Remarks </th>
</tr>
</thead>
<tbody>
<tr>
<td>AliyunECSFullAccess</td>
<td> Permissions to manage ECS </td>
</tr>
<tr>
<td>AliyunVPCFullAccess</td>
<td> Permissions for managing VPC networks </td>
</tr>
<tr>
<td>AliyunROSFullAccess</td>
<td> Manage permissions for Resource Orchestration Services (ROS) </td>
</tr>
<tr>
<td>AliyunComputeNestUserFullAccess</td>
<td> Manage user-side permissions for the compute nest service (ComputeNest) </td>
</tr>
<tr>
<td>AliyunCloudMonitorFullAccess</td>
<td> Permissions to manage CloudMonitor (CloudMonitor) </td>
</tr>
</tbody>
</table>

<h2> Select ECS instance deployment </h2>

<p> Select ECS instance deployment to support Linux OS. </p>

<h3> Prerequisites </h3>

<ol>
<li> The selected ECS instance can access the Internet </li>
<li> The selected ECS instance is running. If the instance has just started, wait a moment. </li>
<li> System compatibility: Alibaba Cloud Linux 3.2104 LTS/CentOS 7.7/CentOS 7.8/CentOS 7.9/Ubuntu 20.04/Ubuntu 22.04</li>
</ol>

<h3> Operation steps </h3>

<ol>
<li> Click <a href = "https://computenest.console.aliyun.com/service/instance/create/default?type=user&ServiceName=Python%E8%BF%90%E8%A1%8C%E7%8E%AF%E5%A2%83"> Deployment Link </a> to go to the Service Instance Deployment page. </li>
<li> Select the target ECS instance and click Next: Confirm Order.
<img src="1.jpg" width="100%" align="bottom"/></li>
<li> Click Create Now and wait for the service instance to be created. After the service instance is created, go to the service instance details page. You can obtain installation logs on the Overview page.
<img src="2.jpg" width="100%" align="bottom"/></li>
</ol>

<h2> Create ECS instance deployment </h2>

<p> The new ECS instance supports the Linux operating system. </p>

<h3> Operation steps </h3>

<ol>
<li> Click <a href = "https://computenest.console.aliyun.com/service/instance/create/default?type=user&ServiceName=Python%E8%BF%90%E8%A1%8C%E7%8E%AF%E5%A2%83"> Deployment Link </a> to go to the Service Instance Deployment page. </li>
<li> Select the new ECS instance and configure the parameters according to the interface prompts. After the configuration is complete, click Next: Confirm Order.
<img src="3.jpg" width="100%" align="bottom"/></li>
<li> Click Create Now and wait for the service instance to be created. After the service instance is created, go to the service instance resource page.
<img src="4.jpg" width="100%" align="bottom"/></li>
<li><p> Run the command on the ECS instance to view the Python3 installation results. </p>

<div class="codehilite">
<pre><span></span><code>python3<span class="w"> </span>-v
</code></pre>
</div>

<p><img src="5.jpg" width="100%" align="bottom"/></p></li>
</ol>
