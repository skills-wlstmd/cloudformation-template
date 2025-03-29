### **Create Stack**

```bash
aws cloudformation create-stack --stack-name <stack name> --region <region> --template-body file://<path>
```

### **Create Stack on IAM Role**

```bash
aws cloudformation create-stack --stack-name <stack name> --region <region> --template-body file://<path> --capabilities CAPABILITY_NAMED_IAM
```

### **Create ChangeSet**

```bash
aws cloudformation create-change-set \
	--stack-name <stack name>\
	--change-set-name <change set name> \
	--template-body file://<path>
```

### Execute ChangeSet

```bash
aws cloudformation execute-change-set \
	--stack-name <stack name>\
	--change-set-name <change set name>
```

### **Deploy Stack**

```bash
aws cloudformation deploy --stack-name <stack name> --region <region> --template-file <path>
```

### **Update Stack**

```bash
aws cloudformation update-template --region <region> --template-body file://<path>
```

### **Delete Stack**

```bash
aws cloudformation delete-stack --stack-name <stack name> --region <region>
```

### **Validate template**

```bash
aws cloudformation validate-template --region <region> --template-body file://<path>
```

### **Sample Code Templates Link**

[CloudFormation 템플릿 스니펫 - AWS CloudFormation](https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/CHAP_TemplateQuickRef.html)
