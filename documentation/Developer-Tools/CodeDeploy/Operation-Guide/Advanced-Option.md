## 部署组高级选项

**同名文件策略**

设置在部署/回滚时，同目录内的同名文件如何处理。现支持三种方式：使部署失败，即若出现同名文件，即标志部署失败；覆盖，即用新文件替换原有的重名文件；保留，即保留原有的重名文件，不进行替换。

默认选项：覆盖

**通知频率与方式**

- 通知频率：单选通知触发的条件，仅部署异常发送、每次部署都发送、不通知。若选择前两项，那么，当满足通知条件时，将按照已选的通知方式进行通知。
- 通知方式：多选，消息、邮件、短信。

默认选项：不通知

**自动回滚**

可设置当部署失败时是否触发自动回滚，将回滚至上一个部署成功的版本。

默认选项：否


![Alt text](https://github.com/jdcloudcom/cn/blob/codedeploy/image/CodeDeploy/operation12.png)
