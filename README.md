# LanGraphChatBot
智能客服
命令行终端中直接运行如下命令安装依赖
pip install langgraph==0.2.74
pip install langchain-openai==0.3.6
pip install fastapi==0.115.8
pip install uvicorn==0.34.0
pip install gradio==5.18.0

主要内容:使用LangGraph+DeepSeek-R1+FastAPI+Gradio实现一个带有记忆功能的流量包推荐智能客服web端用例,同时也支持gpt大模型、国产大模型(OneApi方式)、Ollama本地开源大模型、阿里通义千问大模型

（1）启动main脚本
进入01_ChatBot文件夹下，在使用python main.py命令启动脚本前，需根据自己的实际情况调整代码中的如下参数
llms.py中关于大模型配置参数的调整，以及main.py脚本中的服务IP和PORT、LangSmith平台的API KEY等的设置

（2）运行webUI脚本进行测试
进入01_ChatBot文件夹下，再使用python webUI.py命令启动脚本前，需根据自己的实际情况调整代码中的如下参数，运行成功后，可以查看smith的跟踪情况
是否要流式输出可设置stream_flag = False或True，检查URL地址中的IP和PORT是否和main脚本中相同
运行成功后直接打开网址，在浏览器端进行交互测试
