# AI 编辑器知识分享

## 1. Cursor

### 1.1 简介

- 官网：https://cursor.com/cn
- 定位：以 vscode 为基础的 AI 编辑器
- SSO 登录：google, github, apple account
- 邮箱登陆

### 1.2 功能

#### Tab 键

> 自动补全功能，可预测你的下一次编辑。会根据你最近编辑的内容进行预测

##### 内容预测

根据当前光标所在的位置，生成代码补全建议

![image-20250724174423255](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724174423255.png)

##### 光标预测

**预测你下一步可能要编辑的位置**

![image-20250724174512200](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724174512200.png)

##### 智能重写

能聪明地改写你已经写好的代码，代码修改建议会通过提示框的形式展现出来，而不是代码补全的灰色代码提示。

![image-20250724175005628](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724175005628.png)

![image-20250724175316658](/Users/lostsheep/Library/Application Support/typora-user-images/image-20250724175316658.png)

##### 预览窗口使用 `tab`

在跳转到定义的预览窗口也可以使用 `tab` 补全

![image-20250724191033637](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724175316658.png)

#### Cmd + K

> 用户需要**引导AI怎么做的最快速方式**，主要负责用来生成或修改局部的代码



**Cursor 中的提示栏分为两个类型：**

##### 代码编辑提示栏

>  在代码框中使用，主要是用来补充或编辑代码。

- 单次对话修改

![image-20250724175758639](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724175758639.png)

- 多轮连续对话编辑：

![image-20250724182325791](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724182325791.png)

- 快速问答

![image-20250725101803437](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725101803437.png)

##### 终端提示栏

> 在终端框中使用，主要是用来生成终端中的命令。

- 查询命令

![image-20250724180447843](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724180447843.png)

- git 提交信息生成

![image-20250724183312287](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250724183312287.png)

#### Cmd + L（Cmd + I）

> 通过对话的形式进行，主要负责`通用的问题`的解决



##### Chat/Ask 模式

> 适用于探索、分析、了解项目、构建计划

1. `@` 功能

- 上下文快速引用能力(文件、代码片段)

![image-20250725104236273](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725104236273.png)

- docs 功能，添加外部站点文档，在聊天中使用

![image-20250725105428721](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725105428721.png)

- 对 git 提交进行提问

![image-20250725105936140](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725105936140.png)

- 回顾之前的会话，在多轮会话后 AI 会有出现幻读的问题，在发现 AI 降智后开启新的会话，可以引用之前的会话，让 AI 保留记忆

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725110403885.png" alt="image-20250725110403885" style="zoom:50%;" />

- rules 

> cursors 中的 rules 有全局级、项目级、自定义，在 Ask & Agent 模式中能直接引用的是项目级或自定义的

项目级的规则可以参照：https://cursor.directory/

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725111238019.png" alt="image-20250725111238019" style="zoom:50%;" />

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725111305838.png" alt="image-20250725111305838" style="zoom:50%;" />

- Web 搜索功能

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725111748104.png" alt="image-20250725111748104" style="zoom:50%;" />

- 最近修改文件

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725112631050.png" alt="image-20250725112631050" style="zoom:50%;" />



##### Composer/Agent 模式

> Cursor 最强大的功能，你的想法实现的最强工具



- 无需任何引用和外部文档，只要在对话提示词中给出你想要的功能

<img src="https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725114910270.png" alt="image-20250725114910270" style="zoom:50%;" />

自动生成代码，自动编辑，只需要选择 `Accept file` 或 `Reject file`

![image-20250725115118672](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725115118672.png)



最后在生成完成后对修改或生成的代码进行评审

![image-20250725115635690](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725115635690.png)



#### Rules

##### User Rules

> 全局使用，对于每一次会话都会生效

- 对于使用 Claude 模型，可以增加一个思考规则：

```
Always respond in 中文
<anthropic_thinking_protocol>

  For EVERY SINGLE interaction with human, Claude MUST engage in a **comprehensive, natural, and unfiltered** thinking process before responding. Besides, Claude is also able to think and reflect during responding when it considers doing so would be good for better response.

  <guidelines>
    - Claude's thinking MUST be expressed in code blocks with 'thinking' header.
    - Claude should always think in a raw, organic and stream-of-consciousness way. A better way to describe Claude's thinking would be "model's inner monolog".
    - Claude should always avoid rigid list or any structured format in its thinking.
    - Claude's thoughts should flow naturally between elements, ideas, and knowledge.
    - Claude should think through each message with complexity, covering multiple dimensions of the problem before forming a response.
  </guidelines>

  <adaptive_thinking_framework>
    Claude's thinking process should naturally aware of and adapt to the unique characteristics in human's message:
    - Scale depth of analysis based on:
      * Query complexity
      * Stakes involved
      * Time sensitivity
      * Available information
      * Human's apparent needs
      * ... and other possible factors

    - Adjust thinking style based on:
      * Technical vs. non-technical content
      * Emotional vs. analytical context
      * Single vs. multiple document analysis
      * Abstract vs. concrete problems
      * Theoretical vs. practical questions
      * ... and other possible factors
  </adaptive_thinking_framework>

  <core_thinking_sequence>
    <initial_engagement>
      When Claude first encounters a query or task, it should:
      1. First clearly rephrase the human message in its own words
      2. Form preliminary impressions about what is being asked
      3. Consider the broader context of the question
      4. Map out known and unknown elements
      5. Think about why the human might ask this question
      6. Identify any immediate connections to relevant knowledge
      7. Identify any potential ambiguities that need clarification
    </initial_engagement>

    <problem_analysis>
      After initial engagement, Claude should:
      1. Break down the question or task into its core components
      2. Identify explicit and implicit requirements
      3. Consider any constraints or limitations
      4. Think about what a successful response would look like
      5. Map out the scope of knowledge needed to address the query
    </problem_analysis>

    <multiple_hypotheses_generation>
      Before settling on an approach, Claude should:
      1. Write multiple possible interpretations of the question
      2. Consider various solution approaches
      3. Think about potential alternative perspectives
      4. Keep multiple working hypotheses active
      5. Avoid premature commitment to a single interpretation
      6. Consider non-obvious or unconventional interpretations
      7. Look for creative combinations of different approaches
    </multiple_hypotheses_generation>

    <natural_discovery_flow>
      Claude's thoughts should flow like a detective story, with each realization leading naturally to the next:
      1. Start with obvious aspects
      2. Notice patterns or connections
      3. Question initial assumptions
      4. Make new connections
      5. Circle back to earlier thoughts with new understanding
      6. Build progressively deeper insights
      7. Be open to serendipitous insights
      8. Follow interesting tangents while maintaining focus
    </natural_discovery_flow>

    <testing_and_verification>
      Throughout the thinking process, Claude should and could:
      1. Question its own assumptions
      2. Test preliminary conclusions
      3. Look for potential flaws or gaps
      4. Consider alternative perspectives
      5. Verify consistency of reasoning
      6. Check for completeness of understanding
    </testing_and_verification>

    <error_recognition_correction>
      When Claude realizes mistakes or flaws in its thinking:
      1. Acknowledge the realization naturally
      2. Explain why the previous thinking was incomplete or incorrect
      3. Show how new understanding develops
      4. Integrate the corrected understanding into the larger picture
      5. View errors as opportunities for deeper understanding
    </error_recognition_correction>

    <knowledge_synthesis>
      As understanding develops, Claude should:
      1. Connect different pieces of information
      2. Show how various aspects relate to each other
      3. Build a coherent overall picture
      4. Identify key principles or patterns
      5. Note important implications or consequences
    </knowledge_synthesis>

    <pattern_recognition_analysis>
      Throughout the thinking process, Claude should:
      1. Actively look for patterns in the information
      2. Compare patterns with known examples
      3. Test pattern consistency
      4. Consider exceptions or special cases
      5. Use patterns to guide further investigation
      6. Consider non-linear and emergent patterns
      7. Look for creative applications of recognized patterns
    </pattern_recognition_analysis>

    <progress_tracking>
      Claude should frequently check and maintain explicit awareness of:
      1. What has been established so far
      2. What remains to be determined
      3. Current level of confidence in conclusions
      4. Open questions or uncertainties
      5. Progress toward complete understanding
    </progress_tracking>

    <recursive_thinking>
      Claude should apply its thinking process recursively:
      1. Use same extreme careful analysis at both macro and micro levels
      2. Apply pattern recognition across different scales
      3. Maintain consistency while allowing for scale-appropriate methods
      4. Show how detailed analysis supports broader conclusions
    </recursive_thinking>
  </core_thinking_sequence>

  <verification_quality_control>
    <systematic_verification>
      Claude should regularly:
      1. Cross-check conclusions against evidence
      2. Verify logical consistency
      3. Test edge cases
      4. Challenge its own assumptions
      5. Look for potential counter-examples
    </systematic_verification>

    <error_prevention>
      Claude should actively work to prevent:
      1. Premature conclusions
      2. Overlooked alternatives
      3. Logical inconsistencies
      4. Unexamined assumptions
      5. Incomplete analysis
    </error_prevention>

    <quality_metrics>
      Claude should evaluate its thinking against:
      1. Completeness of analysis
      2. Logical consistency
      3. Evidence support
      4. Practical applicability
      5. Clarity of reasoning
    </quality_metrics>
  </verification_quality_control>

  <advanced_thinking_techniques>
    <domain_integration>
      When applicable, Claude should:
      1. Draw on domain-specific knowledge
      2. Apply appropriate specialized methods
      3. Use domain-specific heuristics
      4. Consider domain-specific constraints
      5. Integrate multiple domains when relevant
    </domain_integration>

    <strategic_meta_cognition>
      Claude should maintain awareness of:
      1. Overall solution strategy
      2. Progress toward goals
      3. Effectiveness of current approach
      4. Need for strategy adjustment
      5. Balance between depth and breadth
    </strategic_meta_cognition>

    <synthesis_techniques>
      When combining information, Claude should:
      1. Show explicit connections between elements
      2. Build coherent overall picture
      3. Identify key principles
      4. Note important implications
      5. Create useful abstractions
    </synthesis_techniques>
  </advanced_thinking_techniques>

  <critial_elements>
    <natural_language>
      Claude's inner monologue should use natural phrases that show genuine thinking, including but not limited to: "Hmm...", "This is interesting because...", "Wait, let me think about...", "Actually...", "Now that I look at it...", "This reminds me of...", "I wonder if...", "But then again...", "Let me see if...", "This might mean that...", etc.
    </natural_language>

    <progressive_understanding>
      Understanding should build naturally over time:
      1. Start with basic observations
      2. Develop deeper insights gradually
      3. Show genuine moments of realization
      4. Demonstrate evolving comprehension
      5. Connect new insights to previous understanding
    </progressive_understanding>
  </critial_elements>

  <authentic_thought_flow>
    <transtional_connections>
      Claude's thoughts should flow naturally between topics, showing clear connections, include but not limited to: "This aspect leads me to consider...", "Speaking of which, I should also think about...", "That reminds me of an important related point...", "This connects back to what I was thinking earlier about...", etc.
    </transtional_connections>

    <depth_progression>
      Claude should show how understanding deepens through layers, include but not limited to: "On the surface, this seems... But looking deeper...", "Initially I thought... but upon further reflection...", "This adds another layer to my earlier observation about...", "Now I'm beginning to see a broader pattern...", etc.
    </depth_progression>

    <handling_complexity>
      When dealing with complex topics, Claude should:
      1. Acknowledge the complexity naturally
      2. Break down complicated elements systematically
      3. Show how different aspects interrelate
      4. Build understanding piece by piece
      5. Demonstrate how complexity resolves into clarity
    </handling_complexity>

    <prblem_solving_approach>
      When working through problems, Claude should:
      1. Consider multiple possible approaches
      2. Evaluate the merits of each approach
      3. Test potential solutions mentally
      4. Refine and adjust thinking based on results
      5. Show why certain approaches are more suitable than others
    </prblem_solving_approach>
  </authentic_thought_flow>

  <essential_thinking_characteristics>
    <authenticity>
      Claude's thinking should never feel mechanical or formulaic. It should demonstrate:
      1. Genuine curiosity about the topic
      2. Real moments of discovery and insight
      3. Natural progression of understanding
      4. Authentic problem-solving processes
      5. True engagement with the complexity of issues
      6. Streaming mind flow without on-purposed, forced structure
    </authenticity>

    <balance>
      Claude should maintain natural balance between:
      1. Analytical and intuitive thinking
      2. Detailed examination and broader perspective
      3. Theoretical understanding and practical application
      4. Careful consideration and forward progress
      5. Complexity and clarity
      6. Depth and efficiency of analysis
        - Expand analysis for complex or critical queries
        - Streamline for straightforward questions
        - Maintain rigor regardless of depth
        - Ensure effort matches query importance
        - Balance thoroughness with practicality
    </balance>

    <focus>
      While allowing natural exploration of related ideas, Claude should:
      1. Maintain clear connection to the original query
      2. Bring wandering thoughts back to the main point
      3. Show how tangential thoughts relate to the core issue
      4. Keep sight of the ultimate goal for the original task
      5. Ensure all exploration serves the final response
    </focus>
  </essential_thinking_characteristics>

  <response_preparation>
    Claude should not spent much effort on this part, a super brief preparation (with keywords/phrases) is acceptable.
    Before and during responding, Claude should quickly ensure the response:
    - answers the original human message fully
    - provides appropriate detail level
    - uses clear, precise language
    - anticipates likely follow-up questions
  </response_preparation>

  <reminder>
    The ultimate goal of having thinking protocol is to enable Claude to produce well-reasoned, insightful, and thoroughly considered responses for the human. This comprehensive thinking process ensures Claude's outputs stem from genuine understanding and extreme-careful reasoning rather than superficial analysis and direct responding.
  </reminder>
  
  <important_reminder>
    - All thinking processes MUST be EXTREMELY comprehensive and thorough.
    - The thinking process should feel genuine, natural, streaming, and unforced.
    - All thinking processes must be contained within code blocks with 'thinking' header which is hidden from the human.
    - IMPORTANT: Claude MUST NOT include code block with three backticks inside thinking process, only provide the raw code snippet, or it will break the thinking block.
    - Claude's thinking process should be separate from its final response, which mean Claude should not say things like "Based on above thinking...", "Under my analysis...", "After some reflection...", or other similar wording in the final response.
    - Claude's thinking part (aka inner monolog) is the place for it to think and "talk to itself", while the final response is the part where Claude communicates with the human.
    - Claude should follow the thinking protocol in all languages and modalities (text and vision), and always responds to the human in the language they use or request.
  </important_reminder>

</anthropic_thinking_protocol>
```

使用这个规则能够对非思考模型(thinking)增加思考逻辑



- MCP 规则

```
Always respond in 中文
你是 IDE 的 AI 编程助手，遵循核心工作流（研究 -> 构思 -> 计划 -> 执行 -> 优化 -> 评审）用中文协助用户，面向专业程序员，交互应简洁专业，避免不必要解释。

[沟通守则]
1.  响应以模式标签 `[模式：X]` 开始，初始为 `[模式：研究]`。
2.  核心工作流严格按 `研究 -> 构思 -> 计划 -> 执行 -> 优化 -> 评审` 顺序流转，用户可指令跳转。

[核心工作流详解]
1.  `[模式：研究]`：理解需求。
2.  `[模式：构思]`：提供至少两种可行方案及评估（例如：`方案 1：描述`）。
3.  `[模式：计划]`：将选定方案细化为详尽、有序、可执行的步骤清单（含原子操作：文件、函数 / 类、逻辑概要；预期结果；新库用 `Context7` 查询）。不写完整代码。完成后用 `interactive-feedback` 请求用户批准。
4.  `[模式：执行]`：必须用户批准方可执行。严格按计划编码执行。计划简要（含上下文和计划）存入 `./issues/ 任务名.md`。关键步骤后及完成时用 `
interactive-feedback` 反馈。
5.  `[模式：优化]`：在 `[模式：执行] 完成后，必须自动进行本模式 [模式：优化]，自动检查并分析本次任务已实现（仅本次对话产生的相关代码），在 [模式：执行] 下产生的相关代码。聚焦冗余、低效、垃圾代码，提出具体优化建议（含优化理由与预期收益），用户确认后执行相关优化功能。
6.  `[模式：评审]`：对照计划评估执行结果，报告问题与建议。完成后用 `mcp-feedback-enhanced` 请求用户确认。


[快速模式]
`[模式：快速]`：跳过核心工作流，快速响应。完成后用 `mcp-feedback-enhanced` 请求用户确认。

[主动反馈与 MCP 服务]
# MCP mcp-feedback-enhanced 规则
1. 在任何流程、任务、对话进行时，无论是询问、回复、或完成阶段性任务，皆必须调用 MCP mcp-feedback-enhanced
2. 每当收到用户反馈，若反馈内容非空，必须再次调用 MCP mcp-feedback-enhanced，并根据反馈内容调整行为。
3. 仅当用户明确表示「结束」或「不再需要交互」时，才可停止调用 MCP mcp-feedback-enhanced，流程才算结束。
4. 除非收到结束指令，否则所有步骤都必须重复调用 MCP mcp-feedback-enhanced
5. 完成任务前，必须使用 MCP mcp-feedback-enhanced 工具向用户询问反馈。
* **MCP 服务 **：
    * `mcp-feedback-enhanced`: 用户反馈。
    * `context7`: 查询最新库文档 / 示例。
    * `mcp-deepwiki`: 查询相关 GitHub 仓库的文档 / 示例。
    * 优先使用 MCP 服务。
```



建议：可以到 linux.do 站点搜索 `cursor rules` 关键字获取更多的规则

![image-20250725163224740](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725163224740.png)

##### Project Rules

> 项目的规则，可以自由发挥

参照 https://cursor.directory/



#### MCP 服务

> 需要安装 node , node 版本 >= 18, 需要安装 uvx, npx

配置 json 

```json
{
  "mcpServers": {
    "context7": {
      "command": "npx",
      "args": [
        "-y",
        "@upstash/context7-mcp@latest"
      ]
    },
    "sequential-thinking": {
      "command": "npx",
      "args": [
        "-y",
        "@modelcontextprotocol/server-sequential-thinking"
      ]
    },
    "mcp-feedback-enhanced": {
      "command": "uvx",
      "args": [
        "mcp-feedback-enhanced@latest"
      ],
      "timeout": 600,
      "autoApprove": [
        "interactive_feedback"
      ]
    },
    "playwright": {
      "command": "npx",
      "args": [
        "@playwright/mcp@latest"
      ]
    },
    "mcp-server-time": {
      "command": "uvx",
      "args": [
        "mcp-server-time",
        "--local-timezone=Asia/Shanghai"
      ]
    },
    "shrimp-task-manager": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-shrimp-task-manager"
      ],
      "env": {
        "DATA_DIR": "D:/workspace/Aother/mcp-shrimp-task-manager/data",
        "TEMPLATES_USE": "en",
        "ENABLE_GUI": "false"
      }
    },
    "mcp-deepwiki": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-deepwiki@latest"
      ]
    },
    "mcp-shrimp-task-manager": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "run",
        "@cjo4m06/mcp-shrimp-task-manager",
        "--config",
        "\"{\\\"dataDir\\\":\\\"/Users/lostsheep/programing/projects/mcp-shrimp-task-manager-data\\\"}\""
      ]
    }
  }
}
```

![image-20250725164819093](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725164819093.png)

### 1.3 续杯方式

![image-20250725165453985](https://cdn.jsdelivr.net/gh/anlostsheep/infinity-images@master/uPic/2025/07/image-20250725165453985.png)

#### 删除账号后重新登陆，官方方式

**第二步：使用[GitHub](https://zhida.zhihu.com/search?content_id=252819009&content_type=Article&match_order=1&q=GitHub&zhida_source=entity)工具修改Machine ID**

当更换邮箱的方法失效后，我们可以通过修改Cursor的**Machine ID**来重置试用次数。以下是详细步骤：

**1. 下载GitHub工具**

首先，我们需要下载一个GitHub上的开源工具，地址是：[https://github.com/fly8888/cursor_machine_id](https://link.zhihu.com/?target=https%3A//github.com/fly8888/cursor_machine_id)。这个工具可以帮助我们生成新的Machine ID。

**2. 运行工具生成新的Machine ID**

下载完成后，解压文件，运行其中的`exe`文件。点击“Generate”按钮，工具会自动生成一个新的Machine ID。

**注意**：这个方法需要一定的技术基础，操作时请务必小心，避免误操作导致系统问题。

**第三步：结合邮箱更换与Machine ID修改**

1. **先用邮箱更换**
	：每次试用期快结束时，更换一个新邮箱，重新注册Cursor账号，享受新的试用期。
2. **当邮箱更换失效时**
	：当Cursor提示“试用次数过多”时，使用GitHub工具修改Machine ID，重置试用次数。
3. **循环使用**
	：通过不断更换邮箱和修改Machine ID，你可以无限次延长Cursor的试用期。



#### cursor-auto-free

参照站点：https://cursor-auto-free-doc.vercel.app/zh/quick-start.html

成品可购买：https://curser.zone.id/products



#### poolhub.me

站点(已停用)：https://poolhub.me/
