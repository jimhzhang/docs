**CodeCC介绍文档 - 二方版**
# **CodeCC简介**
代码检查，一般又称为静态代码分析，是指无需运行被测代码，仅通过分析或检查源程序的语法、结构、过程、接口等来检查程序的正确性，找出代码隐藏的错误和缺陷，如内存泄漏，空指针引用，死代码，变量未初始化，复制粘贴错误，重复代码，函数复杂度过高等等。

CodeCC（代码检查中心）提供专业的代码检查解决方案，检查缺陷、漏洞、规范等多种维度问题，为产品质量保驾护航。
#
# **CodeCC能解决的问题以及交付后默认支持的工具集**

<table><tbody>
<tr>
  <td><b>维度</td>
<td><b>类别</td>
<td><b>工具示例</td>
<td><b>规则示例</td>
  </tr>
  <td rowspan="3"><b>代码问题<b></td>
<td><b>发现代码缺陷</td>
<td>
<p>Clang、Clangwarning、SpotBugs</p>
<p><b>预计22年下半年可用：</b></p>
<p>bkcheck-cpp</p>
<p><b>需要使用自行采买License：</b></p> Coverity、KLOCWORK</p></td>
<td>API使用、内存非法访问、程序卡死、资源泄露、空指针、性能低效……</td>
</tr>
<tr>
<td><b>发现安全漏洞</b></td>
<td><p>啄木鸟敏感信息工具</p><p></p><p><b>需要使用自行采买License：</b></p><p>CheckMarx</p></td>
<td>凭证泄露、不和谐内容、员工信息泄露等等，支持任意文本内容，不局限于特定编程语言范围</td>
</tr>
<tr>
<td><b>代码规范，检查一些逻辑错误</b></td>
<td><p>CppLint、CheckStyle、ESLint、StyleCop、Gometalinter、detekt、PHPCS、PyLint、OCCheck、Clangwarning、</p><p><b>预计22年下半年可用：</b>bkcheck-oc、bkcheck-cpp</p><p></p>
<td>注释、空代码块、异常处理、命名、格式化、风格……</td>
</tr>
<tr>
<td><b>复杂度</b></td>
<td><b>控制复杂度</td>
<td>圈复杂度</td>
<td>函数圈复杂度>=20</td>
</tr>
<tr>
<td><b>重复代码</b></td>
<td><b>检测重复率</td>
<td>重复率</td>
<td>文件代码重复率>=5%</td>
</tr>
<tr>
<td><b>代码统计</b></td>
<td><b>统计代码行数</td>
<td>代码统计（CLOC）</td>
<td>统计代码中各类语言代码行、注释行、空白行的情况</td>
</tr>

</tbody>
</table>
  

# **CodeCC的特色功能**
**支持五大检查维度：**

目前已集成十余款含商用、开源、腾讯自研的代码检查工具，覆盖代码缺陷、安全漏洞、编码规范、圈复杂度、代码重复率五大维度。

**丰富的平台功能：**

通过快速准确地分析源代码，找出质量问题和安全漏洞，并提供自助接入、实时扫描、告警展示、告警屏蔽、定时日报、修复激励等功能。

**质量红线（计划2022年中对外开放）：**

与蓝盾流水线进行了深度整合，通过质量红线服务，可以在流水线中使用CodeCC的检查结果来控制代码库MR/PR、转测、部署等流程，从而使得每一阶段的流水线产出都符合质量标准。

**工具自助上架（计划2022年下半年对外开放）：**

支持工具开发框架和规则开发框架，覆盖八种常用编程语言。
#
# **CodeCC的落地成本**
**部署前提：**

已完成蓝盾的部署

**CodeCC的部署成本：**

8核-16G内存-50G系统盘-200G磁盘，1台

**CodeCC部署周期：**

1天（部署+验收）

**部署实施方：**

蓝盾支持团队
#
# **如何启动下一步**
**如果您想要先试用：**

我们的体验环境能够满足您对功能测试的需求，欢迎随时您的对接人。他会为您提供体验环境账号以及登录方式等信息。

**如果您想要直接部署使用：**

欢迎随时联系您的对接人，在硬件资源准备就绪后，我们会随时启动。

# **FAQ**
**Q：我可以使用Coverity的能力吗？**

A：Coverity需要您自行进行License采买。采买完成后，可以直接通过CodeCC插件调用Coverity对您的代码进行扫描。其他商业的代码扫描工具同理。

**Q：我可以把我使用的，但是不包含在现有工具集中的工具接入CodeCC使用吗？**

A：我们将在22年下半年提供“自定义上架工具”满足该需求。

**Q：我可以对工具中涵盖的规则集进行自定义的调整从而满足我们的使用需求吗？**

A：我们将在22年下半年提供“自定义上架工具”满足该需求。

# **附录：各工具详细介绍**

<table><tbody>
<tr>
  <td><b>维度</td>
<td><b>工具</td>
<td><b>工具ID</td>
<td><b>支持语言</td>
<td><b>License类型</td>
<td><b>CodeCC交付后立即可用</td>
<td><b>工具介绍</td>
</tr>
<tr>
<td rowspan="6"><b>发现代码缺陷</td>
<td><b>Coverity</td>
<td>COVERITY</td>
<td>C/C++,JAVA,C#,JS,<br>OC/OC++,Python,PHP,<br>Ruby,Golang,Swift,TS</td>
<td>商业</td>
<td>否</td>
<td>斯坦福大学科学家研究成果，被第三方权威调查机构VDC评为静态源代码分析领域的领导者。</td> 
</tr>
<tr>
<td><b>Klocwork</td>
<td>KLOCWORK</td>
<td>C/C++,JAVA</td>
<td>商业</td>
<td>否</td>
<td>业界广泛使用的商用代码检查工具，可与Coverity互为补充，通过覆盖更多的逻辑路径，能更全面地扫描空指针、内存泄漏、越界溢出等问题。</td>
</tr>
<tr>
<td><b>PVS-Studio</td>
<td>PVS</td>
<td>C++</td>
<td>商业</td>
<td>否</td>
<td>能够进行综合的静态分析(包括各类缺陷和安全漏洞)，并避免带干扰性的结果，能够与多种IDE集成。其卓越的静态分析技术能够覆盖一般动态测试才能实现的功能，从而把缺陷的发现提早到了第0时间。大大减少了缺陷管理的成本，缩短了周期。PVS-Studio提供的静态分析技术能够发现代码的指针问题、数组越界问题、内存使用问题、编码规则违反的问题</td> 
</tr>
<tr>
<td><b>Clang</td>
<td>CLANG</td>
<td>OC/OC++</td>
<td></td>
<td>是</td>
<td>Clang静态检查工具是Clang编译器下的一款代码检查工具，可以通过推理代码的语义，在项目编译的过程中扫描出项目中存在的bug，例如空指针、API错误使用、无效代码、安全问题等。目前支持84种问题类型。</td>
</tr>
<tr>
<td><b>Clangwarning</td>
<td>CLANGWARNING</td>
<td>OC/OC++</td>
<td></td>
<td>是</td>
<td></td>
</tr>
<tr>
<td><b>bkcheck-cpp</td>
<td>BKCHECK-CPP</td>
<td>C/C++</td>
<td>即将开源</td>
<td>否</td>
<td><p>基于原始的BKCHECK进行新一轮改造，增加多语言扩展支持，实现深度抽象语法树解析、控制流分析等静态分析基础组件。</p><p>目前支持C/C++，新增超过13例新规则，包含空指针检查、逻辑缺陷、代码风格等多种类型。</p><p></p></td>
</tr>
<tr>
<td rowspan="2"><b>发现代码缺陷</td>
<td><b>啄木鸟敏感信息工具</td>
<td>WOODPECKER\_SENSITIVE</td>
<td>所有语言</td>
<td>腾讯自研</td>
<td>是</td>
<td><p>由TEG安全平台部打造的工具，覆盖认证凭证泄露、不和谐内容、员工信息泄露等等，支持任意文本内容，不局限于特定编程语言范围。</p><p></p></td>
</tr>
<tr>
<td><b>CheckMarx</td>
<td>CODEAUDIT</td>
<td>JAVA,Golang,JS,<br>Python,PHP,TS</td>
<td>商业</td>
<td>否</td>
<td><p></td>
</tr>
<tr>
<td rowspan="11"><b>检查代码规范</td>
<td><b>CppLint</td>
<td>CPPLINT</td>
<td>C/C++</td>
<td>开源</td>
<td>是</td>
<td><p>谷歌开源的C++代码风格检查工具，可确保C++代码符合谷歌编码规范，并能检查语法错误。</p><p></p></td>
</tr>
<tr>
<td><b>CheckStyle</td>
<td>CHECKSTYLE</td>
<td>JAVA</td>
<td>开源</td>
<td>是</td>
<td>用于检查Java源代码是否符合编码规范。它可以找到类和方法设计问题，还能够检查代码布局和格式问题。</td>
</tr>
<tr>
<td><b>ESLint</td>
<td>ESLINT</td>
<td>JS</td>
<td>开源</td>
<td>是</td>
<td>开源的JavaScript 代码检查工具，可以在开发阶段发现代码问题，支持最新的ES6语法标准，支持前端框架Vue和React等。</td>
</tr>
<tr>
<td><b>StyleCop</td>
<td>STYLECOP</td>
<td>C#</td>
<td>开源</td>
<td>是</td>
<td>微软的开源静态代码分析工具，它检查C＃代码是否符合StyleCop推荐的编码样式和Microsoft.NET Framework设计指南。</td>
</tr>
<tr>
<td><b>Gometalinter</td>
<td>GOML</td>
<td>Golang</td>
<td>开源</td>
<td>是</td>
<td>一款开源的Golang 代码检查工具，支持检查代码规范、死代码、语法错误和安全漏洞等问题。</td>
</tr>
<tr>
<td><b>detekt</td>
<td>DETEKT</td>
<td>kotlin</td>
<td>开源</td>
<td>是</td>
<td>Kotlin语言代码分析工具，除了能扫出编码的风格规范问题之外，还能检查出代码的复杂度、某些潜在逻辑错误以及性能问题，告警类型多达152种。</td>
</tr>
<tr>
<td><b>PHPCS</td>
<td>PHPCS</td>
<td>php</td>
<td>开源</td>
<td>是</td>
<td>PHP\_CodeSniffer用于检查PHP的编码规范。PHPCS支持包括PEAR、PSR-1、PSR-2、PSR-12等5类代码规范标准，涵盖257种告警类型。</td>
</tr>
<tr>
<td><b>PyLint</td>
<td>PYLINT</td>
<td>python</td>
<td>开源</td>
<td>是</td>
<td>Python代码风格检查工具，可检查代码行的长度、变量命名是否符合编码规范或声明的接口是否被真正的实现等。</td>
</tr>
<tr>
<td><b>bkcheck-cpp</td>
<td>BKCHECK-CPP</td>
<td>C/C++</td>
<td>即将开源</td>
<td>否</td>
<td><p>基于原始的BKCHECK进行新一轮改造，增加多语言扩展支持，实现深度抽象语法树解析、控制流分析等静态分析基础组件。</p><p>目前支持C/C++，新增超过13例新规则，包含空指针检查、逻辑缺陷、代码风格等多种类型。</p><p></p></td>
</tr>
<tr>
<td><b>bkcheck-oc</td>
<td>BKCHECK-OC</td>
<td>OC/OC++</td>
<td>即将开源</td>
<td>否</td>
<td><p></td>
</tr>
<tr>
<td><b>ClangWarning</td>
<td>CLANGWARNING</td>
<td>OC/OC++</td>
<td>开源</td>
<td>是</td>
<td><p></td>
</tr>
<tr>
<td><b>控制复杂度</td>
<td><b>圈复杂度</td>
<td>CCN</td>
<td>JAVA,C#,Golang,C/C++,<br>OC/OC++,JS,PHP,Ruby,<br>Python,Swift,LUA</td>
<td>开源</td>
<td>是</td>
<td><p>通过计算函数的节点个数来衡量代码复杂性。复杂度越高代码存在缺陷的风险越大。</p><p></p></td>
</tr>
<tr>
<td><b>检测重复代码</td>
<td><b>重复率</td>
<td>DUPC</td>
<td>Golang,JAVA,C#,<br>C/C++,OC/OC++,JS,<br>Kotlin,Python,<br>Python,Swift,LUA</td>
<td>开源</td>
<td>是</td>
<td><p>可以检测项目中复制粘贴和重复开发相同功能等问题，帮助开发者发现冗余代码，以便代码抽象和重构。</p><p></p></td>
</tr>
<tr>
<td><b>统计代码行数</td>
<td><b>代码统计</td>
<td>CLOC</td>
<td>所有语言
<td>开源</td>
<td>是</td>
<td><p>统计代码中各类语言代码行、注释行、空白行的情况。</p><p></p></td>
</tr>
</tbody>
</table>



