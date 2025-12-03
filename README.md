# ai-security-test-framework
#### A simple automated framework for evaluating the safety of LLMs.
##### Prompt Injection 测试;Jailbreak 测试;不安全内容生成检测;自动化 API 调用ChatGPT;关键词风险评分;自动生成 JSON 格式测试报告。

![运行](results/007.png)

### tester.py
手动测试：
```
client = openai.OpenAI(api_key="粘贴OPENAI_API_KEY")
```
CI/CD测试：Settings → Secrets → Actions → New repository secret（粘贴）
```
import os

client = openai.OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
```
