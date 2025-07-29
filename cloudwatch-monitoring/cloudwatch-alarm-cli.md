# CloudWatch Alarm CLI

```bash
aws cloudwatch put-metric-alarm   --alarm-name "High-CPU-Utilization"   --metric-name CPUUtilization   --namespace AWS/EC2   --statistic Average   --period 300   --threshold 80   --comparison-operator GreaterThanThreshold   --dimensions Name=InstanceId,Value=i-xxxxxxxxxxxxxxxxx   --evaluation-periods 2   --alarm-actions arn:aws:sns:us-east-1:123456789012:MyTopic   --unit Percent
```