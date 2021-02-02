# Axeleranttest_2


#3 Demonstrate how you can alert a support team when instance or server RAM usage is greater than 60%, disk space usage is greater than 80%, or CPU usage greater than 70%.


# AWS CloudWatch, as we know, is a powerful service provided by Amazon for monitoring and managing our AWS services. It provides us with data and actionable insights which we can use to monitor our application/websites, understand and respond to critical changes, optimise resource utilisation and get a consolidated view of the entire account.

CloudWatch collects monitoring and operational information in the form of logs, metrics, and events.


#Use these steps to use the AWS Management Console to create a CPU usage alarm.

To create an alarm based on CPU usage
---------------------------------------

1. Open the CloudWatch console
2. In the navigation pane, choose Alarms, Create Alarm.

3. Choose Select metric.

4. In the All metrics tab, choose EC2 metrics.

5. Choose a metric category (for example, Per-Instance Metrics).

6. Find the row with the instance that you want listed in the InstanceId column and CPUUtilization in the Metric Name column. Select the check box next to this row, and choose Select metric.

7. Under Specify metric and conditions, for Statistic choose Average, choose one of the predefined percentiles, or specify a custom percentile

8. Choose a period (for example, 5 minutes).

  Under Conditions, specify the following:

  For Threshold type, choose Static.

  For Whenever CPUUtilization is, specify Greater. Under than..., specify the threshold that is to trigger the alarm to go to ALARM state if the CPU utilization exceeds this percentage. For example, 70.
  
 9. Choose Next.

10. Under Notification, choose In alarm and select an SNS topic to notify when the alarm is in ALARM state

11. To have the alarm send multiple notifications for the same alarm state or for different alarm states, choose Add notification.

12. To have the alarm not send notifications, choose Remove.

13. When finished, choose Next.

14. Enter a name and description for the alarm. The name must contain only ASCII characters. Then choose Next.

15. Under Preview and create, confirm that the information and conditions are what you want, then choose Create alarm. 
  
  
  
