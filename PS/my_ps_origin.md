
## 写作思路


**思路**

第一部分（兴趣和基本情况）
- 从科幻小说引入，对机器人感兴趣
- 看到各种智能设备，好奇其如何实现（玩具车、无人机）
- 中学阶段的学习中打下了不错的数理基础，最终去到了中国顶尖大学
- 在大学选专业时，对电子、控制和计算机都很感兴趣，于是选择了自动化专业这样一个交叉专业（将电子工程、控制理论与AI技术结合）

第二部分（大学课程、项目经历）
- 在大学学习期间，学习了什么课程（举例，重点在于自己的知识的广度和理论实践的结合）
- 并不满足于理论知识的学习，还参与各种项目的制作
- 大一的项目（做了什么，主要是熟悉了开发的流程，发现自己对电控的兴趣，无论是写代码还是设计PCB，都很有趣，开始主动自学）
- 在接下来的时间里，还主导了一个物流搬运机器人的比赛项目（硬件的PCB设计，软件的驱动，整体的控制思路，还帮忙辅助视觉功能的实现）

第三部分（问题和留学动机）
- 在项目中遇到了一些问题（只会简单的控制，电路设计也有困难，发现还缺少一些理论深度和更丰富的项目实践）
- 以后想从事xxx相关的工作，觉得EE相关是未来人类社会发展的重要方向，但觉得自己的能力还需要继续学习
- 于是想要去进行更为深入的学习，且想出国进行深造和体验

第四部分（目标大学和项目）
- 在阅读文献的过程中，发现xxx大学的xxx老师或者xxx院系在xxx领域有很深的造诣，且xxx项目在xxx领域处于国际领先地位
- 于是想要申请xxx大学的xxx项目，并希望在xxx老师的指导下进行深入的学习


## 正文

**第三版**

修改思路：
- 加入更为丰富的递进思考的过程，比如最开始只是对如何实现感兴趣，后来开始考虑如何能实现地更好
- 智能是什么（只是软硬件的结合吗？还是有更深层次的科学哲学内涵）


第一部分：
“是什么让设备产生了智能？”这个问题在我小时候阅读阿斯莫夫的机器人小说时突然出现在我的脑海中，自此我开始思考各种智能设备的工作原理。
有一次家里的遥控车坏了，我拆开来，看到了复杂的PCB电路板和电机，那些精密复杂的构造使我着迷。我迫切地想弄懂PCB上各个器件是如何工作的，又是如何驱动电机旋转的，(但中学的知识深度不足以支撑我的思考)。于是中学毕业后，满怀对电子工程的兴趣和对交叉学科的热情，我选择了哈尔滨工业大学（深圳）的自动化专业，一个具有复合人才培养体系和深厚工程底蕴的专业


第二部分：
各种电子设备的软硬件和控制算法的原理是什么？这是我本科课程学习的主线内容。
在学习完数电模电的内容后，我通过自行设计并焊接的DC-DC buck-boost电路，了解了基本的硬件设计流程和原理。在学习控制理论的过程中我借助线性代数等数学工具进行分析和计算，还编写matlab仿真程序对控制系统的频率特性进行分析，提升了自己的数学和编程能力。在有了以上的基础后，我在ROS机器人平台上部署了一些机器视觉识别算法，实现了机器人对颜色的识别和目标的追踪。自己用pytorch完成了U-net网络的实现并实现了90%以上的目标识别准确度。

比知道智能设备工作原理更让我着迷的是自己赋予设备智能的过程。于是在课程学习之外，我还积极参与各种项目和比赛。

在大一的时候我和几个同学一起参与了一个智能自行车码表的项目。
当时我们缺少实际开发的经验，于是对照官方使用文档开始自学。我们分析示例工程的的驱动程序实现，我主导了GPS模块、蓝牙模块和墨水屏的驱动程序移植。最终我们完成了程序设计和硬件设计，实现了速度显示、摔倒检测、GPS定位、10h续航等功能。
在项目制作的过程中，我熟悉了从软件到硬件的基本开发流程，也在PCB设计、程序编写中更加坚定了自己对电子工程的兴趣和热情，开始在课外参与更多的项目，自学了PCB设计，并阅读了很多开源项目代码。更重要的是，当发现其它成员编写的模块功能函数复杂且缺少调用接口时，我便意识到自己并不只满足于功能的实现，而是想要完成一个设计合理、功能完善、性能优异的智能设备产品。

于是到了大三，我参与了一个物流搬运机器人比赛。此时我已经掌握了硬件设计和软件开发的基本方法，作为机器人开发的主要负责人，我在开发的过程中不满足于基本功能的实现，而是开始注重规范性与可拓展性，真正像做一个产品一样去设计这个机器人。
在硬件方面，我设计了一块10\*10cm的STM32的拓展板，集成了降压模块、串口模块、供电接口、电机和舵机接口、无线继电器开关和无线调试器。在减小拓展板尺寸的同时满足了功率负载要求和信号完整性要求。
在软件方面，我还将yaw轴陀螺仪与电机编码器结合，开发了一套基于陀螺仪角度反馈的位置-速度闭环的底盘控制算法，实现了cm级别的移动精度和流畅的运动启停。还配合树莓派openCV库进行目标与颜色识别，采用PID控制机械臂实现了mm级别的物料放置精度。
我还设计了模块化的软件架构，针对各种异常情况设计了应对机制，为各个模块和函数编写了详细的使用说明和文档，引入git进行代码版本的管理。这样不管是后续的继续开发还是进行功能的调整，都能快速而便利地进行。
在最终的比赛中，我们分工协作，凭借稳定的控制效果和充分的准备取得了全国第五的成绩。
在这个项目中，我不光将自己所学的知识应用到了实际中，也在产品开发、团队协作、项目管理等方面有了更深入的理解。认识到一个成功的智能设备，绝对不是软件和硬件的简单堆叠，而是软件算法、硬件设计与系统工程思维三者的有机统一，这种系统化的工程思维成为了我日后学习和思考的核心方法论。


第三部分：
随着比赛的结束，我未来的目标愿景也变得更为清晰：“让设备变得更为智能”。在完成各种项目的过程中，我接触到了从硬件设计到软件开发的整个流程，了解了如今各种智能设备的复杂程度，也对自身的工程技术能力进行了更为深入的思考。在调试机器人的时候我发现，传统的PID控制器面对机械结构的非线性摩擦和负载的突变，难以达到稳定的控制效果，想要在实际工程和应用中达到快速而稳定的控制效果，需要学习诸如MPC等更为复杂的控制方法。同样的，在PCB设计中，我虽然能满足基本的功率和信号传输的要求，但如果涉及到高速信号完整性、信号隔离、功耗管理等更为复杂的要求，我仍然缺乏系统的学习。我希望前往一个更为国际化的学术环境中去，在多元观点的碰撞中，获得更广阔的视野。而香港（新加坡）作为东西方技术与文化的交汇点，完美契合了我的需求。




**第二版**
第一部分：
我对电子工程的兴趣源自小时候阅读阿西莫夫的机器人小说，一个名为丹尼尔的具有智能和情感的机器人点燃了我探究各种智能设备原理的热情。
到了中学，我学习到了电机驱动的简单原理。回到家拆开了自己的玩具遥控车，看到了复杂的PCB电路板和各种芯片，那些精密复杂的构造使我着迷。从那时起，我便下定决心去探究各种电子设备从设计到应用的原理。
当进入大学后，满怀对电子工程的兴趣和对交叉学科的热情，我并不满足于仅仅深入某一个方向学习，而是想要获得一个更为广阔的视野。受到其复合人才培养体系与深厚工程底蕴的吸引，我选择了哈尔滨工业大学（深圳）的自动化专业。


第二部分：(课程内容加入更多细节，比如着重分析某一个课程)
本科阶段的课程为我构建了一个从理论到应用的完整知识体系。我的课程学习也是一个不断将理论付诸实践的过程。
我在学习控制理论的过程中使用线性代数等数学工具进行分析和计算，在matlab中编写仿真程序分析不同控制系统的频率特性。
学完数电模电后，我不满足于理论知识，而是自己设计了DC-DC转换电路并进行PCB的焊接和调试。
我还学习了机器视觉中基本的图像处理和识别方法，在ROS机器人平台上部署了识别算法，实现了机器人对颜色的识别和目标的追踪。
我对机器学习也颇感兴趣，在模式识别课程设计中利用pytorch完成了U-net网络的实现并实现了90%以上的目标识别准确度。


在课程学习之外，我还积极参与各种项目和比赛。

在大一的时候我和几个同学一起参与了一个智能自行车码表的项目。
当时我们缺少实际开发的经验，于是对照官方使用文档开始自学。我们分析实例工程的的驱动程序实现，我主导了GPS模块、蓝牙模块和墨水屏的驱动程序移植。为了降低了整个码表的功耗，我重新设计了UI界面的显示逻辑。我还提议在各个功能模块中设计好API接口，方便在工程中直接调用。
最终我们完成了程序设计和硬件设计，实现了速度显示、摔倒检测、GPS定位、10h续航等功能。
在完成这个项目后，我熟悉了从软件到硬件的基本开发流程，也在PCB设计、程序编写中更加坚定了自己对电子工程的兴趣和热情，开始在课外参与更多的项目，自学了PCB设计，并阅读了很多开源项目代码。（初步觉得，不满足于仅仅的实现，还想要做好，做完美）

到了大三，我参与了一个物流搬运机器人比赛。此时我已经掌握了硬件设计和软件开发的基本方法，作为机器人开发的主要负责人，我在开发的过程中不满足于基本功能的实现，而是开始注重规范性与可拓展性，并满足各种性能指标要求。
在硬件方面，我设计了一块10\*10cm的STM32的拓展板，集成了降压模块、串口模块、供电接口、电机和舵机接口、无线继电器开关和无线调试器。在减小拓展板尺寸的同时满足了功率负载要求和信号完整性要求。
在软件方面，我还将yaw轴陀螺仪与电机编码器结合，开发了一套基于陀螺仪角度反馈的位置-速度闭环的底盘控制算法，实现了cm级别的移动精度和流畅的运动启停。还配合树莓派openCV进行目标与颜色识别，采用PID控制机械臂实现了mm级别的物料放置精度。
我还设计了模块化的软件架构，针对各种异常情况设计了应对机制，为各个模块和函数编写了详细的使用说明和文档，引入git进行代码版本的管理。
在最终的比赛中，我们分工协作，凭借稳定的控制效果和充分的准备取得了国家级的奖项。
在这个项目中，我不光将自己所学的知识应用到了实际中，也在产品开发、团队协作、项目管理等方面有了更深入的理解。也认识到一个成功的产品，绝对不是软件和硬件的简单堆叠，而是软件算法、硬件设计与系统工程思维三者的有机统一，这种系统化的工程思维成为了我日后学习和思考的核心方法论。


第三部分：
在完成各种项目的过程中，我接触到了从硬件设计到软件开发的整个流程，也对自身的工程技术能力进行了更为深入的思考。在调试机器人的时候我发现，传统的PID控制器面对机械结构的非线性摩擦和负载的突变，难以达到稳定的控制效果，想要在实际工程和应用中达到快速而稳定的控制效果，需要学习诸如MPC等更为复杂的控制方法。同样的，在PCB设计中，我虽然能满足基本的功率和信号传输的要求，但如果涉及到高速信号完整性、信号隔离、功耗管理等更为复杂的要求，我仍然缺乏系统的学习。

随着我不断的学习和思考，我逐渐意识到未来的智能系统开发需要兼通软件控制、硬件设计、系统集成等方面的人才。我以后想从事嵌入式开发相关的工作，但我认为本科阶段的学习还达不到我期望的知识深度，我也希望前往一个更为国际化的学术环境中去，在多元观点的碰撞中，获得更广阔的视野。而香港（新加坡）作为东西方技术与文化的交汇点，完美契合了我的需求。

第四部分：
而在查找资料和阅读文献的过程中，我发现xxx学校的xxx项目在xxx领域处于国际领先地位，并且xxx课程和实验室能够补足我本科阶段学习的不足。

不光拥有世界级的实验室，更与全球领先的科技产业紧密相连，


**第一版**
我最初的兴趣源于小时候读科幻小说。在阿西莫夫的机器人系列小说中，我被一个叫丹尼尔的人形机器人深深地吸引了，他拥有一个“正子脑”，能够模拟人类的感受和思考，并且拥有超强的记忆力和处理能力。我对这个机器人产生了非常深刻的印象，并好奇这些智能人形机器人的可实现性？到了中学阶段，随着对自然科学的深入学习，我不满足于虚构的科幻，而是从身边的实物开始探索和了解。从简单的电视遥控器、电热水壶到玩具无人机，我都将它们的外壳拆开过，看到了复杂的PCB板和上面的各种元件和芯片，这些设备尤其是其中的电路芯片的精密构造使我着迷，促使我不断思考他们是如何实现各种复杂功能的，尤其是软件和硬件是如何协同工作的。



到了大学，为了在xx领域获得一个更为广阔和全面的视野，我修读了自动化专业。这个专业将电子工程、控制理论与AI技术结合，有丰富的课程内容。我在学习控制理论的过程中掌握了使用线性代数等数学工具进行分析和计算的能力，在学习数电模电课程的同时还通过实际DC-DC电路的设计和分析获得了实践，在数字图像处理和模式识别等课程中，我将所学的理论知识和算法在ROS和linux环境中通过编程进行实现。


我在学习控制理论的过程中掌握了使用线性代数等数学工具进行分析和计算的能力，在学习数电模电课程的同时还通过实际DC-DC电路的设计和分析获得了实践，在数字图像处理和模式识别等课程中，我将所学的理论知识和算法在ROS和linux环境中通过编程进行实现。我在学习控制理论的过程中掌握了使用线性代数等数学工具进行分析和计算的能力，在学习数电模电课程的同时还通过实际DC-DC电路的设计和分析获得了实践，在数字图像处理和模式识别等课程中，我将所学的理论知识和算法在ROS和linux环境中通过编程进行实现并控制机器人实现特定功能。

在本科阶段丰富的课程中我打下了较为扎实的数学、电路、编程和控制基础。  

我并不仅仅满足于理论知识的学习，也在课余时间积极参与实际项目的制作。在大一我参与完成了一个智能自行车码表的项目。这是我第一次接触到完整的产品开发流程，当时我对于如何开发一个产品毫无概念，于是我们项目团队的成员先去开源社区和论坛寻找设计思路和教程，然后经过讨论初步确定了几版方案思路交由指导老师进行审阅。但当方案确定后，其实我们对于具体的开发还无从下手，于是将项目根据功能和模块分为显示屏、GPS定位、陀螺仪姿态估计等几个部分，每个人针对一到两个部分开展自学。在硬件部分我们学习了PCB原理图的绘制，自己完成了元器件和电路板的焊接。在软件部分我们自己阅读官方开发文档完成了esp-idf开发环境的配置，学习示例工程中蓝牙等功能的写法并加以修改。在各自模块功能完成后我提议编写了一些API接口和使用实例说明，让调用这些功能模块更为方便。  

在完成这个项目之后，我熟悉了从软件到硬件的基本开发流程，了解了从零开始进行开发和学习的过程，也初步感受到了分工协作的必要性。在接下来的时间里，我还参与了几个项目，对电子领域各个方面也进行了更为深入的学习。在项目开发中并不仅满足于基本功能的实现，而开始注重规范性和满足各种指标要求。其中有代表性的是一个物流搬运比赛机器人。在这个机器人项目中，我设计了STM32的拓展板，集成了降压模块、串口模块、供电接口和信号线，还集成了无线继电器开关和无线调试器等，相比之前的项目在供电安全、信号隔离等多种方面有了更为全面的考量。我也负责开发机器人的软件控制部分，通过步进电机配合陀螺仪控制机器人四轮底盘实现精准快速移动，对工程的各个模块进行了合理的代码结构封装，可以适应不同功能需求的开发修改。还采用了更为规范的代码版本管理，便于进行协同开发和修改。在完成这个项目的过程中，我的代码能力得到了明显的提升，积累了更为规范的工程管理和项目制作经验，也通过从具体负责和实现从硬件电路到软件功能的各种设计实现，积累了扎实的软硬件实践经验，对电子领域的各个分支有了更加综合全面的感受和理解。  

在进行理论课程学习和完成实际项目的过程中，我遇到了许多问题，在进行控制器设计时只会使用最简单的PID进行控制，对于更复杂的控制理论缺乏足够的了解。在进行PCB版图设计时仍然对信号完整性、高速信号布线和一些电路的实现原理知之甚少。在进行机器人开发时，对于一些底层的指令集架构和程序运行原理仍是一知半解。于是我迫切希望进行更为深入的学习。  

而我了解到，xxx贵校xxx项目，具有广泛的国际影响力和认可度，提供xxx课程，可以补足我xxxx不足的部分。我以后想从事xxx行业相关的工作，这些课程和项目有助于我的职业规划和发展

我深知 [目标大学] 的 [目标项目名称] 在 [提及项目特色，例如：先进控制理论、机器人感知与决策、智能制造等] 领域处于国际领先地位。尤其是 [提及具体吸引你的课程、实验室或教授的研究方向，例如：XXX教授在鲁棒控制方面的研究、YYY实验室在多机器人协作系统的实践机会]，与我当前希望深化的方向高度契合。我相信在 [目标大学] 严谨的学术氛围和丰富的科研资源下，我不仅能够弥补现有知识短板，系统掌握前沿理论和技术，更能有机会参与到高水平的科研项目中，将理论知识与更复杂的实际问题相结合，进一步提升我的研究能力和创新能力。我的扎实基础、丰富的项目经验以及强烈的求知欲和解决问题的能力，使我深信我能够顺利完成 [目标项目名称] 的学业，并为该领域的未来发展做出贡献。

我渴望在 [目标大学] [目标项目名称] 项目中接受更深入的学术训练，与优秀的师生共同探索自动化与智能系统领域的未知前沿。我坚信，凭借我过去积累的软硬件基础和解决问题的热情，结合 [目标大学] 提供的顶级教育资源，我将能够实现学术上的飞跃，为未来在相关领域进行更高层次的研发工作打下坚实基础。

## 第二版英文AI稿
My first fascination with intelligent machines came not from a laboratory, but from the pages of Isaac Asimov’s robot novels. The sentient robot R. Daneel Olivaw sparked a deep curiosity in me: What gives a machine its intelligence? This question led me to dismantle my toy car in middle school, captivated by the intricate circuits on its PCB. Since then, I have been determined to explore the underlying principles of electronic devices, from design to implementation.

Motivated by this curiosity and a desire for interdisciplinary learning, I chose to pursue Automation at Harbin Institute of Technology, Shenzhen (HIT Shenzhen), a program known for its strong engineering foundation and cross-disciplinary curriculum. My undergraduate studies provided me with a solid theoretical and practical background. In Control Theory, I applied linear algebra to system analysis and wrote MATLAB scripts to simulate frequency characteristics. Moving from theory to practice, I designed and debugged a DC-DC converter and explored machine vision by deploying recognition algorithms on the ROS platform. My interest in machine learning also grew as I implemented a U-Net model with PyTorch for a pattern recognition project, achieving high accuracy in target identification.

Beyond my coursework, I have actively sought out hands-on experience through various projects and competitions. During my freshman year, I collaborated on a smart bicycle computer project. With limited practical experience, we relied on official documentation and self-learning. I took the lead in porting the drivers for the GPS, Bluetooth, and e-ink display modules. To reduce power consumption, I redesigned the UI display logic. Furthermore, I proposed the implementation of modular API interfaces, which significantly streamlined our team's development process. Our final product successfully integrated features such as real-time speed display, fall detection, GPS positioning, and a 10-hour battery life. This project provided me with a holistic understanding of the hardware-to-software development workflow and solidified my passion for electronics. (add more about passion and interest when doing the project)

By my junior year, I served as the lead developer for a logistics robot in a national competition, shifting my focus to system robustness and scalability. On the hardware front, I designed a compact 10x10 cm STM32 expansion board that integrated modules for power conversion, serial communication, motor/servo control, and wireless relays/debuggers, all while meeting stringent power load and signal integrity requirements. On the software side, I developed a position-velocity closed-loop control algorithm for the chassis by fusing data from a yaw-axis gyroscope and motor encoders, achieving centimeter-level motion accuracy and smooth kinematics. Collaborating with a Raspberry Pi for computer vision, I implemented a PID controller for the robotic arm that achieved millimeter-level placement accuracy. To ensure a smooth development process, I introduced Git for version control, built a modular software framework, and wrote comprehensive documentation for all modules. Our team’s synergy and the robot’s stable performance earned us a national-level award.

This project was more than a practical application of my knowledge; it gave me a profound understanding of product development, teamwork, and project management. I learned that a successful product is not a simple stack of hardware and software, but an organic integration of algorithms, hardware design, and systems engineering thinking. This systems-level methodology has become the cornerstone of my approach to learning and problem-solving.

However, these projects have also revealed the limits of my current expertise. While debugging the logistics robot, I recognized the limitations of traditional PID controllers in handling non-linear friction and abrupt load variations, realizing the need to master advanced techniques such as Model Predictive Control. Similarly, while my PCB designs meet basic requirements, I lack systematic training in high-speed signal integrity, noise mitigation, and advanced power management.

Looking forward, I aim to pursue a career in embedded systems and intelligent robotics. To achieve this, I am eager to immerse myself in a world-class academic environment that provides both the theoretical depth and international perspective I seek. Hong Kong and Singapore, as a nexus of Eastern and Western technology and culture, offer the unique ecosystem where I can refine my expertise and collaborate with peers from diverse backgrounds. 



With a strong foundation in both hardware and software, hands-on experience in building complex systems, and a clear vision for my future, I am confident in my readiness to contribute to and excel in your program.


## 第一版英文AI稿
My initial interest in technology was sparked in childhood by reading science fiction. In Isaac Asimov's robot series, I was deeply captivated by a humanoid robot named Daneel, who possessed a "positronic brain" capable of simulating human feelings and thoughts, coupled with exceptional memory and processing power. This depiction left a profound impression on me and ignited my curiosity about the feasibility of realizing such intelligent humanoid robots. In middle school, as I delved deeper into the natural sciences, my interest moved beyond fictional concepts towards exploring and understanding the real-world objects around me. From simple television remotes and electric kettles to toy drones capable of controlling flight attitude and position, I frequently opened their casings. Inside, I saw complex PCB boards populated with various components and chips. The intricate design of these devices, especially the integrated circuits, deeply fascinated me and led me to constantly ponder how they achieved their complex functions, particularly how software and hardware worked together.
Arriving at university, I chose to major in Automation Engineering to gain a broader and more comprehensive perspective in the field of electronics. This program effectively integrates traditional electronics, control theory, and AI technologies through a rich and varied curriculum. While studying control theory, I gained proficiency in using mathematical tools like linear algebra for analysis and calculation. Parallel to learning digital and analog electronics, I acquired practical experience through the hands-on design and analysis of actual DC-DC circuits. In courses such as Digital Image Processing and Pattern Recognition, I implemented learned theories and algorithms through programming in ROS and Linux environments. These diverse undergraduate courses provided me with a solid foundation in mathematics, circuits, programming, and control systems.
Not content with merely theoretical learning, I actively engaged in hands-on projects during my spare time. In my first year, I participated in completing a smart bicycle computer project. This was my first exposure to the full product development process. Having no prior concept of how to develop a product from scratch, our team members first sought design ideas and tutorials from open-source communities and online forums. After thorough discussion, we preliminarily determined several potential solutions to be reviewed by our advisor. Even after the solution was decided, we initially felt unsure how to proceed with the actual development. Consequently, we collaboratively divided the project into several functional modules such as display, GPS positioning, and gyroscope attitude estimation, with each member undertaking self-directed learning for one or two parts. For the hardware, we learned PCB schematic design and independently completed the component soldering and circuit board assembly. On the software side, we read official development documentation to set up the esp-idf development environment, studied how to implement functions like Bluetooth from example projects, and adapted them for our needs. After completing the individual module functionalities, I took the initiative to propose writing some API interfaces and usage examples to make calling these functional modules more convenient for the team.
Completing this project familiarized me with the fundamental software-to-hardware development flow, taught me the process of learning and developing from scratch, and gave me a preliminary understanding of the necessity of division of labor and collaboration in engineering projects. Subsequently, I participated in several other projects, engaging in deeper learning across various aspects of electronics. In developing these projects, I moved beyond merely achieving basic functionality and began to focus on engineering standards, code quality, and meeting various performance metrics.
A representative example is a robot designed for a logistics handling competition. In this project, I designed an STM32 expansion board, integrating crucial components like step-down modules, serial communication interfaces, power supply connectors, and signal lines. It also incorporated wireless relay switches and a wireless debugger, demonstrating more comprehensive considerations for power safety, signal isolation, and reliability compared to previous projects. I was also responsible for developing the robot's software control system, utilizing stepper motors in conjunction with a gyroscope to achieve precise and rapid movement of the four-wheeled chassis. I structured the code logically with clear encapsulation for various engineering modules, allowing for adaptable development and modification based on different functional requirements. Furthermore, I adopted more standardized code version control, facilitating collaborative development and modification within the team. Completing this project significantly enhanced my coding abilities, built more standardized engineering management and project development experience, and cultivated solid hardware-software practical expertise by being directly responsible for designing and implementing various functions from circuit design to software control. This gave me a more comprehensive understanding and appreciation of different branches within the field of electronics and reinforced my desire to explore complex system integration.
Throughout my theoretical studies and practical project work, I encountered numerous challenges and became aware of my limitations. When designing controllers, for instance, I was often limited to using only the simplest PID control and lacked sufficient understanding of more complex control theories required for optimal performance. Similarly, in PCB layout design, I realized I still had limited knowledge regarding critical aspects like signal integrity, high-speed routing techniques, and the underlying implementation principles of certain complex circuits. When developing robots and embedded systems, I remained somewhat uncertain about underlying instruction set architectures and the fundamental principles of program execution at a low level. Therefore, I am now eager to pursue further, in-depth study to gain a more profound and systematic understanding of these advanced topics.