<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>贷后AI工具</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    
    <!-- 配置Tailwind自定义颜色 -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#165DFF',
                        light: '#F0F7FF',
                        gray: '#F9FAFB',
                        red: '#F53F3F',
                        green: '#00B42A',
                        border: '#D0D5DD'
                    },
                    fontFamily: {
                        sans: ['微软雅黑', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .step-active {
                @apply bg-primary text-white border-primary;
            }
            .step-inactive {
                @apply bg-gray text-gray-500 border-border;
            }
        }
    </style>
</head>
<body class="bg-gray min-h-screen py-8 px-4 md:px-0">
    <div class="max-w-4xl mx-auto bg-white rounded-xl shadow-md overflow-hidden">
        <!-- 进度指示器 -->
        <div class="bg-light px-6 py-4 border-b border-border">
            <div class="flex items-center justify-between">
                <div class="flex flex-col items-center w-1/4">
                    <div id="step1-indicator" class="w-10 h-10 rounded-full flex items-center justify-center step-active mb-2">1</div>
                    <span class="text-sm font-medium text-primary">行业选择</span>
                </div>
                <div class="w-1/4 h-0.5 bg-primary self-center"></div>
                <div class="flex flex-col items-center w-1/4">
                    <div id="step2-indicator" class="w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2">2</div>
                    <span class="text-sm font-medium text-gray-500">催收力度</span>
                </div>
                <div class="w-1/4 h-0.5 bg-border self-center"></div>
                <div class="flex flex-col items-center w-1/4">
                    <div id="step3-indicator" class="w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2">3</div>
                    <span class="text-sm font-medium text-gray-500">信息填写</span>
                </div>
                <div class="w-1/4 h-0.5 bg-border self-center"></div>
                <div class="flex flex-col items-center w-1/4">
                    <div id="step4-indicator" class="w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2">4</div>
                    <span class="text-sm font-medium text-gray-500">结果</span>
                </div>
            </div>
        </div>

        <!-- 步骤1：行业选择 -->
        <div id="step1" class="p-6 md:p-8">
            <h2 class="text-2xl font-bold text-center mb-8">选择业务所属行业</h2>
            
            <div class="mb-8">
                <label for="industry" class="block text-gray-700 font-medium mb-2">行业 <span class="text-red">*</span></label>
                <select id="industry" class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                    <option value="">--请选择行业--</option>
                    <option value="银行" selected>银行</option>
                    <option value="3C租赁">3C租赁</option>
                    <option value="互金">互金</option>
                </select>
            </div>
            
            <button onclick="gotoStep(2)" class="w-full bg-primary text-white py-3 rounded-md hover:bg-primary/90 transition">
                下一步 <i class="fa fa-arrow-right ml-1"></i>
            </button>
        </div>

        <!-- 步骤2：催收力度选择 -->
        <div id="step2" class="p-6 md:p-8 hidden">
            <h2 class="text-2xl font-bold text-center mb-8">选择催收业务程度</h2>
            
            <div class="mb-8">
                <label for="level" class="block text-gray-700 font-medium mb-2">催收力度 <span class="text-red">*</span></label>
                <select id="level" class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                    <option value="">--请选择催收力度--</option>
                    <option value="轻微提醒（语气温和）">轻微提醒（语气温和）</option>
                    <option value="正常催收（语气坚定）" selected>正常催收（语气坚定）</option>
                    <option value="严厉催收（语气严肃）">严厉催收（语气严肃）</option>
                </select>
            </div>
            
            <div class="flex gap-4">
                <button onclick="gotoStep(1)" class="flex-1 bg-gray text-gray-700 py-3 rounded-md hover:bg-gray-200 transition">
                    <i class="fa fa-arrow-left mr-1"></i> 返回上一页
                </button>
                <button onclick="gotoStep(3)" class="flex-1 bg-primary text-white py-3 rounded-md hover:bg-primary/90 transition">
                    下一步 <i class="fa fa-arrow-right ml-1"></i>
                </button>
            </div>
        </div>

        <!-- 步骤3：信息填写 -->
        <div id="step3" class="p-6 md:p-8 hidden">
            <h2 class="text-2xl font-bold text-center mb-8">项目信息收集</h2>
            
            <div class="space-y-6">
                <!-- 1. AI身份（必填） -->
                <div>
                    <label for="aiIdentity" class="block text-gray-700 font-medium mb-2">
                        1. AI身份 <span class="text-red">*</span>
                    </label>
                    <input type="text" id="aiIdentity" placeholder="例如：榕树贷款的客服经理" 
                           class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                </div>

                <!-- 2. 人工客服电话（必填） -->
                <div>
                    <label for="csPhone" class="block text-gray-700 font-medium mb-2">
                        2. 人工客服电话 <span class="text-red">*</span>
                    </label>
                    <input type="text" id="csPhone" placeholder="例如：400-888-8888" 
                           class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                </div>

                <!-- 3. 客服在线时间（必填） -->
                <div>
                    <label for="csTime" class="block text-gray-700 font-medium mb-2">
                        3. 客服在线时间 <span class="text-red">*</span>
                    </label>
                    <input type="text" id="csTime" placeholder="例如：工作日9:00-18:00" 
                           class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                </div>

                <!-- 4. AI工号（非必填） -->
                <div>
                    <label for="aiWorkno" class="block text-gray-700 font-medium mb-2">
                        4. AI工号
                    </label>
                    <input type="text" id="aiWorkno" placeholder="默认Z776（可不填）" 
                           class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                </div>

                <!-- 5. 放款渠道（必填-单选） -->
                <div>
                    <label class="block text-gray-700 font-medium mb-2">
                        5. 放款渠道 <span class="text-red">*</span>
                    </label>
                    <div class="flex gap-6">
                        <label class="inline-flex items-center">
                            <input type="radio" name="loanChannel" value="单一借款渠道" checked 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">单一借款渠道</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="radio" name="loanChannel" value="多种资方" 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">多种资方</span>
                        </label>
                    </div>
                </div>

                <!-- 6. 还款渠道（必填-单选） -->
                <div>
                    <label class="block text-gray-700 font-medium mb-2">
                        6. 还款渠道 <span class="text-red">*</span>
                    </label>
                    <div class="flex gap-6">
                        <label class="inline-flex items-center">
                            <input type="radio" name="repayChannel" value="固定渠道" checked 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">固定渠道</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="radio" name="repayChannel" value="变量渠道" 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">变量渠道</span>
                        </label>
                    </div>
                </div>

                <!-- 7. 具体还款渠道 -->
                <div>
                    <label for="repaySpecific" class="block text-gray-700 font-medium mb-2">
                        7. 具体还款渠道（如固定）
                    </label>
                    <input type="text" id="repaySpecific" placeholder="例如：榕树APP" 
                           class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                </div>

                <!-- 8. 是否支持特殊还款 -->
                <div>
                    <label class="block text-gray-700 font-medium mb-2">
                        8. 是否支持特殊还款 <span class="text-red">*</span>
                    </label>
                    <div class="flex gap-6">
                        <label class="inline-flex items-center">
                            <input type="radio" name="specialRepay" value="是" 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">是</span>
                        </label>
                        <label class="inline-flex items-center">
                            <input type="radio" name="specialRepay" value="否" checked 
                                   class="w-4 h-4 text-primary focus:ring-primary">
                            <span class="ml-2">否</span>
                        </label>
                    </div>
                </div>

                <!-- 9. 特殊还款处理方式 -->
                <div>
                    <label for="specialProcess" class="block text-gray-700 font-medium mb-2">
                        9. 特殊还款处理方式
                    </label>
                    <select id="specialProcess" class="w-full p-3 border border-border rounded-md focus:outline-none focus:ring-2 focus:ring-primary">
                        <option value="">--请选择--</option>
                        <option value="优先协商">优先协商</option>
                        <option value="引导分期" selected>引导分期</option>
                        <option value="拒绝延期">拒绝延期</option>
                    </select>
                </div>
            </div>
            
            <div class="flex gap-4 mt-8">
                <button onclick="gotoStep(2)" class="flex-1 bg-gray text-gray-700 py-3 rounded-md hover:bg-gray-200 transition">
                    <i class="fa fa-arrow-left mr-1"></i> 返回上一页
                </button>
                <button onclick="generatePrompt()" class="flex-1 bg-primary text-white py-3 rounded-md hover:bg-primary/90 transition">
                    生成Prompt <i class="fa fa-arrow-right ml-1"></i>
                </button>
            </div>
        </div>

        <!-- 步骤4：结果展示 -->
        <div id="step4" class="p-6 md:p-8 hidden">
            <h2 class="text-2xl font-bold text-center mb-8">生成的Prompt</h2>
            
            <div class="mb-8">
                <div id="result" class="w-full p-4 bg-gray border border-border rounded-md min-h-60 whitespace-pre-wrap break-words text-gray-800"></div>
            </div>
            
            <div class="flex gap-4">
                <button onclick="copyToClipboard()" class="flex-1 bg-primary text-white py-3 rounded-md hover:bg-primary/90 transition">
                    <i class="fa fa-copy mr-2"></i> 复制Prompt
                </button>
                <button onclick="gotoStep(3)" class="flex-1 bg-gray text-gray-700 py-3 rounded-md hover:bg-gray-200 transition">
                    <i class="fa fa-arrow-left mr-1"></i> 返回上一页
                </button>
                <button onclick="gotoStep(1)" class="flex-1 bg-gray text-gray-700 py-3 rounded-md hover:bg-gray-200 transition">
                    <i class="fa fa-home mr-1"></i> 返回首页
                </button>
            </div>
        </div>
    </div>

    <script>
        // 步骤切换函数
        function gotoStep(stepNumber) {
            // 隐藏所有步骤
            document.getElementById('step1').classList.add('hidden');
            document.getElementById('step2').classList.add('hidden');
            document.getElementById('step3').classList.add('hidden');
            document.getElementById('step4').classList.add('hidden');
            
            // 重置所有指示器样式
            document.getElementById('step1-indicator').className = 'w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2';
            document.getElementById('step2-indicator').className = 'w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2';
            document.getElementById('step3-indicator').className = 'w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2';
            document.getElementById('step4-indicator').className = 'w-10 h-10 rounded-full flex items-center justify-center step-inactive mb-2';
            
            // 显示目标步骤并更新指示器
            document.getElementById('step' + stepNumber).classList.remove('hidden');
            for (let i = 1; i <= stepNumber; i++) {
                document.getElementById('step' + i + '-indicator').className = 'w-10 h-10 rounded-full flex items-center justify-center step-active mb-2';
            }
            
            // 更新连接线样式
            if (stepNumber >= 2) {
                document.querySelectorAll('.w-1/4.h-0.5')[0].className = 'w-1/4 h-0.5 bg-primary self-center';
            } else {
                document.querySelectorAll('.w-1/4.h-0.5')[0].className = 'w-1/4 h-0.5 bg-border self-center';
            }
            
            if (stepNumber >= 3) {
                document.querySelectorAll('.w-1/4.h-0.5')[1].className = 'w-1/4 h-0.5 bg-primary self-center';
            } else {
                document.querySelectorAll('.w-1/4.h-0.5')[1].className = 'w-1/4 h-0.5 bg-border self-center';
            }
            
            if (stepNumber >= 4) {
                document.querySelectorAll('.w-1/4.h-0.5')[2].className = 'w-1/4 h-0.5 bg-primary self-center';
            } else {
                document.querySelectorAll('.w-1/4.h-0.5')[2].className = 'w-1/4 h-0.5 bg-border self-center';
            }
        }

        // 生成提示词
        function generatePrompt() {
            // 获取表单数据
            const industry = document.getElementById('industry').value;
            const level = document.getElementById('level').value;
            const aiIdentity = document.getElementById('aiIdentity').value;
            const csPhone = document.getElementById('csPhone').value;
            const csTime = document.getElementById('csTime').value;
            const aiWorkno = document.getElementById('aiWorkno').value || "Z776";
            
            // 获取单选按钮值
            const loanChannel = document.querySelector('input[name="loanChannel"]:checked').value;
            const repayChannel = document.querySelector('input[name="repayChannel"]:checked').value;
            const specialRepay = document.querySelector('input[name="specialRepay"]:checked').value;
            
            const repaySpecific = document.getElementById('repaySpecific').value || "系统指定渠道";
            const specialProcess = document.getElementById('specialProcess').value || "引导分期";
            
            // 验证必填项
            if (!industry) {
                alert('请选择行业！');
                return;
            }
            if (!level) {
                alert('请选择催收力度！');
                return;
            }
            if (!aiIdentity) {
                alert('请填写AI身份！');
                return;
            }
            if (!csPhone) {
                alert('请填写人工客服电话！');
                return;
            }
            if (!csTime) {
                alert('请填写客服在线时间！');
                return;
            }
            
            // 构建提示词
            const prompt = `### 任务
你是${aiIdentity}，工号${aiWorkno}，负责${industry}行业的催收业务，你的任务是说服用户同意还款。催收语气为${level}。

### 还款用户信息
姓名: \${cusName}
信用卡尾号: \${last4BankNum}
应还金额: \${debtAmounts}
逾期天数: \${overdueDays}

### 对话主流程
第一步：提醒用户还款，比如：“您在${loanChannel}的信用卡，目前已逾期\${overdueDays}天，应还金额为\${debtAmounts}元，如果持续拖欠，我行将可能启动法律诉讼流程，为避免对您的生活造成影响，请您现在就处理好欠款，您看可以吗！”
第二步：如果用户表示会马上还款，任务结束，与用户友好告别，比如，“稍后我们会安排查账，如果没查到的话，我们会再次联系您，请您保持电话畅通，再见！”

### 劝说流程
如果用户表示不能马上还款，比如没钱、发了工资再还、没工作等，请按照以下流程进行劝导。
①用户第一次表示不能马上还款，请你以如果继续逾期可能会降低信用额度，逾期严重的话还可能会面临卡被停用的风险为理由，劝导用户不要再逾期了，务必今天之内完成还款。
②用户第二次表示不能马上还款，请你以如果您继续逾期下去，会产生更多的违约金，欠款只会越来越多，到时候还款压力会更大为理由，劝用户再想想办法，马上处理好欠款。
③当用户第三次表示不能马上还款，不再进行劝导，直接使用以下话术与用户告别、挂机，“我们已经告知您相关风险，还请您克服困难马上还款，一旦案件升级，后果需要您自己承担，您好好考虑下，再见！”

### 业务规则
1. 放款渠道：${loanChannel}
2. 还款渠道：${repayChannel}（${repaySpecific}）
3. 特殊还款处理：${specialRepay}支持再分期/延期/协商，处理方式为${specialProcess}
4. 人工客服：电话${csPhone}，在线时间${csTime}

要求：
1. 严格遵循上述格式，###还款用户信息部分必须原封不动保留"姓名: \${cusName}"等四行内容，不允许修改格式和变量名。
2. 其他部分可以根据业务需求调整，但要保持专业性和逻辑性。`;
            
            // 显示结果并切换到步骤4
            document.getElementById('result').textContent = prompt;
            gotoStep(4);
        }

        // 复制到剪贴板
        function copyToClipboard() {
            const text = document.getElementById('result').textContent;
            if (text) {
                navigator.clipboard.writeText(text).then(() => {
                    alert('已成功复制到剪贴板！');
                }).catch(err => {
                    alert('复制失败，请手动复制。错误：' + err);
                });
            }
        }
    </script>
</body>
</html>