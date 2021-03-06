# Robot Monitoring<a name="gs-robotmonitoring"></a>

This section shows how to monitor health and operational metrics for a robot in a simulated bookstore using Amazon CloudWatch Metrics and Amazon CloudWatch Logs\. The streams metrics including speed, distance to nearest obstacle, distance to current goal, robot CPU utilization, and RAM usage\. 

Before you use AWS RoboMaker for the first time, complete the tasks in [Create an Account](gs-set-up.md)\. Then, in the AWS RoboMaker console, launch the Robot Monitoring sample application\.

**Topics**
+ [View Robot Health and Performance Metrics](#gs-robotmonitoring-metrics)
+ [View CloudWatch Logs](#gs-robotmonitoring-logs)

## View Robot Health and Performance Metrics<a name="gs-robotmonitoring-metrics"></a>

The Robot Monitoring sample application uses AWS RoboMaker cloud extensions to write custom health and performance metrics to Amazon CloudWatch\.

**To view robot health and performance metrics**

1. Open the CloudWatch console at [https://console\.aws\.amazon\.com/cloudwatch/](https://console.aws.amazon.com/cloudwatch/)\.

1. In the CloudWatch console, select **Metrics**\. 

1. On the **Metrics** page, in the **All metrics** tab, select the Robot Monitoring example\. 

1. On the **Metrics** page, in the **All metrics** tab, select **Robot**\. These are the operational metrics for the robot\. 

1. Select all of the metrics\. Each metric will appear on the graph in a different color\. 

1. Hover over the graph to see values for that moment\. You can also select a region on the graph to zoom in or select **custom** at the top of the page to select a custom time period\.

## View CloudWatch Logs<a name="gs-robotmonitoring-logs"></a>

When a simulation job runs, logs are generated by simulation tools and the applications in the simulation job\.

**To view the logs**

1. Open the CloudWatch console at [https://console\.aws\.amazon\.com/cloudwatch/](https://console.aws.amazon.com/cloudwatch/)\.

1. In the CloudWatch console, select **Logs**\. 

1. On the **Log groups** page, select the Robot Monitoring **Log Group**, and then select **Turtlebot3**\. 

1. Select an event to see details\. For example, if you filter for **monitor\_obstacle\_distance** events, you can see the distance to the nearest obstacle at that moment\. 