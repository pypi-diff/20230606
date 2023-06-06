# Comparing `tmp/awsibox-0.8.0.tar.gz` & `tmp/awsibox-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.0.tar", last modified: Thu Apr 27 10:31:11 2023, max compression
+gzip compressed data, was "awsibox-0.8.2.tar", last modified: Tue Jun  6 14:36:27 2023, max compression
```

## Comparing `awsibox-0.8.0.tar` & `awsibox-0.8.2.tar`

### file list

```diff
@@ -1,281 +1,280 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.0/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.0/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-04-27 10:31:11.129942 awsibox-0.8.0/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.0/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.025940 awsibox-0.8.0/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    17889 2023-04-27 10:00:09.000000 awsibox-0.8.0/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-04-27 10:30:14.000000 awsibox-0.8.0/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.0/awsibox/args.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3755 2023-02-20 15:00:23.000000 awsibox-0.8.0/awsibox/autoscaling.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.025940 awsibox-0.8.0/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.057941 awsibox-0.8.0/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      637 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1811 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.069941 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1398 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6819 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      977 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.069941 awsibox-0.8.0/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.073941 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      365 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      251 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.073941 awsibox-0.8.0/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.077941 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2067 2023-04-27 10:06:22.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.077941 awsibox-0.8.0/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      165 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1764 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2937 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2442 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3101 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     4759 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      955 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      426 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1018 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     6608 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1986 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5166 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     3972 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2920 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     2287 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2300 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7723 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      357 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7683 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8101 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      397 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1751 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      311 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4591 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3433 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      846 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2510 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      621 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      240 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.113942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3527 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      595 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4700 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       67 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2157 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.113942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2490 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    16432 2023-04-27 10:25:15.000000 awsibox-0.8.0/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.8.0/awsibox/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2324 2023-01-17 08:49:47.000000 awsibox-0.8.0/awsibox/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.0/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13204 2023-02-09 13:53:52.000000 awsibox-0.8.0/awsibox/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/ecr.py
--rw-r--r--   0 mello     (1000) mello     (1000)      922 2023-02-09 16:43:35.000000 awsibox-0.8.0/awsibox/ecs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.8.0/awsibox/efs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.8.0/awsibox/elasticloadbalancing.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2418 2023-04-17 07:28:21.000000 awsibox-0.8.0/awsibox/generate.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3369 2023-04-14 07:54:55.000000 awsibox-0.8.0/awsibox/iam.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2784 2023-04-11 16:23:54.000000 awsibox-0.8.0/awsibox/joker.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.0/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.0/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.0/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.0/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.0/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.0/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.0/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.0/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.0/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.0/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.0/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.0/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5132 2023-04-12 16:00:53.000000 awsibox-0.8.0/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.0/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.0/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.0/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.0/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.0/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2126 2022-12-22 11:51:40.000000 awsibox-0.8.0/awsibox/lambdas/StacksOps.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.8.0/awsibox/mappings.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.8.0/awsibox/rds.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.8.0/awsibox/s3.py
--rw-r--r--   0 mello     (1000) mello     (1000)    45456 2023-04-17 09:53:49.000000 awsibox-0.8.0/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.0/awsibox/user-data/ecs-cluster.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/waf.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.017940 awsibox-0.8.0/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     8974 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3177 2023-04-27 09:19:18.000000 awsibox-0.8.0/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-04-27 10:31:11.129942 awsibox-0.8.0/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      506 2023-04-27 09:19:18.000000 awsibox-0.8.0/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.244610 awsibox-0.8.2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.2/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.2/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-06 14:36:27.244610 awsibox-0.8.2/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.2/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.152608 awsibox-0.8.2/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19179 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-06 14:34:45.000000 awsibox-0.8.2/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.2/awsibox/args.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3755 2023-02-20 15:00:23.000000 awsibox-0.8.2/awsibox/autoscaling.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.152608 awsibox-0.8.2/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.140608 awsibox-0.8.2/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.188609 awsibox-0.8.2/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1811 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.192609 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.196609 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1441 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6945 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      931 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.196609 awsibox-0.8.2/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      365 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      251 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.200609 awsibox-0.8.2/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      165 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.140608 awsibox-0.8.2/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.204609 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1764 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2937 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2442 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3101 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4759 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      955 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.208609 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      426 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1018 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     9845 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.212609 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3972 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.216609 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2287 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2444 2023-05-20 09:12:43.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      357 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7683 2023-05-02 08:15:00.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8101 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.220610 awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      397 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.144608 awsibox-0.8.2/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1751 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      311 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3433 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.224609 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2510 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.228610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.228610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      240 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.232610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3527 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      595 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4700 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       67 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2157 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.232610 awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2490 2023-06-05 15:35:41.000000 awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    16593 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.8.2/awsibox/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2332 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.2/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    13278 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-04-27 09:19:18.000000 awsibox-0.8.2/awsibox/ecr.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.8.2/awsibox/efs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.8.2/awsibox/elasticloadbalancing.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2409 2023-06-06 14:34:34.000000 awsibox-0.8.2/awsibox/generate.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3369 2023-04-14 07:54:55.000000 awsibox-0.8.2/awsibox/iam.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2942 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/joker.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.2/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.2/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.2/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.2/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.2/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.2/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.2/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.2/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.2/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.2/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.2/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.2/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5327 2023-05-18 13:11:03.000000 awsibox-0.8.2/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.2/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.2/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.2/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.2/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.2/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.2/awsibox/lambdas/StacksOps.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.8.2/awsibox/mappings.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.8.2/awsibox/rds.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.8.2/awsibox/s3.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    45530 2023-06-06 14:25:53.000000 awsibox-0.8.2/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.2/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.2/awsibox/user-data/ecs-cluster.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.8.2/awsibox/waf.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.132608 awsibox-0.8.2/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.148608 awsibox-0.8.2/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     8959 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-06 14:36:26.000000 awsibox-0.8.2/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-06 14:36:27.240610 awsibox-0.8.2/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3177 2023-04-27 09:19:18.000000 awsibox-0.8.2/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-06 14:36:27.244610 awsibox-0.8.2/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      506 2023-04-27 09:19:18.000000 awsibox-0.8.2/setup.py
```

### Comparing `awsibox-0.8.0/.gitignore` & `awsibox-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/PKG-INFO` & `awsibox-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.0
+Version: 0.8.2
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.0/awsibox/RP.py` & `awsibox-0.8.2/awsibox/RP.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,51 +6,73 @@
 import json
 import logging
 from pprint import pprint, pformat
 
 from . import cfg
 
 
-def RP_to_cfg(key, prefix="", overwrite=True, mappedvalues=[]):
+def inject_in_RP_map(key_name, value):
+    for n, v in cfg.Mappings.items():
+        for m, w in v.items():
+            if key_name not in w:
+                w[key_name] = value
+
+
+def RP_to_cfg(key, prefix="", overwrite=True, mappedvalues=[], check_mapped=False):
     if hasattr(key, "items"):
         for k, v in key.items():
             # remove both * and + that can be present for special IBOX usage
             key_name = f"{prefix}{k}".translate("".maketrans({"*": None, "+": None}))
             try:
                 getattr(cfg, key_name)
                 exist = True
             except Exception:
                 exist = False
             if not exist or overwrite:
                 setattr(cfg, key_name, v)
                 if key_name not in mappedvalues:
                     cfg.fixedvalues[key_name] = v
+                elif check_mapped:
+                    # key_name is in mapped value and i need to check that cfg.Mappings is complete (Ex. IBOX_SOURCE_OBJ)
+                    inject_in_RP_map(key_name, v)
             # recursively traverse dict
             # keys name are the concatenation of traversed dict keys
             if isinstance(v, dict):
                 for j, w in v.items():
-                    RP_to_cfg({f"{k}{j}": w}, prefix, overwrite)
+                    if j == cfg.IBOX_BASE_KEY_NAME:
+                        # avoid creating cfg entries for IBOX_BASE keys
+                        continue
+                    RP_to_cfg(
+                        {f"{k}{j}": w},
+                        prefix,
+                        overwrite,
+                        mappedvalues=mappedvalues,
+                        check_mapped=check_mapped,
+                    )
 
 
-def merge_dict(base, work):
+def merge_dict(base, work, keep=False):
     if isinstance(work, (str, list)) or not base:
         return work
     keys = dict(list(base.items()) + list(work.items())).keys()
     for k in keys:
         if k.endswith("**"):
             # ** is used to replace existing dict instead of merging it
             base[k.replace("**", "")] = work[k]
         elif isinstance(base.get(k), dict) and isinstance(work.get(k), dict):
-            base[k] = merge_dict(base[k], work[k])
+            base[k] = merge_dict(base[k], work[k], keep=keep)
         elif k.endswith("++") and isinstance(work.get(k), list):
             # ++ is used to append elements to an existing key
             try:
                 base[k.replace("++", "")] += work[k]
             except Exception:
                 base[k.replace("++", "")] = work[k]
+        elif k in base and keep:
+            # key is in base and want to keep that value
+            pass
         elif k in work:
             base[k] = work[k]
     return base
 
 
 def build_RP():
     LD_INCLUDED = []
@@ -264,15 +286,15 @@
                 cfg = yaml.load(ymlfile, Loader=Loader)
 
                 return cfg
         except IOError:
             return {}
 
     def inject_ibox_base(RP, root=""):
-        base_key = "IBOX_BASE"
+        base_key = cfg.IBOX_BASE_KEY_NAME
         for main_key in list(RP.keys()):
             main_key_full = f"{root}{main_key}"
             main_key_value = RP[main_key]
             if isinstance(main_key_value, dict) and base_key in main_key_value:
                 base_key_value = main_key_value[base_key]
                 base_key_value["IBOX_BASE_REF"] = True
 
@@ -292,15 +314,21 @@
                     # inject in existing structure
                     merged = merge_dict(
                         copy.deepcopy(base_key_value), resource_key_value
                     )
                     # need to do it this way to keep the "link" between existing dict keys and values
                     for n, v in merged.items():
                         RP[main_key][resource_key][n] = v
+                # delete IBOX_BASE in RP structure..
                 del RP[main_key][base_key]
+                # ..and in cfg one
+                try:
+                    del getattr(cfg, f"{root}{main_key}")[base_key]
+                except Exception:
+                    pass
 
             if isinstance(main_key_value, dict):
                 inject_ibox_base(main_key_value, root=main_key_full)
 
     def get_RP(yaml_cfg):
         cfg_keys = ["IBoxLoader", "IBoxLoaderAfter"]
 
@@ -439,14 +467,18 @@
         pprint(LD_EXCLUDED)
         print("########## EXCLUDED ####### END #######")
 
         print("########## INCLUDED ####### START #####")
         pprint(LD_INCLUDED)
         print("########## INCLUDED ####### END #######")
 
-        print("########## FIXEDVALUES ######### START #####")
+        print("########## FIXED_VALUES ######### START #####")
         pprint(cfg.fixedvalues)
-        print("########## FIXEDVALUES ######### END #######")
+        print("########## FIXED_VALUES ######### END #######")
+
+        print("########## MAPPED_VALUES ######### START #####")
+        pprint(cfg.mappedvalues)
+        print("########## MAPPED_VALUES ######### END #######")
 
-        print("########## MAPPEDVALUES ######### START #####")
+        print("########## RP_MAP ######### START #####")
         pprint(cfg.RP_map)
-        print("########## MAPPEDVALUES ######### END #######")
+        print("########## RP_MAP ######### END #######")
```

### Comparing `awsibox-0.8.0/awsibox/args.py` & `awsibox-0.8.2/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/autoscaling.py` & `awsibox-0.8.2/awsibox/autoscaling.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.8.2/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/common.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files 5% similar despite different names*

```diff
@@ -15,21 +15,14 @@
         get_condition('', 'equals', 'yes', 'DaemonReserveCpu')
   Output:
     - ClusterStack:
         Value: Ref("AWS::StackName")
     - DaemonReserveCpu:
         Value: get_endvalue('DaemonReserveCpu')
   DaemonReserveCpu: 'no'
-  ContainerDefinitions:
-    - ReserveCpu:
-        Command: ['tail', '-f']
-        Cpu: 512
-        Image: 'busybox'
-        LogConfiguration: IBOX_SKIP_FUNC
-        Memory: 32
   EC2SecurityGroup:
     - EcsService:
         IBOX_ENABLED: False
   # Included yaml ecs/task.yml have changed ParameterStore Roles to RoleTask, need to restore it.
   IAMPolicy:
     - ParameterStore:
         Roles:
@@ -48,7 +41,15 @@
         Cluster: Ref('Cluster')
         LoadBalancers: IBOX_SKIP_FUNC
         NetworkConfiguration: IBOX_SKIP_FUNC
         Role: Ref("AWS::NoValue")
   ECSTaskDefinition:
     - Base:
         Condition: DaemonReserveCpu
+        ContainerDefinitions:
+          - ReserveCpu:
+              Command: ['tail', '-f']
+              Cpu: 512
+              Image: 'busybox'
+              LogConfiguration: IBOX_SKIP_FUNC
+              Memory: 32
+
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files 4% similar despite different names*

```diff
@@ -87,27 +87,27 @@
         IBOX_NO_OUTPUT: True
         SecurityGroupIngress:
           - External:
               IBOX_IF:
                 - LoadBalancerApplicationExternal
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
-              FromPort: get_endvalue("ContainerDefinitions1ContainerPort")
+              FromPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
               IpProtocol: tcp
               SourceSecurityGroupId: ImportValue("SecurityGroupLoadBalancerApplicationExternal")
-              ToPort: get_endvalue("ContainerDefinitions1ContainerPort")
+              ToPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
           - Internal:
               IBOX_IF:
                 - LoadBalancerApplicationInternal
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
-              FromPort: get_endvalue("ContainerDefinitions1ContainerPort")
+              FromPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
               IpProtocol: tcp
               SourceSecurityGroupId: ImportValue("SecurityGroupLoadBalancerApplicationInternal")
-              ToPort: get_endvalue("ContainerDefinitions1ContainerPort")
+              ToPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
   EC2SecurityGroupIngress:
     - LoadBalancerApplicationHttpExternal:
         IBOX_ENABLED: False
         CidrIp: '0.0.0.0/0'
         GroupId: get_expvalue('SecurityGroupLoadBalancerApplicationExternal', 'LoadBalancerApplicationStack')
         FromPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpExternalPort')
         ToPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpExternalPort')
@@ -155,18 +155,18 @@
         LoadBalancers:
           - External:
               IBOX_IF:
                 - LoadBalancerApplicationExternal
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
               ContainerName: Ref('EnvRole')
-              ContainerPort: get_endvalue('ContainerDefinitions1ContainerPort')
+              ContainerPort: get_endvalue('ECSTaskDefinitionBaseContainerDefinitions1ContainerPort')
               TargetGroupArn: Ref('TargetGroupExternal')
           - Internal:
               IBOX_IF:
                 - LoadBalancerApplicationInternal
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
               ContainerName: Ref('EnvRole')
-              ContainerPort: get_endvalue('ContainerDefinitions1ContainerPort')
+              ContainerPort: get_endvalue('ECSTaskDefinitionBaseContainerDefinitions1ContainerPort')
               TargetGroupArn: Ref('TargetGroupInternal')
         Role: If("ECSServiceDoNotNeedRole", Ref("AWS::NoValue"), ImportValue("RoleECSService"))
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 global:
   Parameter:
     - ClusterStack:
         Description: 'Cluster Stack Name used to launch service on - empty for default based on env/role'
     - DockerLabelLastUpdate:
         Description: 'Use to force redeploy - can use: $(date +%F_%T)'
-  Condition:
-    - ECSTaskDefinitionBaseUseOneContainer:
-        Equals(1, len(cfg.ContainerDefinitions))
   Output:
     - ClusterStack:
         Value: get_endvalue('ClusterStack')
   ClusterStack: ecs-a
+  ECSTaskDefinition:
+    - Base:
+        IBOX_ENABLED: True
   LogsLogGroup:
     - Base:
         IBOX_TITLE: LogsLogGroup
         LogGroupName: Sub('/aws/ecs/${AWS::StackName}')
         RetentionInDays: 30
   IAMPolicy:
     - ParameterStore:
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
                   - 's3:Put*'
                   - 'iam:PassRole'
                   - 'iam:ListServerCertificates'
                   - 'iam:GetRole'
                   - 'iam:PutRolePolicy'
                   - 'iam:GetInstanceProfile'
                   - 'elasticloadbalancing:*'
+                  - 'application-autoscaling:*'
                   - 'ec2:*'
                   - 'ecs:*'
                   - 'ecr:*'
                   - 'sqs:*'
                   - 'sns:*'
                   - 'cloudwatch:*'
                   - 'autoscaling:*'
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/s3/bucket-log.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/services.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/ecs/services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/efs/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,20 @@
   IBOX_PARAMETER:
     - ElastiCacheReplicationGroup.IBOX_INDEXNAME.AutomaticFailoverEnabled:
         Description: 'Multi-AZ is enabled for this replication group (only for redis and ReplicationGroup) - empty for default based on env/role'
         AllowedValues: ['', 'true', 'false']
     - ElastiCacheCacheCluster.IBOX_INDEXNAME.CacheNodeType:
         Description: 'Node Type - empty for default based on env/role'
         AllowedValues: [
-          '', 'cache.t2.micro', 'cache.t2.small', 'cache.t2.medium', 'cache.t2.large',
-          'cache.m3.medium', 'cache.m3.large', 'cache.m3.xlarge', 'cache.m3.2xlarge',
-          'cache.m4.large', 'cache.m4.xlarge', 'cache.m4.2xlarge', 'cache.m4.4xlarge', 'cache.m4.10xlarge',
-          'cache.r3.large', 'cache.r3.xlarge', 'cache.r3.2xlarge', 'cache.r3.4xlarge', 'cache.r3.8xlarge',
+          '', 'cache.t3.micro', 'cache.t3.small', 'cache.t3.medium',
+          'cache.t4g.micro', 'cache.t4g.small', 'cache.t4g.medium',
+          'cache.m5.large', 'cache.m5.xlarge', 'cache.m5.2xlarge',
+          'cache.m5.4xlarge', 'cache.m5.12xlarge', 'cache.m5.24xlarge',
+          'cache.m6g.large', 'cache.m6g.xlarge', 'cache.m6g.2xlarge',
+          'cache.m6g.4xlarge', 'cache.m6g.8xlarge', 'cache.m6g.12xlarge', 'cache.m6g.16xlarge',
         ]
     - CacheEnabled:
         Description: 'Enable or disable cache creation'
         AllowedValues: [ 'yes', 'no']
         Default: 'yes'
     - ElastiCacheCacheCluster.IBOX_INDEXNAME.Engine:
         Description: 'Engine - empty for default based on env/role'
@@ -79,14 +81,15 @@
   AutoMinorVersionUpgrade: true
   NumCacheNodes: 1
 
 ReplicationGroup: &replication-group
   Condition: ReplicationGroup
   AutomaticFailoverEnabled: false
   CacheNodeType.IBOX_CODE: get_endvalue(f"ElastiCacheCacheCluster{IBOX_INDEXNAME}CacheNodeType")
+  CacheParameterGroupName: get_endvalue(f"ElastiCacheCacheCluster{IBOX_INDEXNAME}CacheParameterGroupName")
   Enabled: 'no'
   Engine.IBOX_CODE: get_endvalue(f"ElastiCacheCacheCluster{IBOX_INDEXNAME}Engine")
   EngineVersion.IBOX_CODE: get_endvalue(f"ElastiCacheCacheCluster{IBOX_INDEXNAME}EngineVersion")
   NumCacheClusters: 1
   ReplicationGroupDescription: 'Redis ReplicaGroup'
   ## Internal
   SecurityGroupIds: [Ref('SecurityGroupCCH')]
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,14 @@
         Targets:
           - ServiceUnavailable:
               Id: get_expvalue(f'LambdaServiceUnavailableArn')
         TargetType: lambda
     - ECSLoadBalancerApplicationExternal:
         IBOX_ENABLED: False
         <<: *base
-        Port: get_endvalue('ContainerDefinitions1ContainerPort')
+        Port: get_endvalue('ECSTaskDefinitionBaseContainerDefinitions1ContainerPort')
         TargetType: If('ECSTaskDefinitionBaseNetworkModeAwsVpc', 'ip', Ref('AWS::NoValue'))
     - ECSLoadBalancerApplicationInternal:
         IBOX_ENABLED: False
         <<: *base
-        Port: get_endvalue('ContainerDefinitions1ContainerPort')
+        Port: get_endvalue('ECSTaskDefinitionBaseContainerDefinitions1ContainerPort')
         TargetType: If('ECSTaskDefinitionBaseNetworkModeAwsVpc', 'ip', Ref('AWS::NoValue'))
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files 12% similar despite different names*

```diff
@@ -57,12 +57,13 @@
           Type: Base
           Conf:
             IBOX_RESNAME: LambdaLayerPermission.IBOX_INDEXNAME
             IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
         IBOX_OUTPUT:
           - _:
               Value: Ref(IBOX_RESNAME)
-        # Uncomment to retain previous layerversion
+        # Uncomment to retain previous layerversion possible values (Retain|Delete)
+        # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-attribute-updatereplacepolicy.html
         #UpdateReplacePolicy: Retain
         Content:
           S3Key.IBOX_AUTO_PO:
             Description: str(f"S3Key Name for lambda {IBOX_INDEXNAME} Content")
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,16 @@
           - IBOX_MAPNAME.PerformanceInsights:
               Description: 'The amount of time, in days, to retain Performance Insights data - empty for mapped value - 0 to disable'
           - IBOX_MAPNAME.StorageType:
               Description: 'empty for mapped value'
               AllowedValues: ['', 'standard', 'io1', 'gp2', 'gp3']
           - IBOX_MAPNAME.StorageThroughput:
               Description: 'empty for mapped value'
+          - IBOX_MAPNAME.Iops:
+              Description: 'empty for mapped value'
         IBOX_CONDITION:
           - IBOX_MAPNAME.DBSnapshotIdentifier:
               get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}DBSnapshotIdentifier')
           - IBOX_MAPNAME.SourceDBInstanceIdentifier:
               get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}SourceDBInstanceIdentifier')
           - IBOX_MAPNAME.DBInstanceSkipProperties:
               Or(Condition(f'{IBOX_MAPNAME}DBSnapshotIdentifier'), Condition(f'{IBOX_MAPNAME}SourceDBInstanceIdentifier'))
@@ -85,14 +87,16 @@
               get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MonitoringInterval')
           - IBOX_MAPNAME.PerformanceInsights:
               get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}PerformanceInsights')
           - IBOX_MAPNAME.StorageAutoScaling:
               get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MaxAllocatedStorage')
           - IBOX_MAPNAME.StorageThroughput:
               get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}StorageThroughput')
+          - IBOX_MAPNAME.Iops:
+              get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}Iops')
         IBOX_OUTPUT:
           - IBOX_MAPNAME.AllocatedStorage:
               Value: ${AllocatedStorage}
           - IBOX_MAPNAME.MaxAllocatedStorage:
               Value: ${MaxAllocatedStorage}
           - IBOX_MAPNAME.DBInstanceClass:
               Value: ${DBInstanceClass}
@@ -118,23 +122,28 @@
               Value: ${PubliclyAccessible}
           - IBOX_MAPNAME.SourceDBInstanceIdentifier:
               Value: ${SourceDBInstanceIdentifier}
           - IBOX_MAPNAME.StorageType:
               Value: ${StorageType}
           - IBOX_MAPNAME.StorageThroughput:
               Value: ${StorageThroughput}
+          - IBOX_MAPNAME.Iops:
+              Value: ${Iops}
         AllocatedStorage: 50
         AllowMajorVersionUpgrade: true
         DBInstanceClass: db.t3.micro
         DBName: dbname
         DBParameterGroupName: Ref('DBParameterGroup1')
         DBSnapshotIdentifier: none
         DeletionProtection: false
         EnablePerformanceInsights:
           If(f'{IBOX_MAPNAME}PerformanceInsights', True, False)
+        Iops.IBOX_CODE:
+          If(f'{IBOX_MAPNAME}Iops', get_endvalue(f'{IBOX_MAPNAME}Iops'), Ref('AWS::NoValue'))
+        Iops: 0
         MasterUsername: masterusername
         MasterUserPassword: masteruserpassword
         MaxAllocatedStorage: 0
         MaxAllocatedStorage.IBOX_CODE:
           If(f'{IBOX_MAPNAME}StorageAutoScaling', get_endvalue(f'{IBOX_MAPNAME}MaxAllocatedStorage'), Ref('AWS::NoValue'))
         MonitoringInterval: 0
         MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', get_expvalue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/s3/bucket-policies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/s3/bucket-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/s3/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files 3% similar despite different names*

```diff
@@ -109,20 +109,20 @@
     - Data:
         BlockDeviceMappings:
           - Xvda:
               Ebs:
                 VolumeSize: 30
         ImageIdLatest.IBOX_AUTO_PO:
           Description: 'Latest ecs ami available from SSM'
-          Default: '/aws/service/ecs/optimized-ami/amazon-linux-2/recommended/image_id'
+          Default: '/aws/service/ecs/optimized-ami/amazon-linux-2023/recommended/image_id'
           AllowedValues:
+            - '/aws/service/ecs/optimized-ami/amazon-linux-2023/recommended/image_id'
             - '/aws/service/ecs/optimized-ami/amazon-linux/recommended/image_id'
             - '/aws/service/ecs/optimized-ami/amazon-linux-2/recommended/image_id'
             - '/aws/service/ecs/optimized-ami/amazon-linux-2/arm64/recommended/image_id'
-            - '/aws/service/ecs/optimized-ami/amazon-linux-2022/recommended/image_id'
             - '/aws/service/bottlerocket/aws-ecs-1/x86_64/latest/image_id'
             - '/aws/service/bottlerocket/aws-ecs-1/arm64/latest/image_id'
   Listeners: []
   RecordSet: []
   IAMRole:
     - Instance:
         ManagedPolicyArns++:
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files 15% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 global:
   StackName: bkt
   ApplicationAutoScalingScalingPolicy: IBOX_SKIP_FUNC
   Capacity:
     Desired: 3
     Max: 4
     Min: 3
-  ContainerDefinitions:
-    - 1:
-        Cpu: 128
-        Environment:
+  ECSTaskDefinition:
+  - Base:
+      Volumes:
+      - DockerSock:
+          Name: DockerSock
+          Host:
+            SourcePath: /var/run/docker.sock
+      ContainerDefinitions:
+      - 1:
+          Cpu: 128
+          Environment:
           - AWSDEFAULTREGION:
               Name: AWS_DEFAULT_REGION
               Value: Ref('AWS::Region')
-        Memory: 128
-        MountPoints:
+          Memory: 128
+          MountPoints:
           - DockerSock:
               ReadOnly: false
               SourceVolume: DockerSock
               ContainerPath: /var/run/docker.sock
-  ECSTaskDefinition:
-    - Base:
-        Volumes:
-          - DockerSock:
-              Name: DockerSock
-              Host:
-                SourcePath: '/var/run/docker.sock'
+
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,20 @@
   - res/cloudwatch/alarms.yml
 
 global:
   StackName: rsc
   ApplicationAutoScalingScalableTarget: IBOX_SKIP_FUNC
   ApplicationAutoScalingScalingPolicy: IBOX_SKIP_FUNC
   CloudWatchAlarm: IBOX_SKIP_FUNC
-  ContainerDefinitions:
-    - 1:
-        Command: ['tail', '-f', '.dockerenv']
-        Cpu: 512
-        Image: 'amazonlinux:2'
-        Memory: 64
   ECSService:
     - Base:
         IBOX_ENABLED: False
     - Daemon:
         IBOX_ENABLED: True
+  ECSTaskDefinition:
+    - Base:
+        ContainerDefinitions:
+          - 1:
+              Command: ['tail', '-f', '.dockerenv']
+              Cpu: 512
+              Image: 'amazonlinux:2'
+              Memory: 64
```

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/vpc.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.8.2/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cfg.py` & `awsibox-0.8.2/awsibox/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 PATH_INT = os.path.join(APP_DIR, "cfg")
 PATH_INT = os.path.normpath(PATH_INT)
 
 PATH_EXT = os.path.join(cwd, "cfg")
 PATH_EXT = os.path.normpath(PATH_EXT)
 
+IBOX_BASE_KEY_NAME = "IBOX_BASE"
+
 IBOX_BRAND_DIR = "ibox"
 STACKS_DIR = "stacks"
 
 STACK_TYPES = [
     "agw",
     "cch",
     "clf",
@@ -401,21 +403,25 @@
         "func": ("ecs", "ClusterCapacityProviderAssociations"),
     },
     "ECSService": {
         "module": "joker",
         "func": ("ecs", "Service"),
         "dep": ["SecurityGroups"],
     },
-    "ECSTaskDefinition": {"module": "ecs", "func": "ECS_TaskDefinition"},
+    "ECSTaskDefinition": {"module": "joker", "func": ("ecs", "TaskDefinition")},
     "EFSAccessPoint": {"module": "joker", "func": ("efs", "AccessPoint")},
     "EFSFileSystem": {"module": "efs", "func": "EFS_FileStorage"},
     "ElastiCacheCacheCluster": {
         "module": "joker",
         "func": ("elasticache", "CacheCluster"),
     },
+    "ElastiCacheParameterGroup": {
+        "module": "joker",
+        "func": ("elasticache", "ParameterGroup"),
+    },
     "ElastiCacheReplicationGroup": {
         "module": "joker",
         "func": ("elasticache", "ReplicationGroup"),
     },
     "ElastiCacheSubnetGroup": {
         "module": "joker",
         "func": ("elasticache", "SubnetGroup"),
```

### Comparing `awsibox-0.8.0/awsibox/cloudformation.py` & `awsibox-0.8.2/awsibox/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/cloudfront.py` & `awsibox-0.8.2/awsibox/cloudfront.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
                 del v[k]
             except Exception:
                 pass
 
 
 def cache_behavior_process(key):
     # process default behavior
-    process_cache_policy(
-        key["DefaultCacheBehavior"]
-    )
+    process_cache_policy(key["DefaultCacheBehavior"])
     # process other behaviors
     for n, v in key["CacheBehaviors"].items():
         process_cache_policy(v)
 
 
 def origin_process(name, key):
     for n, v in key["Origins"].items():
@@ -59,15 +57,17 @@
 
         # Automatically compute Behaviour Order based on PathPattern
         cfg.dbg_clf_compute_order = {}
         sortedcachebehaviors = sorted(
             distribution_config["CacheBehaviors"].items(),
             key=lambda x_y: clf_compute_order(x_y[1]["PathPattern"]),
         )
-        distribution_config["CacheBehaviors"] = {x[0]: x[1] for x in sortedcachebehaviors}
+        distribution_config["CacheBehaviors"] = {
+            x[0]: x[1] for x in sortedcachebehaviors
+        }
 
         if cfg.debug:
             print("##########CLF_COMPUTE_ORDER#########START#######")
             for n, v in iter(
                 sorted(cfg.dbg_clf_compute_order.items(), key=lambda x_y: x_y[1])
             ):
                 print(f"{n} {v}\n")
```

### Comparing `awsibox-0.8.0/awsibox/common.py` & `awsibox-0.8.2/awsibox/common.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/discover.py` & `awsibox-0.8.2/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/ec2.py` & `awsibox-0.8.2/awsibox/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,27 +146,31 @@
 def SG_SecurityGroupsECS(key):
     Out_String = ["Service=${SecurityGroupEcsService}"]
     Out_Map = {"SecurityGroupEcsService": {"Ref": "SecurityGroupEcsService"}}
 
     SecurityGroups = SG_SecurityGroupsExtra(Out_String, Out_Map)
     # add Condition to Output created by SG_SecurityGroupsExtra
     try:
-        cfg.Outputs["SecurityGroups"].Condition = "ECSTaskDefinitionBaseNetworkModeAwsVpc"
+        cfg.Outputs[
+            "SecurityGroups"
+        ].Condition = "ECSTaskDefinitionBaseNetworkModeAwsVpc"
     except Exception:
         pass
 
 
 def SG_SecurityGroupsTSK(key):
     Out_String = []
     Out_Map = {}
 
     SecurityGroups = SG_SecurityGroupsExtra(Out_String, Out_Map)
     # add Condition to Output created by SG_SecurityGroupsExtra
     try:
-        cfg.Outputs["SecurityGroups"].Condition = "ECSTaskDefinitionBaseNetworkModeAwsVpc"
+        cfg.Outputs[
+            "SecurityGroups"
+        ].Condition = "ECSTaskDefinitionBaseNetworkModeAwsVpc"
     except Exception:
         pass
 
 
 def SG_SecurityGroupRules(groupname, ingresses):
     SecurityGroup_Rules = []
     listeners_cfg = {}
@@ -271,15 +275,17 @@
             else:
                 raise ValueError
         except KeyError:
             # key SecurityGroupIngress do not exist
             pass
         except ValueError:
             # to_dict failed or SecurityGroupIngress is empty, populate it using SG_SecurityGroupRules
-            r_SG.SecurityGroupIngress = SG_SecurityGroupRules(mapname, v["SecurityGroupIngress"])
+            r_SG.SecurityGroupIngress = SG_SecurityGroupRules(
+                mapname, v["SecurityGroupIngress"]
+            )
 
         try:
             outname = v["OutputName"]
         except Exception:
             outname = resname
         else:
             outname = f"SecurityGroup{outname}"
```

### Comparing `awsibox-0.8.0/awsibox/ecr.py` & `awsibox-0.8.2/awsibox/ecr.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/efs.py` & `awsibox-0.8.2/awsibox/efs.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/elasticloadbalancing.py` & `awsibox-0.8.2/awsibox/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/generate.py` & `awsibox-0.8.2/awsibox/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from . import (
     __version__,
     autoscaling,
     cloudformation,
     cloudfront,
     ec2,
     ecr,
-    ecs,
     efs,
     iam,
     joker,
     elasticloadbalancing,
     mappings,
     rds,
     s3,
```

### Comparing `awsibox-0.8.0/awsibox/iam.py` & `awsibox-0.8.2/awsibox/iam.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/joker.py` & `awsibox-0.8.2/awsibox/joker.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,24 @@
 
         # use IBOX_SOURCE_OBJ to prepopulate obj
         ibox_source_obj = v.get("IBOX_SOURCE_OBJ", [])
         if isinstance(ibox_source_obj, str):
             ibox_source_obj = [ibox_source_obj]
         for source_obj in ibox_source_obj:
             source_obj = parse_ibox_key(source_obj, parse_ibox_key_conf)
-            source_obj_conf = getattr(cfg, source_obj)
-            RP_to_cfg(source_obj_conf, prefix=mapname, mappedvalues=cfg.mappedvalues)
-            v = merge_dict(v, source_obj_conf)
+            source_obj_conf = copy.deepcopy(getattr(cfg, source_obj))
+            RP_to_cfg(
+                source_obj_conf,
+                prefix=mapname,
+                overwrite=False,
+                mappedvalues=cfg.mappedvalues,
+                check_mapped=True,
+            )
+            v = merge_dict(v, source_obj_conf, keep=True)
+
             # Uncomment to use old method: auto_get_props
             # auto_get_props(obj, mapname=source_obj, indexname=n)
             # #reset obj title, if changed by IBOX_TITLE key
             # obj.title = resname
 
         # autocreate condition
         if v.get("Create"):
```

### Comparing `awsibox-0.8.0/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.2/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.2/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.8.2/awsibox/lambdas/CCRFargateSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.2/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.8.2/awsibox/lambdas/CCRStackReplicator.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.2/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.2/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.2/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.2/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.2/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.2/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.2/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.8.2/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.8.2/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.2/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.2/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.2/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/InfraInfo.code` & `awsibox-0.8.2/awsibox/lambdas/InfraInfo.code`

 * *Files 5% similar despite different names*

```diff
@@ -92,33 +92,38 @@
         )
         for s in response_iterator_service:
             if not s["serviceArns"]:
                 continue
             s_d = CLIENT_ECS.describe_services(
                 cluster=c,
                 services=s["serviceArns"],
+                include=["TAGS"],
             )["services"]
             for srv in s_d:
                 cluster_name = c.split("/")[-1]
-                ResourceId = f"service/{cluster_name}/" + srv["serviceName"]
+                service_name = srv["serviceName"]
+                ResourceId = f"service/{cluster_name}/{service_name}"
                 deploymentConf = srv["deploymentConfiguration"]
+                cluster_stack = cluster_name[0 : cluster_name.find("-Cluster-")]
+                stack = service_name[0 : service_name.find("-Service-")]
+                role = None
+                for r in srv["tags"]:
+                    if r["key"] == "EnvRole":
+                        role = r["value"]
+                        break
                 services_tdd.update(
                     {
                         ResourceId: {
-                            "cluster": cluster_name[0:7],
-                            "stack": srv["serviceName"][0:7],
+                            "cluster": cluster_stack,
+                            "stack": stack,
                             "desired": srv["desiredCount"],
                             "running": srv["runningCount"],
                             "pending": srv["pendingCount"],
                             "launchType": srv.get("launchType"),
-                            "role": (
-                                srv["loadBalancers"][0]["containerName"]
-                                if srv["loadBalancers"]
-                                else None
-                            ),
+                            "role": role,
                             "max%": deploymentConf["maximumPercent"],
                             "min%": deploymentConf["minimumHealthyPercent"],
                         }
                     }
                 )
                 resource_id_list.append(ResourceId)
```

### Comparing `awsibox-0.8.0/awsibox/lambdas/ManageService.code` & `awsibox-0.8.2/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.2/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/PyPackager.code` & `awsibox-0.8.2/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.2/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.2/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.2/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.2/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.2/awsibox/lambdas/StacksOps.code`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # vim: ft=python
 import cfg as app_cfg
 import os
 from datetime import datetime
+from pprint import pformat
 from iboxstacksops import cfg as i_cfg, commands as i_commands, msg as i_msg
 from iboxstacksops.aws import myboto3 as i_myboto3
 
 # Get Secrets from ParameterStore
 app_cfg.envRole = "buildkite"
 app_cfg.set({})
 
@@ -31,23 +32,34 @@
 
     result = {}
     for stack, appversion in event.items():
         i_cfg.stack = [stack]
         if appversion == "log":
             # just show stack log
             i_commands.log()
+        elif appversion == "info":
+            # just show stack info
+            result = pformat(i_commands.info())
         else:
             if isinstance(appversion, dict):
                 # appversion is a dict, used for stack with multiple appversions
                 for appn, appn_version in appversion.items():
                     setattr(i_cfg, f"EnvApp{appn}Version", appn_version)
             elif appversion == "restart":
                 # set vars to re-init/start services
                 i_cfg.EnvServiceRestartTime = str(datetime.now())
                 i_cfg.DockerLabelLastUpdate = str(datetime.now())
+            elif appversion == "start":
+                i_cfg.CapacityDesired = ''
+                i_cfg.CapacityMax = ''
+                i_cfg.CapacityMin = ''
+            elif appversion == "stop":
+                i_cfg.CapacityDesired = 0
+                i_cfg.CapacityMax = 0
+                i_cfg.CapacityMin = 0
             else:
                 i_cfg.EnvApp1Version = appversion
 
             try:
                 cmd_result = i_commands.update()
             except Exception as e:
                 result[stack] = e.args[0]
```

### Comparing `awsibox-0.8.0/awsibox/mappings.py` & `awsibox-0.8.2/awsibox/mappings.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/rds.py` & `awsibox-0.8.2/awsibox/rds.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/s3.py` & `awsibox-0.8.2/awsibox/s3.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/shared.py` & `awsibox-0.8.2/awsibox/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,14 +799,16 @@
                     parameter = Parameter(n)
                     _populate(parameter, rootdict=v)
                     add_obj(parameter)
 
             def _condition(k):
                 for n, v in k.items():
                     n = parse_ibox_key(n)
+                    if v == "IBOX_SKIP":
+                        continue
                     condition = {n: eval(v)}
                     add_obj(condition)
 
             def _output(k):
                 for n, v in k.items():
                     n = parse_ibox_key(n)
                     if not eval(v.get("IBOX_ENABLED_IF", "True")):
```

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.2/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.2/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/awsibox/waf.py` & `awsibox-0.8.2/awsibox/waf.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.2/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.0
+Version: 0.8.2
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.8.0/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.2/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 awsibox/cfg.py
 awsibox/cloudformation.py
 awsibox/cloudfront.py
 awsibox/common.py
 awsibox/discover.py
 awsibox/ec2.py
 awsibox/ecr.py
-awsibox/ecs.py
 awsibox/efs.py
 awsibox/elasticloadbalancing.py
 awsibox/generate.py
 awsibox/iam.py
 awsibox/joker.py
 awsibox/mappings.py
 awsibox/rds.py
```

### Comparing `awsibox-0.8.0/scripts/ibox_generate_templates.py` & `awsibox-0.8.2/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.0/setup.cfg` & `awsibox-0.8.2/setup.cfg`

 * *Files identical despite different names*

