当请求或完成工作流程运行时，将发生此事件，并允许您基于另一个工作流程的完成结果执行工作流程。 无论上一个工作流程的结果如何，工作流程运行都会被触发。

例如，如果 `pull_request` 工作流程生成构件，您可以创建一个使用 `workflow_run` 来分析结果的新工作流程，并向原始拉取请求添加注释。

由 `workflow_run` 事件启动的工作流程能够访问密钥和写入令牌，即使以前的工作流程不能访问也一样。 这在以前的工作流程有意未获权限的情况下很有用，但您需要在以后的工作流程中采取特权行动。