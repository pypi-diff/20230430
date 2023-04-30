# Comparing `tmp/aws-arn-0.0.2.tar.gz` & `tmp/aws-arn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-arn-0.0.2.tar", last modified: Sun Apr 30 13:10:11 2023, max compression
+gzip compressed data, was "aws-arn-0.0.3.tar", last modified: Sun Apr 30 13:20:45 2023, max compression
```

## Comparing `aws-arn-0.0.2.tar` & `aws-arn-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:10:11.201689 aws-arn-0.0.2/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:10:11.201508 aws-arn-0.0.2/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)    47960 2023-04-27 21:39:59.000000 aws-arn-0.0.2/README.md
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:10:11.200701 aws-arn-0.0.2/aws_arn/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2898 2023-04-30 12:56:06.000000 aws-arn-0.0.2/aws_arn/__init__.py
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157803 2023-04-30 11:54:55.000000 aws-arn-0.0.2/aws_arn/arn.py
-drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:10:11.201349 aws-arn-0.0.2/aws_arn.egg-info/
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:10:11.000000 aws-arn-0.0.2/aws_arn.egg-info/PKG-INFO
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      211 2023-04-30 13:10:11.000000 aws-arn-0.0.2/aws_arn.egg-info/SOURCES.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 13:10:11.000000 aws-arn-0.0.2/aws_arn.egg-info/dependency_links.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       41 2023-04-30 13:10:11.000000 aws-arn-0.0.2/aws_arn.egg-info/entry_points.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 13:10:11.000000 aws-arn-0.0.2/aws_arn.egg-info/top_level.txt
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 13:10:11.201723 aws-arn-0.0.2/setup.cfg
--rw-r--r--   0 gabrielsoltz   (501) staff       (20)      712 2023-04-30 13:09:58.000000 aws-arn-0.0.2/setup.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:20:45.663112 aws-arn-0.0.3/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:20:45.662997 aws-arn-0.0.3/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)    48465 2023-04-30 13:20:23.000000 aws-arn-0.0.3/README.md
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:20:45.662216 aws-arn-0.0.3/aws_arn/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)     2898 2023-04-30 12:56:06.000000 aws-arn-0.0.3/aws_arn/__init__.py
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)   157803 2023-04-30 11:54:55.000000 aws-arn-0.0.3/aws_arn/arn.py
+drwxr-xr-x   0 gabrielsoltz   (501) staff       (20)        0 2023-04-30 13:20:45.662843 aws-arn-0.0.3/aws_arn.egg-info/
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      455 2023-04-30 13:20:45.000000 aws-arn-0.0.3/aws_arn.egg-info/PKG-INFO
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      211 2023-04-30 13:20:45.000000 aws-arn-0.0.3/aws_arn.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        1 2023-04-30 13:20:45.000000 aws-arn-0.0.3/aws_arn.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       33 2023-04-30 13:20:45.000000 aws-arn-0.0.3/aws_arn.egg-info/entry_points.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)        8 2023-04-30 13:20:45.000000 aws-arn-0.0.3/aws_arn.egg-info/top_level.txt
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)       38 2023-04-30 13:20:45.663144 aws-arn-0.0.3/setup.cfg
+-rw-r--r--   0 gabrielsoltz   (501) staff       (20)      704 2023-04-30 13:20:36.000000 aws-arn-0.0.3/setup.py
```

### Comparing `aws-arn-0.0.2/README.md` & `aws-arn-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 # aws-arn
 A complete list of all AWS ARNs
 
 Isn't anyoning trying to guess the ARN for a specific AWS resource? This is a complete list of all AWS ARNs. The list is sorted alphabetically by service and resource.  This is the only complete list of AWS ARNs available anywhere.
 
+> :warning: **Work in progress**: This is a work in progress.  Not all services and resources are included yet.  Please open an issue or pull request if you find any errors or omissions.
+
 - Total number of services:  151
 - Total number of resources:  463
 
-If you find this useful, please star this repo.  If you find any errors, please open an issue or pull request.
+# Use it as a module
+
+```
+import aws_arn
+
+arn = aws_arn.generate_arn('i-1234568901', 'ec2', 'instance', 'us-east-1', '012345789012', 'aws')
+
+print (arn)
+
+arn:aws:ec2:us-east-1:012345789012:instance/i-1234568901
+
+```
+
+# Use it as CLI
+
+```
+./main.py --generate-arn --id test --service ec2 --sub-service instance --region us-east-1 --account 012345789012 --partition aws
+
+arn:aws:ec2:us-east-1:012345789012:instance/test
+```
 
-## ARN Format
+## Full List of ARNs
 
 | Service | ARN Format |
 | --- | --- |
 | acm | certificate: `arn:${Partition}:acm:${Region}:${Account}:certificate/${CertificateId}`<br> |
 | acm-pca | certificate_authority: `arn:${Partition}:acm-pca:${Region}:${Account}:certificate-authority/${CertificateAuthorityId}`<br> |
 | alexaforbusiness | skill: `arn:${Partition}:aplb:${Region}:${Account}:skill/${SkillId}`<br> |
 | apigateway | api: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}`<br>api_key: `arn:${Partition}:apigateway:${Region}::/apikeys/${ApiKeyId}`<br>authorizer: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/authorizers/${AuthorizerId}`<br>base_path_mapping: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/basepathmappings/${BasePathMappingId}`<br>client_certificate: `arn:${Partition}:apigateway:${Region}::/clientcertificates/${ClientCertificateId}`<br>deployment: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/deployments/${DeploymentId}`<br>documentation_part: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/documentation/parts/${DocumentationPartId}`<br>documentation_version: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/documentation/versions/${DocumentationVersion}`<br>domain_name: `arn:${Partition}:apigateway:${Region}::/domainnames/${DomainName}`<br>gateway_response: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/gatewayresponses/${GatewayResponseId}`<br>integration: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/resources/${ResourceId}/methods/${HttpMethod}/integrations/${IntegrationId}`<br>method: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/resources/${ResourceId}/methods/${HttpMethod}`<br>model: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/models/${ModelName}`<br>request_validator: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/requestvalidators/${RequestValidatorId}`<br>resource: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/resources/${ResourceId}`<br>rest_api: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}`<br>stage: `arn:${Partition}:apigateway:${Region}::/restapis/${ApiId}/stages/${StageName}`<br>usage_plan: `arn:${Partition}:apigateway:${Region}::/usageplans/${UsagePlanId}`<br>usage_plan_key: `arn:${Partition}:apigateway:${Region}::/usageplans/${UsagePlanId}/keys/${KeyId}`<br>vpc_link: `arn:${Partition}:apigateway:${Region}::/vpclinks/${VpcLinkId}`<br> |
@@ -158,8 +179,8 @@
 | waf | ipset: `arn:${Partition}:waf:${Region}:${Account}:ipset/${IpSetId}`<br>rule: `arn:${Partition}:waf:${Region}:${Account}:rule/${RuleId}`<br>web_acl: `arn:${Partition}:waf:${Region}:${Account}:webacl/${WebACLId}`<br>regional_rule_group: `arn:${Partition}:waf::${Account}:regional-rulegroup/${RuleGroupName}/${RuleGroupId}`<br>regional_web_acl: `arn:${Partition}:waf::${Account}:webacl/${WebACLName}/${WebACLId}`<br>global_web_acl: `arn:${Partition}:waf::${Account}:global-webacl/${WebACLName}/${WebACLId}`<br> |
 | waf-regional | ipset: `arn:${Partition}:waf-regional:${Region}:${Account}:ipset/${IpSetId}`<br>rule: `arn:${Partition}:waf-regional:${Region}:${Account}:rule/${RuleId}`<br>web_acl: `arn:${Partition}:waf-regional:${Region}:${Account}:webacl/${WebACLId}`<br>regional_rule_group: `arn:${Partition}:waf-regional:${Region}:${Account}:rulegroup/${RuleGroupName}/${RuleGroupId}`<br>regional_web_acl: `arn:${Partition}:waf-regional:${Region}:${Account}:webacl/${WebACLName}/${WebACLId}`<br> |
 | wafv2 | ip_set: `arn:${Partition}:wafv2:${Region}:${Account}:/ipset/${Scope}/${Id}`<br>rule_group: `arn:${Partition}:wafv2:${Region}:${Account}:/rulegroup/${Scope}/${Id}`<br>web_acl: `arn:${Partition}:wafv2:${Region}:${Account}:/webacl/${Scope}/${Id}`<br> |
 | wellarchitected | workload: `arn:${Partition}:wellarchitected:${Region}:${Account}:workload/${WorkloadId}`<br> |
 | workdocs | document: `arn:${Partition}:workdocs:${Region}:${Account}:${FolderHierarchy}/${DocumentName}`<br>folder: `arn:${Partition}:workdocs:${Region}:${Account}:${FolderHierarchy}/${FolderName}`<br>user: `arn:${Partition}:workdocs:${Region}:${Account}:user/${UserId}`<br> |
 | worklink | fleet: `arn:${Partition}:worklink:${Region}:${Account}:fleet/${FleetArnName}`<br>website_certificate_authority_association: `arn:${Partition}:worklink:${Region}:${Account}:website-certificate-authority-association/${WebsiteCertificateAuthorityAssociationId}`<br> |
 | workmail | organization: `arn:${Partition}:workmail:${Region}:${Account}:organization/${OrganizationId}`<br>resource: `arn:${Partition}:workmail:${Region}:${Account}:resource/${ResourceId}`<br>user: `arn:${Partition}:workmail:${Region}:${Account}:user/${UserId}`<br> |
-| workspaces | directory: `arn:${Partition}:workspaces:${Region}:${Account}:directory/${DirectoryId}`<br>workspace: `arn:${Partition}:workspaces:${Region}:${Account}:workspace/${WorkspaceId}`<br> |
+| workspaces | directory: `arn:${Partition}:workspaces:${Region}:${Account}:directory/${DirectoryId}`<br>workspace: `arn:${Partition}:workspaces:${Region}:${Account}:workspace/${WorkspaceId}`<br> |
```

### Comparing `aws-arn-0.0.2/aws_arn/__init__.py` & `aws-arn-0.0.3/aws_arn/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.2/aws_arn/arn.py` & `aws-arn-0.0.3/aws_arn/arn.py`

 * *Files identical despite different names*

### Comparing `aws-arn-0.0.2/setup.py` & `aws-arn-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='aws-arn',
-    version='0.0.2',
+    version='0.0.3',
     description='A library to work with AWS ARNs',
     packages=["aws_arn"],
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
-            'aws-arn = aws_arn:main',
+            'aws-arn = main',
         ],
     },
     author="Gabriel Alejandro Soltz",
     author_email="gabriel@3ops.com",
     project_urls={
         "Source code": "https://github.com/gabrielsoltz/aws-arn",
     },
```

